# InvoMark: Hidden Watermarking in Images using Python
# Overview
InvoMark is a Python-based project that implements a technique for embedding hidden watermarks in images. This method is widely used for purposes such as copyright protection, authentication, and security. The technique involves converting the image into an array of pixels, generating a watermark, applying a transform to the watermark, embedding the watermark into the original image by modifying the pixel values, and saving the watermarked image to a file.
# Features
• Convert images to arrays of pixels
• Generate and apply discrete cosine transform (DCT) to the watermark
• Embed the watermark into the original image by modifying the least significant bit (LSB) of the pixel values
• Extract and verify the watermark from the watermarked image
• Evaluate the performance of the technique on various test images
# Libraries Used
• NumPy: For numerical operations and array manipulations
• OpenCV: For image processing tasks
• Pillow: For handling and manipulating images
# Installation
1.Clone the repository:
'''git clone https://github.com/yourusername/invomark.git'''

