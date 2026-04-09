# Color Detection with OpenCV

## Overview

This project is a simple real-time color detection system built using **Python**, **OpenCV**, **NumPy**, and **Pillow**.
It captures video from a webcam, detects a specific color (green by default), and draws a bounding box around the detected object.

This project is useful for:

* Learning basic computer vision concepts
* Understanding HSV color space
* Practicing real-time webcam processing
* Building simple object tracking systems

---

## Features

* Real-time webcam video capture
* HSV-based color detection
* Automatic mask creation
* Bounding box around detected object
* Easy to customize for other colors

---

## Technologies Used

* Python
* OpenCV (`cv2`)
* NumPy
* Pillow (`PIL`)

---

## Project Structure

```bash
color-detection/
│
├── main.py          # Main program for webcam color detection
├── util.py          # HSV color range helper function
├── README.md        # Project documentation
```

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install dependencies

```bash
pip install opencv-python numpy pillow
```

---

## How to Run

Run the following command:

```bash
python main.py
```

---

## How It Works

1. The webcam captures live video frames.
2. Each frame is converted from BGR to HSV color space.
3. The program detects the selected color range.
4. A mask is created to isolate the detected color.
5. A bounding box is drawn around the object.

---

## Customization

To detect another color, simply change this line in `main.py`:

```python
green = [0, 255, 0]
```

Example:

* Red → `[0, 0, 255]`
* Blue → `[255, 0, 0]`

---

## Controls

* Press **Q** to quit the application.

---

## Future Improvements

* Support multiple colors
* Add object centroid tracking
* Improve detection accuracy with contour filtering
* Add GUI for color selection

---

## Author

Created as a beginner computer vision project using OpenCV.
