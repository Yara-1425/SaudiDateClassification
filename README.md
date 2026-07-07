# Saudi Dates Classification 

## Project Overview
The dates sector is one of the most vital pillars of agriculture and the economy in the Kingdom of Saudi Arabia. This project aims to automate and optimize the process of sorting and classifying dates to assist Saudi factories and farms in identifying and categorizing their harvest accurately and efficiently.

An Artificial Intelligence (Image Classification) model has been developed to classify two of the most popular types of Saudi dates: **Sukkari** and **Saghai**. By analyzing input images, the model predicts the date type along with a high-accuracy confidence score, significantly reducing manual labor and enhancing production line efficiency.

---

##  Project Structure & Files
```text
├── keras_model.h5         # The exported trained Keras model
├── labels.txt             # Text file containing class names (0 Sukkari, 1 Saghai)
├── saqie.png              # Test image of a Saghai date
└── DateClassfication.py   # Python inference script

```

---

## Step-by-Step Workflow

### 1. Model Training

The image recognition model was trained using **Teachable Machine by Google**. Custom image datasets were uploaded for each category:

* **Sukkari Class:** Samples of Sukkari dates, characterized by their golden color and unique texture.
* **Saghai Class:** Samples of Saghai dates, distinguished by their reddish-brown body and lighter-colored tips.

### 2. Exporting the Model

Once training was successfully completed, the model was exported in the **TensorFlow, Keras** format. The export generated two main files included in this repo:

* `keras_model.h5` (model weights)
* `labels.txt` (class classifications)

### 3. Writing the Python Inference Script

## 4. Testing & Results

The model was evaluated using a test image of a Saghai date (`saqie.png`). The model successfully recognized the date type with a remarkably high precision rate.

### Terminal Execution Output:

```bash
1/1 [==============================] - 1s 525ms/step
Class: صقعي
Confidence Score: 0.9990219

```
