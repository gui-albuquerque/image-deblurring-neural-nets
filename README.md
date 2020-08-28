# image-deblurring-neural-nets
Several architectures of neural networks used for image deblurring (more especifically CNNs, GANs and a proposed mixture of experts).

## 256colors: 
Experiments over images with 256 gradations of color (B&W or RGB).

## 8colors: 
Experiments over images with 8 gradations of gray (only B&W).

## mixture_of_experts:
Proposed mixture of trained CNNs for the restoration of images with 256 gradations of gray (only B&W).

### Degradation of the images used:
The degradation of the images was simulated by a gaussian point spread function (that have sigma and the dimension of the filter as parameters -- with higher values for sigma and broader dimensions for the filter, worse the degradation).

### Measure of similarity between images (SSIM Index):
The SSIM index was used to measure the similarity between the restoratios achieved and the original images without degradation. The SSIM index is contained in the interval $[-1, 1]$ and returns 1 when both images are identical. This index takes in account characteriscs from the human visual system (see [https://ece.uwaterloo.ca/~z70wang/publications/ssim.pdf]).
