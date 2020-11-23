# spsstereo
 Efficient Joint Segmentation, Occlusion Labeling, Stereo and Flow Estimation by Koichiro Yamaguchi, David McAlleste, Raquel Urtasun
 
## SPS-Stereo: Slanted Plane Smoothing Stereo

SPS-Stereo is a dense stereo method employing a slanted plane model. It jointly estimates a superpixel segmentation, boundary labels (such as occlusion boundaries), and a dense depth estimate from a pair of stereo images.

**Citation**  

    @inproceedings{Yamaguchi14,
    author = {Koichiro Yamaguchi and David McAllester and Raquel Urtasun},
    title = {Efficient Joint Segmentation, Occlusion Labeling, Stereo and Flow Estimation},
    booktitle = {ECCV},
    year = {2014}
    }


### Building SPS-Stereo

1. Prerequisites
    * sudo apt install libpng++-dev
2. Building
    1. type 'cmake .'
    2. type 'make'


### Usage of demo code

First, download KITTI stereo/flow dataset from [KITTI Vision Benchmark Suite homepage](http://www.cvlibs.net/datasets/kitti/eval_stereo_flow.php?benchmark=stereo) and extract it.

Run SPS-Stereo  
`> ./spsstereo left_image_1.png right_image_1.png
	
**Outputs**  

* `disparity.png`  
Disparity image (PNG 16bit grayscale format)  
(Disparity value) = (Pixel value)/256.0

### License
SPS-Stereo is licensed under the GNU General Public License Version 3 (GPLv3), see [http://www.gnu.org/licenses/gpl.html](http://www.gnu.org/licenses/gpl.html).
