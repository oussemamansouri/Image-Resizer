# Image Resizer

This Python script uses TensorFlow and OpenCV to resize images in a given folder and save the resized images to another folder.

## Requirements

Before running the script, make sure you have the following libraries installed:

*   TensorFlow: `tensorflow`
*   OpenCV: `opencv-python`
*   NumPy: `numpy`

You can install these libraries using pip:

```Bash
pip install tensorflow opencv-python numpy
```

## Installation

1.  Clone the repository (or download the script directly):

```Bash
git clone https://github.com/oussemamansouri/Image-Resizer
cd Image_Resizer 
```

2.  (Optional) Create a virtual environment (recommended):

```Bash
python3 -m venv .venv  # Create a virtual environment
source .venv/bin/activate  # Activate the virtual environment (Linux/macOS)
.venv\Scripts\activate  # Activate the virtual environment (Windows)
```

3.  Install the required packages (if you haven't already):

```Bash
pip install -r requirements.txt 
```

## Usage

1.  **Prepare your input folder:** Place the images you want to resize in a folder. Update the `input_folder` variable in the script to point to this directory.

2.  **Specify the output folder:** The resized images will be saved in the folder specified by the `output_folder` variable. This folder will be created if it doesn't exist.

3.  **Set the desired dimensions:** Modify the `width` and `height` variables to the desired dimensions for the resized images.

4.  **Run the script:**

## Script Details

The `resize_images` function takes the following arguments:

*   `input_folder`: Path to the folder containing the images to resize.
*   `output_folder`: Path to the folder where the resized images will be saved.
*   `width`: Desired width of the resized images.
*   `height`: Desired height of the resized images.

The script iterates through all image files (PNG, JPG, JPEG) in the input folder, resizes them using TensorFlow's `tf.image.resize` function, and saves the resized images to the output folder using OpenCV's `cv2.imwrite` function. It provides progress updates during the resizing process.
