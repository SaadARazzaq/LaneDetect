# Lane Detection in Images and Videos

This repository contains Python code to detect lane lines in images and videos using OpenCV and Python. Lane detection is a critical component in many autonomous vehicle systems and can be applied in various other domains where understanding lane positioning is important.

## Requirements

- Python 3.x
- OpenCV (`pip install opencv-python`)
- NumPy (`pip install numpy`)
- Matplotlib (`pip install matplotlib`)

## Installation

1. Clone the repository:
2. Install dependencies:
```sh
pip install -r requirements.txt
```

## Usage

To detect lanes in image or a video, first run:
```sh
python lanes.py
```

Then Select from the main menu you want to detect lanes from the image or the video

The program will use `test_video.mp4` as input. It will display the processed video with lane lines overlaid in real-time. Press 'q' to exit the video playback.

## How It Works

1. **Image Processing:**
   - Converts the image to grayscale and applies Gaussian blur.
   - Detects edges using Canny edge detection.

2. **Region of Interest:**
   - Defines a polygonal mask to isolate the region where lane lines are expected.

3. **Hough Transform:**
   - Applies Hough Transform to detect line segments in the region of interest.

4. **Lane Detection:**
   - Groups and averages detected line segments to determine left and right lane lines.
   - Draws these averaged lines on the original image/video frame.

5. **Display:**
   - Combines the lane lines with the original image/video using weighted addition to visualize the detected lanes.

## Output Screenshots

![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/a0534252-273c-41cb-a876-8adff493eca3)
![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/2df86e39-d8d5-49fd-ad48-ecdd55663114)
![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/aba5fa08-0ff2-4e21-9d05-717336b28bc2)

![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/a0534252-273c-41cb-a876-8adff493eca3)
![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/632ec91e-375f-49ce-b844-91409db64503)
![image](https://github.com/SaadARazzaq/LaneDetect/assets/123338307/60ae8bc3-5f39-4538-8005-23f9672352a9)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
