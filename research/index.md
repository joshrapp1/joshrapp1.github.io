
# Single-Photon Lidar
## Robust Imaging in Strong Background Light
<img src="/images/unmixing.png" width="600">

We introduce a new approach to depth and reflectivity estimation that emphasizes 
the unmixing of contributions from signal and noise sources. At each pixel in an image,
short-duration range gates are adaptively determined and applied to remove detections 
likely to be due to noise. For pixels with too few detections to perform this censoring accurately,
data are combined from neighboring pixels to improve depth estimates, 
where the neighborhood formation is also adaptive to scene content.

## Dithered Depth Measurement
<img src="/images/dither.png" width="600">

Using detector arrays can speed up lidar systems by parallelizing acquisition. 
However, current SPAD arrays have time bins longer than typical laser pulse durations, 
resulting in measurement errors dom- inated by quantization. 
We propose an optical time-of-flight system that uses subtractive dither to improve image depth resolution. 
Additional modeling of the measurement noise with a generalized Gaussian distribution 
leads to more efficient order statistics-based estimators and rules of thumb for when subtractive dither is useful
and which estimator to apply.

## Dead Time Compensation
<img src="/images/deadtime.png" width="600">
