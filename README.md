# Replacing PC Screen in a Video

This project processes a video to detect **ArUco markers** and uses them as reference points to project a custom image onto a defined region (e.g., a monitor screen). The output is a video where the image is seamlessly integrated into the screen, maintaining the correct perspective.

---

## Features

- **Detect ArUco Markers**: Identifies markers placed in the corners of a monitor or any rectangular region.
- **Perspective Projection**: Calculates the transformation required to overlay an image onto the marked region.
- **Overlay Custom Images**: Replaces the screen content in the video with a custom image.
- **Dynamic Image Adaptation**: Any photo can be used as an overlay, and it will be automatically resized and adjusted to fit perfectly within the area defined by the ArUco markers.
- **Output Video**: Saves the processed video with the overlay applied.

---

## Process

1. ArUco markers are placed in the corners of a monitor or any desired rectangular region.
2. The video is processed frame by frame to detect these markers.
3. A custom image is dynamically resized and warped to match the perspective of the marker-defined region.
4. The processed frames are saved as a new video with the overlay seamlessly replacing the original screen content.

<img width="680" alt="Screenshot 2024-12-05 at 16 03 47" src="https://github.com/user-attachments/assets/eb276e4d-6609-4040-b78c-fcd4b1067865">
<img width="680" alt="Screenshot 2024-12-05 at 16 03 54" src="https://github.com/user-attachments/assets/20dd0f05-6bad-443c-9340-f6e30d99a8aa">
<img width="677" alt="Screenshot 2024-12-05 at 16 04 02" src="https://github.com/user-attachments/assets/7ae6fff1-3024-42bb-a39b-9a9a40df9376">
<img width="411" alt="Screenshot 2024-12-05 at 16 04 12" src="https://github.com/user-attachments/assets/6423959e-6ef0-49ba-9066-1a89163f2726">

Final output video in the Path (output.mp4)





---

### Required Libraries

The project requires the following libraries:
- `opencv-python`
- `opencv-contrib-python`
- `numpy`
- `matplotlib`
- `tqdm`

---

## Installation

### Install Libraries with `pip`

Run the following command to install the required libraries individually:
```bash
pip install -r requirements.txt



