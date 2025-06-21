# 🧠 Mask R-CNN Instance Segmentation & Evaluation Pipeline

This project performs **object detection** and **instance segmentation** on input images using a **pre-trained Mask R-CNN model** with OpenCV’s DNN module. It detects objects like `car`, `person`, and `motorcycle`, overlays segmentation masks, and evaluates predictions using standard metrics: **IoU, Precision, and Recall**.

---

## 📌 Features

- ✅ Load COCO-pretrained Mask R-CNN (`Inception v2`) via OpenCV
- ✅ Detect and segment objects from an input image
- ✅ Draw bounding boxes and overlay color-coded masks
- ✅ Save masks as mock ground truth
- ✅ Compute **IoU**, **Precision**, **Recall** for each instance
- ✅ Display evaluation summary and visualization using matplotlib

---

## 🗂️ Project Structure

📁 mask_rcnn_project/
├── dnn/
│   ├── frozen_inference_graph.pb
│   └── mask_rcnn_inception_v2_coco_2018_01_28.pbtxt
├── car.jpg                     # Sample input image
├── mask_rcnn_classes.txt      # COCO class labels
├── ground_truth/              # Saved predicted masks (mock GT)
├── Mask_RCNN.ipynb            # Jupyter notebook (main code)
└── README.md                  # Project documentation



---

## ⚙️ Setup & Installation

> Ensure you have Python 3.6+ installed.

### 🔧 Install dependencies:
pip install opencv-python numpy matplotlib

## 🚀 How to Run
Clone the repository:
git clone https://github.com/haziqAbdullah028/Mask_RCNN-and-Instance-Segmentation
cd Mask_RCNN-and-Instance-Segmentation

Open the jupyter notebook:
jupyter notebook Mask_RCNN.ipynb
Add your input image as car.jpg (or modify the code to use a different name).


Mask images saved in ground_truth/

Printed evaluation metrics in console

Visualized results using matplotlib

## 📊 Sample Output

[person] Detection 1 — IoU: 1.000, Precision: 1.000, Recall: 1.000
[motorcycle] Detection 16 — IoU: 1.000, Precision: 1.000, Recall: 1.000
[car] Detection 21 — IoU: 1.000, Precision: 1.000, Recall: 1.000

## === Evaluation Summary ===
Mean IoU: 1.000
Mean Precision: 1.000
Mean Recall: 1.000
Currently, the system evaluates predicted masks against themselves (mock ground truth). For real performance measurement, use manually annotated masks.

## 🧪 Evaluation Metrics
Metric	Description
IoU	Intersection over Union of predicted vs actual
Precision	TP / (TP + FP)
Recall	TP / (TP + FN)

## 🎨 Visual Results
## Bounding Boxes	
![image](https://github.com/user-attachments/assets/8f9fb86c-59fa-45c9-b442-a7b0e0c0dfed)
## Segmentation Masks
![image](https://github.com/user-attachments/assets/8d833249-ecc4-4621-90d1-66aa38f5e9e7)


📚 References
📘 Mask R-CNN (He et al.)

🧠 OpenCV DNN Module

🧾 COCO Dataset

👨‍💻 M.Haziq Abdullah
📧 haziqabdullah028@gmail.com
🌐 https://github.com/haziqAbdullah028

📄 License
This project is licensed under the MIT License.

---

