<div align="center">

# tensorflow_hysteresis_models

**A TensorFlow 2 / Keras starting point from December 2021: a subclassed Keras model and a custom training loop, trained on MNIST.**

[![Python](https://img.shields.io/badge/Python-3.9-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-Keras-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-notebook-F37626?style=flat-square&logo=jupyter&logoColor=white)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/status-starter%20only-lightgrey?style=flat-square)](#-status)

</div>

## 📌 Status

> [!NOTE]
> No hysteresis model has been committed yet. The only model in the repository is an image classifier for handwritten digits, used to set up the TensorFlow training loop.

## 🗂️ Files

| File | Contents |
|:---|:---|
| `models/BasicModel.py` | `BasicModel(tf.keras.Model)`: `Conv2D(32, 3, relu)` → `Flatten` → `Dense(128, relu)` → `Dense(10, softmax)` |
| `quick_start.ipynb` | Loads MNIST, scales pixels to [0, 1], batches of 32; `@tf.function` train and test steps with `GradientTape`, Adam and sparse categorical cross-entropy; 5 epochs |

## 📈 Saved result

The notebook's saved output for epoch 5 reports a test accuracy of **98.28 %** and a test loss of **0.0659**. Its progress messages are in Spanish (*Perdida*, *Exactitud*).

## 🚀 Getting started

```bash
git clone https://github.com/mavasbel-research/tensorflow_hysteresis_models.git
cd tensorflow_hysteresis_models
python -m pip install tensorflow notebook
jupyter notebook quick_start.ipynb
```

Start Jupyter from the repository root so `from models.BasicModel import BasicModel` resolves. MNIST is downloaded on first run. The notebook was last run with Python 3.9.7; the TensorFlow version it used is not recorded.

This repository does not include a license file.

---

<div align="center">
<sub>Part of <a href="https://github.com/mavasbel-research">mavasbel-research</a> · <a href="https://github.com/mavasbel">Marco Vásquez Beltrán</a></sub>
</div>
