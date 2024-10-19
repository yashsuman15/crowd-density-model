# Crowd Detection Program

This project implements a real-time crowd detection and counting system using YOLOv11 and OpenCV. It processes video input to detect and count people in a scene, providing a visual representation of the crowd with bounding boxes and a total count.

## Features

- Real-time crowd detection using YOLOv11
- Processes video files or live camera feed
- Draws bounding boxes around detected individuals
- Displays a unique count number for each detected person
- Shows total people count in the top left corner of the frame
- Adjustable confidence threshold for detections

## Preview
![image](https://github.com/user-attachments/assets/09086bc7-90e3-479c-81db-ace67cfccbbf)

![train_batch2](https://github.com/user-attachments/assets/a9f85346-7d05-493d-8632-70fe0a3d19f9)



## Requirements

- Python 3.11
- OpenCV (`cv2`)
- Ultralytics YOLO (`ultralytics`)
- cvzone

## Installation

1. Clone this repository:
   ```
   git clone [https://github.com/yashsuman15/crowd-detection.git](https://github.com/yashsuman15/crowd-density-model)
   cd crowd-detection
   ```

2. Install the required packages:
   ```
   pip install opencv-python ultralytics cvzone
   ```

3. Download the YOLOv11 weights file trained for crowd detection and place it in the `runs/kaggle/working/runs/detect/train/weights/` directory.

## Usage

1. Update the paths in the script:
   - Set the correct path for the YOLOv8 weights file
   - Set the correct path for the input video file, or use `0` for live camera feed

2. Run the script:
   ```
   python crowd-detection.py
   ```

3. The program will open a window showing the processed video with:
   - Bounding boxes around detected individuals
   - A unique count number for each detected person
   - Total people count in the top left corner
   Press 'q' to quit the application.

## Customization

- Adjust the `confidence` threshold in the script to fine-tune detection sensitivity (currently set to 0.3)
- Modify the colors of bounding boxes and text as needed
- Adjust the scale and thickness of the text for better visibility

## Important Notes

- This program is designed for crowd monitoring and analysis purposes.
- Ensure you comply with all local laws and regulations regarding privacy and surveillance when using this system.
- The accuracy of the detection depends on the quality of the trained model and input video.

## Contributing

Contributions to improve the project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## Acknowledgments

- [Ultralytics](https://github.com/ultralytics/ultralytics) for the YOLOv8 implementation
- [cvzone](https://github.com/cvzone/cvzone) for enhanced OpenCV utilities

## Disclaimer

This software is provided for educational and research purposes only. The authors and contributors are not responsible for any misuse or illegal use of this software. Users are solely responsible for ensuring their use of this software complies with all applicable laws and regulations, particularly those concerning privacy and data protection.
