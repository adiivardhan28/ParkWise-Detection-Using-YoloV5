# 🚗 PARKWISE – Smart Parking Slot Detection using YOLOv5

**PARKWISE** is a smart parking detection system that uses a top-view image and YOLOv5 object detection to identify parked vehicles and determine which parking slots are occupied or vacant.

---

<img width="1675" height="898" alt="Screenshot 2025-06-04 105441" src="https://github.com/user-attachments/assets/3501db5f-e119-4762-bd23-cc92d9962023" />


## 📌 Project Overview

- Detects vehicles using YOLOv5s on a static top-down parking lot image.
- Allows manual marking of parking slots through a simple GUI.
- Determines slot occupancy based on Intersection over Union (IoU).
- Outputs results as both annotated image and CSV reports.

---

## 📁 Folder Structure

```
📦 PARKWISE/
├── yolov5/                  # YOLOv5 model files
├── InputImg.png             # Input parking lot image
├── main.py                  # Main logic for detection & analysis
├── ParkingSpacePicker.py    # GUI for marking parking slots
├── ParkingStatus.csv        # Slot-wise occupancy results
├── ParkingSummary.csv       # Summary of total occupied/vacant
├── slot\_positions           # Pickle file for saved slot data
├── yolov5s.pt               # YOLOv5s weights
└── README.md                # Project documentation

````

## ⚙️ Technologies Used

- **Python 3**
- **YOLOv5s (PyTorch)**
- **OpenCV** (for image handling and GUI)
- **Pandas** (for CSV and data processing)
- **Pickle** (for saving/loading slot positions)

---

## 🚀 How to Run

1. Clone the repo:
```
   git clone https://github.com/sahith215/Parkwise.git
   cd Parkwise
```
3. Install dependencies:
```
   pip install -r yolov5/requirements.txt
   pip install opencv-python pandas
```
5. Mark parking slots:
```
   python ParkingSpacePicker.py
```
7. Run detection:
```
   python main.py
```
---

## 📤 Output

* Annotated parking image showing occupied/vacant slots.
* `ParkingStatus.csv` – Slot-wise status.
* `ParkingSummary.csv` – Total occupied/vacant count.

---

## 👨‍💻 Author

**Sahith**
🔗 GitHub: (https://github.com/sahith215/Parkwise)



