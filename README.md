# Lane Line Detection and Vehicle Detection for Self-Driving Cars

## Project Overview

This project focuses on developing a computer vision-based driver assistance simulation using Python, OpenCV, NumPy, and YOLOv8.

The system processes road video footage to detect lane markings, identify nearby vehicles, estimate lane curvature and vehicle position, and display visual safety alerts through a simulated driving dashboard.

## Key Features

- **Lane Detection:** Identifies road lane markings using image processing techniques.
- **Vehicle Detection:** Detects cars, motorcycles, buses, and trucks using YOLOv8.
- **Distance Estimation:** Estimates the approximate distance of detected vehicles.
- **Lane Curvature Estimation:** Calculates the approximate curvature of road lanes.
- **Lane Departure Warning:** Displays warnings when the vehicle moves away from the lane center.
- **Collision Warning:** Generates visual alerts when a detected vehicle is estimated to be too close.
- **Driving Dashboard:** Displays FPS, simulated speed, lane curvature, vehicle position, and vehicle count.
- **Visual Simulation:** Combines the original road video with a simulated driving view.

## Technologies Used

- Python
- OpenCV
- NumPy
- YOLOv8
- Ultralytics
- Computer Vision

## Working Methodology

1. Load the input road video using OpenCV.
2. Process each video frame.
3. Apply YOLOv8 for vehicle detection.
4. Use LAB and HLS color spaces to identify yellow and white lane markings.
5. Apply perspective transformation to obtain a bird's-eye view.
6. Detect lane positions using the sliding window technique.
7. Estimate lane curvature and vehicle position relative to the lane.
8. Generate visual lane departure and collision warnings.
9. Display the processed output with a driving simulation dashboard.
10. Save the final processed video.

## Project Structure

```text
Lane-Line-Detection/
│
├── input_data/
│   └── road_video.mp4
│
├── output_data/
│   └── final_high_contrast_lanes.mp4
│
├── main.py
├── yolov8n.pt
├── requirements.txt
└── README.md
```

## Installation

Install the required libraries:

```bash
pip install opencv-python numpy ultralytics
```

## How to Run

1. Clone the repository.
2. Install the required dependencies.
3. Place the input road video inside the `input_data` folder.
4. Update the input and output folder paths in the Python script.
5. Run the program:

```bash
python main.py
```

## Output

The system generates a processed video containing:

- Detected vehicles with bounding boxes.
- Highlighted road lane boundaries.
- Estimated vehicle distance.
- Lane departure and collision warnings.
- Simulated driving dashboard.

## Applications

- Driver assistance systems
- Autonomous driving research
- Intelligent transportation systems
- Road lane monitoring
- Vehicle safety monitoring

## Future Enhancements

- Improve lane detection under different lighting and weather conditions.
- Integrate vehicle tracking across video frames.
- Improve distance estimation accuracy.
- Explore real-time driver assistance applications.

## Author

**Mangali Sravanthi**

B.Tech – Computer Science and Data Science

