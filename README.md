# OpenCV Functions Repository

This repository contains a Jupyter Notebook with various functions implemented using OpenCV, a popular computer vision library. The functions included in this notebook allow you to perform operations such as cropping, resizing, warping, color change, video reading, photo reading, webcam usage, color detection, face detection, edge detection, drawing shapes, and adding text to images.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
  - [Crop](#crop)
  - [Resize](#resize)
  - [Warp](#warp)
  - [Color Change](#color-change)
  - [Video Reading](#video-reading)
  - [Photo Reading](#photo-reading)
  - [Webcam](#webcam)
  - [Color Detection](#color-detection)
  - [Face Detection](#face-detection)
  - [Edge Detection](#edge-detection)
  - [Drawing Shapes](#building-shapes)
  - [Adding Text](#adding-text)
- [Contributing](#contributing)
- [License](#license)

## Installation

To use the functions in this repository, you need to have OpenCV installed. You can install OpenCV using the following command:

```bash
pip install opencv-python
```

Make sure you have Jupyter Notebook installed as well. You can install it with the following command:

```bash
pip install jupyter
```

Clone this repository to your local machine:

```bash
git clone https://github.com/your-username/opencv-functions.git
```

## Usage

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open the `opencv_functions.ipynb` file in the Jupyter Notebook interface.

3. Run each cell in the notebook to execute the desired function. You can modify the input parameters as needed.

## Functions

### Crop

The `crop(image, x, y, width, height)` function allows you to crop a rectangular region from an image.

- `image`: The input image.
- `x`: The x-coordinate of the top-left corner of the region.
- `y`: The y-coordinate of the top-left corner of the region.
- `width`: The width of the region.
- `height`: The height of the region.

### Resize

The `resize(image, width, height)` function resizes an image to the specified width and height.

- `image`: The input image.
- `width`: The desired width of the output image.
- `height`: The desired height of the output image.

### Warp

The `warp(image, src_points, dst_points, output_size)` function applies a perspective transform (warp) to an image using the specified source and destination points.

- `image`: The input image.
- `src_points`: List of four source points specifying the region to be warped.
- `dst_points`: List of four destination points specifying the output region.
- `output_size`: Tuple specifying the width and height of the output image.

### Color Change

The `change_color(image, conversion_code)` function changes the color space of an image.

- `image`: The input image.
- `conversion_code`: The color space conversion code. For example, `cv2.COLOR_BGR2GRAY` for converting to grayscale.

### Video Reading

The `read_video(video_path)` function reads a video file and displays it frame by frame.

- `video_path`: The path to the input video file.

### Photo Reading

The `read_photo(image_path)` function reads and displays an image file.

- `image_path`: The path to the input image

 file.

### Webcam

The `read_webcam()` function captures video from the webcam and displays it frame by frame.

### Color Detection

The `detect_color(image, lower_range, upper_range)` function detects objects in an image based on a specified color range.

- `image`: The input image.
- `lower_range`: The lower range of the color to detect.
- `upper_range`: The upper range of the color to detect.

### Face Detection

The `detect_faces(image)` function detects faces in an image using Haar cascades.

- `image`: The input image.

### Edge Detection

The `detect_edges(image, threshold1, threshold2)` function applies edge detection to an image using the Canny edge detection algorithm.

- `image`: The input image.
- `threshold1`: The lower threshold value for the hysteresis procedure.
- `threshold2`: The upper threshold value for the hysteresis procedure.

### Drawing Shapes

The `draw_shape(image, shape, parameters)` function allows you to draw different shapes on an image.

- `image`: The input image.
- `shape`: Specifies the shape to be drawn. Options include "rectangle", "circle", "line", and "polygon".
- `parameters`: A dictionary of parameters specific to the chosen shape. For example, for a rectangle, you would provide parameters such as `top_left`, `bottom_right`, and `color`.

### Adding Text

The `add_text(image, text, position, font, font_scale, color, thickness)` function allows you to add text to an image.

- `image`: The input image.
- `text`: The text string to be added.
- `position`: The position of the text in the image specified as a tuple (x, y).
- `font`: The font type of the text.
- `font_scale`: The scale factor for the font size.
- `color`: The color of the text.
- `thickness`: The thickness of the text.

## Contributing

If you would like to contribute to this repository, feel free to open issues or submit pull requests. Any contributions to improve existing functions or add new ones are welcome!

## License

This repository is licensed under the [MIT License](LICENSE). Feel free to use the code provided in this repository for your own projects.
