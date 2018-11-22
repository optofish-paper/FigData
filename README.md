# Processed light-sheet data of zebrafish brain activity

## FunctionalMaps (Figure 1c)
Functional maps of zebrafish brains during optomotor response behavior: 

`/nuc`, nuclear-expressing GCaMP6f fish (paper Fig.1c, SI Video 1)

`/cyto`, cytosol-expressing GCaMP6f fish (paper SI Video 2)

Folders contain the following files:
  * Functional maps in RGB representation: `CompositeRGB-gamma0.5-w_range(0-1)-16bit-scaled.tif.zip`. The regression-computed weights `w_i (i=1,2,3)` (swimming, forward stimulus, backward stimulus) were linearly scaled into 16-bit image intensities (0,1) -> (0, 65535) and combined in a 3-channel 16-bit RGB TIFF stack (size: 251 MB).
  * Anatomy stacks: `Anatomy-16bit-scaled.tif.zip`, made of raw imaging stacks averaged over 20 time points, saved as 16-bit grayscale TIFF stack (size: 47 MB).
  * Maximum intensity projection stacks: `MIP_...tif`, for low-dimensional representation of the files above.

## Ablation Effects in dF/F (Figure 2)
**(a)**, exemplary functional map of an individual fish, in RGB TIFF stack. Color code: red for swimming activity, green for forward stimulus motion, blue for backward stimulus motion.

**(c-h)** effect of regions ablation on the `dF/F` signal across the fish brains. The `dF/F` change was computed relative to pre-ablation conditions (magenta for elevation, green for decrease). Before averaging, individual fish brains were registered to a reference [Z-brain](http://engertlab.fas.harvard.edu/Z-Brain/#/home) atlas, colored in gray.

## File downloading
Files are stored using [Git LFS](https://git-lfs.github.com/) system because of size. The simplest way to download them is to click on each file and proceed through `Download` button, or `View raw` link ([example](https://github.com/optofish-paper/FigData/blob/master/Fig2D/nuc/MIP_CompositeRGB-w_max0p46.tif)). For automatic download of all files in the repository, install [Git LFS](https://git-lfs.github.com/) and clone the repo.

## Screenshots (maximum intensity projections)
![nuclear-expressing GCaMP6f fish (paper Fig.1c, SI Video 1)](/functionalMaps/nuc/MIP_CompositeRGB-w_max0p46-scale0.5.tif)

![cytosol-expressing GCaMP6f fish (paper SI Video 2)](/functionalMaps/cyto/MIP-CompositeRGB-gamma0.5-w_max0.46-scale0.5.tif)

![]()

![]()