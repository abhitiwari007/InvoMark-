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
