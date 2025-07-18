# Gamma Encoding and Decoding

## Instructions

1. Open an image (Use standard Lena image), convert it to grayscale, and plot both the original and grayscale image using subplots.

2. Write a function to implement gamma encoding to simulate how camera sensor encodes the original scene before storage. The function should take 2 arguments: image, gamma value.

3. Pass the image and the gamma value = 2.2 to the function to encode the image.
   [Recall from the class that we use 1/gamma to encode, and gamma to decode]

4. Decode the encoded image with gamma value = 2.2.

5. Plot the images and histogram of the original image, encoded image and the decoded image.

6. Repeat the above steps but with different gamma values while decoding. Use these values:
   - Gamma while encoding = 2.2
   - Gamma while decoding = 1.0, 1.8, 2.2, 4.0

7. Plot 4 different graphs (for 4 different decode operations with above values).
   - X-axis should mean "Scene Luminance", Y-axis should mean "Perceived Brightness".
   - Each individual graph should consist of following 3 curves/lines:
     i. Blue curve = Encode operation during storage
     ii. Red curve = Decode operation if applied to the original scene (without encoding)
     iii. Green curve = Decode operation applied to the encoded scene (Captures the overall effect after Gamma encoding and decoding)
