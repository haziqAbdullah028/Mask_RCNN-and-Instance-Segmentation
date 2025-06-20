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

📁 your-project/
├── dnn/
│ ├── frozen_inference_graph.pb
│ └── mask_rcnn_inception_v2_coco_2018_01_28.pbtxt
├── car.jpg # Sample input image
├── mask_rcnn_classes.txt # COCO class labels
├── ground_truth/ # Saved predicted masks (mock GT)
├── script.py # Main code file
└── README.md # Project documentation

yaml
Copy
Edit

---

## ⚙️ Setup & Installation

> Ensure you have Python 3.6+ installed.

### 🔧 Install dependencies:
pip install opencv-python numpy matplotlib

🚀 How to Run
Clone the repository:
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Add your input image as car.jpg (or modify the code to use a different name).

Run the Python script:
python script.py
Output:

Mask images saved in ground_truth/

Printed evaluation metrics in console

Visualized results using matplotlib

📊 Sample Output
yaml
Copy
Edit
[person] Detection 1 — IoU: 1.000, Precision: 1.000, Recall: 1.000
[motorcycle] Detection 16 — IoU: 1.000, Precision: 1.000, Recall: 1.000
[car] Detection 21 — IoU: 1.000, Precision: 1.000, Recall: 1.000

=== Evaluation Summary ===
Mean IoU: 1.000
Mean Precision: 1.000
Mean Recall: 1.000
Currently, the system evaluates predicted masks against themselves (mock ground truth). For real performance measurement, use manually annotated masks.

🧪 Evaluation Metrics
Metric	Description
IoU	Intersection over Union of predicted vs actual
Precision	TP / (TP + FP)
Recall	TP / (TP + FN)

🎨 Visual Results
Bounding Boxes	Segmentation Masks

(Replace with your own image results or screenshots)

📚 References
📘 Mask R-CNN (He et al.)

🧠 OpenCV DNN Module

🧾 COCO Dataset

👨‍💻 Author
Your Name
📧 your.email@example.com
🌐 GitHub

📄 License
This project is licensed under the MIT License.

---

### ✅ Final Tips

- ✅ Replace `your-username`, `your-repo-name`, and `Your Name` with your actual info.
- ✅ Optionally add `examples/boxes.jpg` and `examples/masks.jpg` for GitHub previews.
- ✅ Place this content in `README.md` at your project root.

Let me know if you want a version in Jupyter Notebook, or if you're planning to replace
