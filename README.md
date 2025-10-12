# 🐶 City Dog Show Image Classifier 🐶
_AWS AI Scholars Program Project One_

> Built to classify pet images using pre-trained CNN models (VGG, ResNet, and AlexNet).  
> Showcases modular Python design, PyTorch fundamentals, and a hands-on look at how accuracy and speed trade off across different models.

---

## 👁️ Project Overview 👁️
This project checks if an image is a **dog or not a dog**, and if it *is* a dog, it digs a little deeper to guess the **breed** using pre-trained CNN architectures.

The goal was to stregthen my understanding of how these deep learning tools really work while focusing on:
- Command-line argument handling with `argparse`
- Working with file I/O and Python dictionaries
- Using pre-trained CNNs for transfer learning
- Measuring runtime and accuracy trade-offs between models

> I built this project as a part of the AWS Scholars program and didn’t train the CNNs from scratch. They came pre-trained as part of the project.  
> My job was to wire everything up in Python, run the classifiers, and figure out which model actually performed best and fastest. Allowing me to get more comfortable bridging theory with real, working code.

---

## 📚 Tech Stack 📚
| Category | Tools |
|-----------|--------|
| Language | Python 3.13 |
| Libraries | PyTorch, Torchvision, Pillow, NumPy |
| Environment | venv |
| Version Control | Git + GitHub |
| IDE | VS Code |

---

## 🏋🏾‍♂️ How It Works 🏋🏾‍♂️
1. **Label Extraction** — Converts filenames into clean, lowercase labels.  
2. **Image Classification** — Feeds each image into a pre-trained model (`--arch vgg`, `--arch resnet`, `--arch alexnet`).  
3. **Evaluation** — Compares classifier output to the true label.  
4. **Timing & Analysis** — Reports accuracy and runtime per model.

---

## 🧪 Example Run 🧪
```bash
# Activate your virtual environment
source .venv/bin/activate

# Install dependencies
python3 -m pip install -r requirements.txt

# Run the classifier
python3 data/check_images.py --dir data/pet_images/ --arch vgg

```
>After running, the results will print in the terminal for each model.
>The full summaries are also stored in the results/ folder as well.
>
>I also uploaded a small batch of photos outside of the provided dataset to see how each model handled it.