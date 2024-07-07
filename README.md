# InvoMark: Hidden Watermarking in Images using Python
# Overview

InvoMark is a Python-based project that implements a technique for embedding hidden watermarks in images. This method is widely used for purposes such as copyright protection, authentication, and security. The technique involves converting the image into an array of pixels, generating a watermark, applying a transform to the watermark, embedding the watermark into the original image by modifying the pixel values, and saving the watermarked image to a file.
## Featured 

- Convert images to arrays of pixels
- Generate and apply discrete cosine transform (DCT) to the watermark
- Embed the watermark into the original image by modifying the least significant bit (LSB) of the pixel values
- Extract and verify the watermark from the watermarked image
- Evaluate the performance of the technique on various test images
## Libraries Used
- NumPy: For numerical operations and array manipulations
- OpenCV: For image processing tasks
- Pillow: For handling and manipulating images
## Installation

1. Clone the repository:

```
git clone https://github.com/yourusername/invomark.git

```
2. Navigate to the project directory:

  ```
cd invomark

```
3. Install the required libraries:

```
pip install numpy opencv-python pillow
```
## Usage
1. Embedding a Watermark:

```
from invomark import embed_watermark

original_image_path = 'path/to/your/image.jpg'
watermark_text = 'Your Watermark'
watermarked_image_path = 'path/to/save/watermarked_image.jpg'

embed_watermark(original_image_path, watermark_text, watermarked_image_path)
```
2. Extracting a Watermark:
```
from invomark import extract_watermark

watermarked_image_path = 'path/to/your/watermarked_image.jpg'
original_watermark_text = 'Your Watermark'

watermark_present = extract_watermark(watermarked_image_path, original_watermark_text)

if watermark_present:
    print("The watermark is present and the image is authentic.")
else:
    print("The watermark is not present or the image has been tampered with.")
```
## Methodology
- Convert Image to Array: The original image is converted into an array of pixels using OpenCV.
- Generate Watermark: A watermark is generated, which can be a text or image.
- Apply Transform: The discrete cosine transform (DCT) is applied to the watermark.
- Embed Watermark: The watermark is embedded into the original image by modifying the least significant bit (LSB) of the pixel values.
- Save Watermarked Image: The watermarked image is saved to a file.
- Extract Watermark: The DCT transform is applied to the watermarked image and compared with the original watermark to determine if the image has been tampered with.
## Performance Evaluation
The performance of the proposed technique is evaluated on various test images. The results show that the embedded watermark is not easily visible and can only be detected using specific techniques. This provides a simple and efficient way of implementing hidden watermarking on an image using Python.
## Applications
- Copyright protection
- Authentication
- Security
## Contact 
For any questions or suggestions, feel free to open an issue or contact us at abhishektiwari182002@gmail.com
