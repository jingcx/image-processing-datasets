# image-processing-datasets

## Dehazing

> Waterloo IVC Dehazed Image Database

Kede Ma, Wentao Liu and Zhou Wang, "Perceptual evaluation of single image dehazing algorithms," IEEE International Conference on Image Processing, Sept. 2015

The dataset consists of 25 hazy images covering diverse outdoor scenes and indoor static objects. 22 images of outdoor scenes are captured in the real world and are degraded by haze to different extents, while the hazes of the other 3 indoor images are simulated homogenously. Then 8 dehazing algorithms proposed between 2009 and 2014 are selected to produce 8 different dehazed images for each of the 25 hazy images to form 25 image sets, each of which includes 9 images of the same content (1 hazy, 8 dehazed). In the subjective test, 24 subjects were showed 9 images of one image set at the same time on a display, and were asked to give scores according to perceptual qualities of these images.

> Vision enhancement in homogeneous and heterogeneous fog

FRIDA dataset designed for Advanced Driver Assistance Systems (ADAS) that is a synthetic image database (computer graphics generated scenes) with 66 roads synthesized scenes.

> D-hazy: A dataset to evaluate quantitatively dehazing algorithms

http://www.meo.etc.upt.ro/AncutiProjectPages/D_Hazzy_ICIP2016/ (dataset publicly available)

A dataset of 1400+ images of real complex scenes has been derived from the Middleburry1 and the NYU-Depth V22 datasets. It contains high quality real scenes, and the depth map associated to each image has been used to yield synthesized hazy images based on Koschmieder’s light propagation model.

> A color image database for haze model and dehazing methods evaluation

We created a database called CHIC (Color Hazy Image for Comparison), consisting of two scenes in controlled environment. In addition to the haze-free image, we provide 9 images of different fog densities. Moreover, for each scene, we provide a number of parameters such as local scene depth, distance from the camera of known objects such as Macbeth Color Checkers, their radiance, and the haze level through transmittance.

> HazeRD: an outdoor dataset for dehazing algorithms

https://ieee-dataport.org/documents/hazerd-outdoor-dataset-dehazing-algorithms

HazeRD contains 10 different scenes based on the architectural biometrics project. For each scene, the ground RGB images, depth maps, and synthesized hazy images following the atmospheric optics are provided; the hazy images come with five different haze level using real life physical parameters. HazeRD focuses on outdoor scenes whereas other datasets provide indoor scenes(?); and, the synthesis is based on real life parameters.

> I-HAZE: A DEHAZING BENCHMARK WITH REAL HAZY AND HAZE-FREE INDOOR IMAGES *(NTIRE18)*

Contains 35 image pairs of hazy and corresponding haze-free (ground-truth) indoor images. Hazy images have been generated
using real haze produced by two professional haze machines (LSM1500 PRO 1500 W). The images are captured in a controlled environment, both haze-free and hazy images are captured under the same illumination conditions.

Before shooting the hazy scene, we use a fan that helps to obtain in a relatively short period of time a homogenous haze distribution in the entire room (obviously that is kept isolated as much as possible by closing all the doors and windows).

Since each scene contains the color checker, the white-balance can be manually adjusted (a posteriori) using specialized software such as Adobe Photoshop Lightroom.

> O-HAZE: a dehazing benchmark with real hazy and haze-free outdoor images

We introduce the first outdoor scenes database (named O-HAZE) composed of pairs of real hazy and corresponding haze-free images. Hazy images have been captured in presence of real haze, generated by professional haze machines, and OHAZE contains 45 different outdoor scenes depicting the same visual content recorded in haze-free and hazy conditions, under the same illumination parameters.

Each scene acquisition has started with a manual adjustment of the camera settings. The same parameters are adopted to capture the haze-free and hazy scene. Those parameters include the shutter-speed (exposure-time), the aperture (F-stop), the ISO and white-balance. The similarity between hazy and haze-free acquisition settings is confirmed by the fact that the closer regions (that in general are less distorted by haze) have similar appearance (in terms of color and visibility) in the pair of hazy and haze-free images associated to a given scene.

To set the camera parameters (aperture-exposure-ISO), we took advantage of the built-in light-meter of the camera, but also used an external exponometer (Sekonic). For the custom white-balance, we used the middle gray card (18% gray) of the color checker. This commonly used process in photography is quite straight-forward and requires to change the camera white-balance mode in manual mode and place the reference grey-card in the front of it. For this step, we have placed the gray-card in the center of the scene in the range of four meters.

> RESIDE: A Benchmark for Single Image Dehazing

https://sites.google.com/view/reside-dehaze-datasets

RESIDE highlights diverse data sources and image contents, and is divided into five subsets, each serving different training or evaluation purposes. We further provide a rich variety of criteria for dehazing algorithm evaluation, ranging from full-reference metrics, to no-reference metrics, to subjective evaluation and the novel task-driven evaluation. 

The RESIDE testing set is uniquely composed of Synthetic Objective Testing Set (SOTS), annotated Real-world Task-driven Testing Set (RTTS), and Hybrid Subjective Testing Set (HSTS) which has 1;000, 4;332, and 20 hazy images correspondingly.

## Deblurring (sharpening)

> Understanding and evaluating blind deconvolution algorithms (CVPR 2009)

Constructs a dataset with four latent sharp images and eight uniform blur kernels, resulting in a total of 32 test images.

> Edge-based blur kernel estimation using patch priors

Extend the dataset(the above one) by using 80 high-resolution natural images of diverse scenes and synthetically blurring each one with the eight blur kernels.

>  Benchmarking blind deconvolution with a real-world database (ECCV 2012)

Records 6D camera trajectories over time, and play back the camera motion on a robotic platform to capture blurred images. This benchmark contains four latent images and 12 camera trajectories.

> A Comparative Study for Single Image Blind Deblurring (CVPR 2016)

http://vllab.ucmerced.edu/wlai24/cvpr16_deblur_study/

We construct two large datasets for evaluating image deblurring algorithms: (1) 100 real blurred images and (2) 200 synthetically blurred images with both uniform and non-uniform blur. Our real dataset contains real blurred images captured under different scenarios. Our synthetic dataset includes both uniform and non-uniform motion-blurred images.

Real images: All these blurred images are captured in the real-world scenarios from different cameras (e.g., consumer cameras, DSLR, or cellphone cameras), different settings (e.g., exposure time, aperture size, ISO), and different users. We categorize images according to the following five attributes: man-made, natural, people/face, saturated, and text.

Synthetic: To synthesize nonuniform blurred images, we record the 6D camera trajectories using a cellphone with inertial sensors (gyroscope and accelerometer), and construct a collection of spatially varying blur kernels by assuming constant depth for the scenes. We obtain the 100 non-uniform blurred images by applying four camera trajectories to 25 latent images and adding 1% Gaussian noise to simulate camera noise.

## De-rain

### rain streak removal

> Removing rain from a single image via discriminative sparse coding

http://ieeexplore.ieee.org/document/7410745/

The rain images for testing are synthesized by adding rainy effect on 200+ outdoor images randomly selected from the UCID dataset. The rainy effect is generated by two existing composite models: one is additive composite model and the other is screen blend model. The rain images are synthesized with rain streaks whose orientations varying from 70◦ to 110◦. Thus, we obtain two data sets for performance evaluation with one corresponding to additive composite model and one corresponding to screen blend model.

> Rain Streak Removal Using Layer Priors

Synthesize a new dataset with more images (12) using the photorealistic rendering techniques proposed by Grag and Shree. (Photorealistic rendering of rain streaks)

> Photorealistic rendering of rain streaks

http://www1.cs.columbia.edu/CAVE/projects/rain_ren/rain_ren.php (dataset publicly available)

> Automatic Single-Image-Based Rain Streaks Removal via Image Decomposition

Used photoshop to generate synthesized data: https://www.photoshopessentials.com/photo-effects/rain/

> Single Image Rain Streak Decomposition Using Layer Priors

https://ieeexplore.ieee.org/abstract/document/7934436/

dataset: http://yu-li.github.io/paper/li_cvpr16_rain.zip

### rain drop removal

> Attentive Generative Adversarial Network for Raindrop Removal from A Single Image (CVPR'2018)

https://github.com/rui1996/DeRaindrop (dataset publicly available)

Image pairs where each pair contains exactly the same background scene, yet one is degraded by raindrops and the other one is free from raindrops. Contains 1119 pairs of images (861 image pairs for training and 239 image pairs for testing), with various background scenes and raindrops. Sony A6000 and Canon EOS 60 for the image acquisition.

> Restoring an Image Taken through a Window Covered with Dirt or Rain (ICCV'2013)

http://openaccess.thecvf.com/content_iccv_2013/papers/Eigen_Restoring_an_Image_2013_ICCV_paper.pdf

Built by taking photographs of multiple scenes with and without the corruption present. For corrupt images, we simulated the effect of rain on a window by spraying water on a pane of anti-reflective MgF2-coated glass, taking care to produce drops that closely resemble real rain. To limit motion differences between clean and rainy shots, all scenes contained only static objects.
