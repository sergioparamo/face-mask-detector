
# Face Mask Detector

This project uses a **deep learning model** with [OpenCV](https://opencv.org/) to detect whether individuals are wearing masks. The detection output highlights mask-wearing individuals with a green box and those not wearing a mask with a red box.


## Project Components

- **Dataset**: Contains images of people wearing masks and those not wearing them, used for training the model.
- **train_mask_detector.py**: Python script for training the mask detection model using the dataset.
- **detect_mask_video.py**: Python script for detecting mask-wearing status via webcam in real-time and save cropped faces.
- **mask_detector.model**: The trained model file (generated after training).
- **requirements.txt**: Lists the necessary libraries for the project.
- **plot.png**: A plot illustrating the training process, showing loss and accuracy.
- **cropped_faces**: Folder to store images of people not wearing masks, automatically populated by running `detect_mask_video.py`.
- **face-detector-demo.mp4**: Demo video showing the mask detection in action.

## Installation

1. Clone this repository or download the files.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. **Train the model**:
   Run the following command to train the mask detection model:
   ```bash
   python train_mask_detector.py
   ```
   Training takes approximately 20 minutes.

4. **Run the detection script**:
   Once the model is trained, you can run the webcam detection using:
   ```bash
   python detect_mask_video.py
   ```

   The webcam will activate, and the system will display whether individuals are wearing a mask. If someone is detected without a mask, their image will be saved in the `cropped_faces` folder.

## Prerequisites

- Anaconda (for managing dependencies)
- PyCharm (optional, for IDE usage)
- A webcam for real-time detection
- Python (intermediate knowledge required)

## Usage

- **Train the model**: Run `train_mask_detector.py` to train on the provided dataset.
- **Real-time detection**: Execute `detect_mask_video.py` to use the model for live detection through your webcam.

---

Enjoy using the Face Mask Detector! For any issues or contributions, feel free to open an issue or pull request.
