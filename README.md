# **Horses and Humans Classifier**

This project will use Convolution Neural Network (CNN) to classify or determine determine what makes a horse a horse and a human a human

## **Convolution**

A convolution is simply a filter of weights that are used to multiply a pixel with its neighbors to get a new value for the pixel.

![alt text](img/image.png)
*Figure 1: Ankle boot with convolution.*

Look at the pixel in the middle of the selection, we can see that it has a value of 192 with a filter in the same 3 x 3 grid, as shown below the original values $\rightarrow$ transform that pixel by calculating a new value by multiplying the current value of each pixel in the grid by the value in the same position in the filter grid, and summing up the total amount. This total will be the new value for the current pixel and repeat this for all pixels in the image.

So in this case, while the current value of the pixel in the center of the selection is 192, the new value after applying the filter will be:
$$newvalue = (-1 * 0) + (0 * 64) + (-2 * 129) + (0.5 * 48) + (4.5 * 192) +.... = 577$$
