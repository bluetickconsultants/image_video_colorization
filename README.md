<div align="center">
  <img src="https://user-images.githubusercontent.com/88481845/215695216-7627029c-0257-44fb-83c3-73fd7ae84555.png">
</div>

<hr>

# Image and Video colorization using Deep learning and OpenCV 

Converting color images to black and white is quite easy using the OpenCV framework,but for converting black and white images to color we need to take a different approach. We need to add colors to black and white pixels using Deep Learning Neural Networks. Let’s first look at how the color information is represented in gray scale images and digital images.

Gray scale image means the value of each pixel represents only the intensity information of the light. Such images commonly display only the darkest black to the brightest white. The image carries only black, white, and gray colors, in which gray has multiple levels.Each pixel typically consists of 8 bits(1byte) for gray scale images and there are 256 possible grayscale colors.

Color images have three different channels called RGB. Each pixel intensity was represented by three channels. Each color image has 24 bits/pixel, which means 8 bits for each of the three color bands(RGB).There are 16 million colors possible. 

<table>
  <tbody>
    <tr>
      <td>
        <img src="https://user-images.githubusercontent.com/88481845/215695590-17d2366f-4a22-4278-89e4-441e8dac1e31.png">
      </td>
      <td>
      <img src="https://user-images.githubusercontent.com/88481845/215695598-878a8879-1510-488d-88f9-e55491b67c0c.png">
      </td>
    </tr>
  </tbody>
</table>

# Black and White Image to Color Image

We trained a neural network which converts this grayscale image to the colored one. It needs to learn to map this single value to a three channel image. For this purpose we used a concept called LAB space where we figured out the lightness scale of each pixel and mapped them correspondent A and B channels. 

<img src="https://user-images.githubusercontent.com/88481845/215697061-abd60059-32d3-4a32-840b-03d90533d258.jpg" width="25%">

LAB color space

Lab is an another color space same like RGB where
L channel = Lightness
A channel = from green-red
B channel = from Yellow-blue 

# Technologies used

● Neural Networks
● Open CV
● Tensorflow
● Statistics for Normalization

For this purpose we used a pre-trained neural network which was already trained on Imagenet grayscale dataset.It uses a simple convolutional neural network architecture. As explained above, we take the L channel image and learn to predict a and b channels. Combining the prediction and input would give us the colorized image which looks like a Lab color space image. 

![4](https://user-images.githubusercontent.com/88481845/215697305-eb3c7e38-6f8a-4b54-ab85-581a74a11abd.jpg)

After collecting pretrained weights and using tensorflow and opencv we convert predicted lab space images into RGB format.Hence the Neural network trained on 1000 different greyscale images we got 91.29 % accuracy for our results. 

# Outputs

<table>
  <tbody>
    <tr>
      <td>
        <video src="https://user-images.githubusercontent.com/88481845/215699989-66ad471b-e037-4779-83a9-b0955ea5f31c.mp4">
      </td>
      <td>
      <video src="https://user-images.githubusercontent.com/88481845/215700022-0694d538-dd1e-4526-b285-03a2b8dd8407.mp4">
      </td>
    </tr>
    <tr>
      <td>
        <video src="https://user-images.githubusercontent.com/88481845/215701613-d1770007-1d85-4488-ac03-f804970a82e4.mp4">
      </td>
      <td>
      <video src="https://user-images.githubusercontent.com/88481845/215701789-a2e3632f-5514-47c0-b6da-36bc1143ee9f.mp4">
      </td>
    </tr>
    <tr>
      <td>
        <video src="https://user-images.githubusercontent.com/88481845/215702122-a8fd4d65-7f42-4b01-a9a5-98b2973c7211.mp4">
      </td>
      <td>
      <video src="https://user-images.githubusercontent.com/88481845/215702561-75ba04d3-abb8-4f79-851a-51d17d1190c8.mp4">
      </td>
    </tr>
    <tr>
      <td>
        <video src="https://user-images.githubusercontent.com/88481845/215703014-6e17de9a-0f6f-464c-a5b3-5d37f6a284b1.mp4">
      </td>
      <td>
      <video src="https://user-images.githubusercontent.com/88481845/215703307-03f740e1-9d67-4c12-8e70-a5b4288736a4.mp4">
      </td>
    </tr>
  </tbody>
</table>


## Useful Information

### References
- [Image and Video colorization using Deep learning and OpenCV ](https://www.bluetickconsultants.com/image-and-video-colorization-using-deep-learning-and-openCV.html)

## Author

- [Bluetick Consultants LLP](https://www.bluetickconsultants.com/)
<img src="https://user-images.githubusercontent.com/88481845/215745914-16aa10a5-f24b-4fa9-b1be-432454487788.png" width="50%">




































