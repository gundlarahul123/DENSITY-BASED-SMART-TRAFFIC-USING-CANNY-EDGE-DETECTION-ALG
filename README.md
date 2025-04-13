# DENSITY-BASED-SMART-TRAFFIC-USING-CANNY-EDGE-DETECTION-ALGORITHM

# Density Based Smart Traffic Control System Using Canny Edge Detection

## 📌 Project Overview

This project presents a **smart traffic control system** that adjusts green light duration based on real-time traffic congestion, detected through image processing using the **Canny Edge Detection Algorithm**.

The system captures road images, processes them to identify white pixels (typically representing vehicles or lane lines), and dynamically allocates green signal time based on the detected traffic density.

## 💡 Features

- GUI built using **Tkinter**
- Image preprocessing using **Canny Edge Detection**
- White pixel count to estimate traffic density
- Dynamic green signal time allocation based on pixel ratio
- Reference image comparison for accurate traffic estimation

## 🖼️ System Workflow

1. **Upload** a traffic image.
2. **Apply** the Canny Edge Detection algorithm.
3. **Count** white pixels (vehicle presence).
4. **Compare** with a reference image.
5. **Allocate** green light signal time based on the congestion level.

## 🧪 Tech Stack

- **Python**
- **OpenCV**
- **Tkinter**
- **Matplotlib**
- **NumPy**
- **Scipy**
- **Skimage**

## 🚦 Green Signal Allocation Logic

Based on the percentage of white pixels in the test image compared to the reference image:

| Traffic Level     | White Pixel % | Signal Time |
|-------------------|---------------|-------------|
| Very High         | ≥ 90%         | 60 seconds  |
| High              | 85% – 89%     | 50 seconds  |
| Moderate          | 75% – 84%     | 40 seconds  |
| Low               | 50% – 74%     | 30 seconds  |
| Very Low          | < 50%         | 20 seconds  |

## 📁 Project Structure

```bash
├── CannyEdgeDetector.py         # Core Canny Edge Detector class
├── main.py                      # Tkinter GUI interface
├── test1.py                     # Script for automated testing
├── gray/                        # Stores processed edge-detected images
│   ├── test.png
│   └── refrence.png
├── images/                      # Directory for sample input images
│   ├── D.png
│   └── refrence.png
🛠️ How to Run
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/yourusername/smart-traffic-control.git
cd smart-traffic-control
2. Install Dependencies
Ensure you have Python 3.x and then install the required packages:

bash
Copy
Edit
pip install numpy matplotlib opencv-python scikit-image scipy
3. Run the GUI Application
bash
Copy
Edit
python main.py
4. Use the Interface
Upload a traffic image

Apply Canny Edge Detection

Count white pixels

View time allocation based on detected congestion

🎯 Applications
Smart City Traffic Management

Real-time Traffic Monitoring

Intelligent Transportation Systems (ITS)

📷 Sample Output

🤝 Contributions
Pull requests and contributions are welcome! Feel free to fork and improve the project.

📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.

vbnet
Copy
Edit

Let me know if you also want a `requirements.txt` or sample screenshots added!
