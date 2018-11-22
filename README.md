# Zebrafish brain activity
This repository provides full-resolution TIFF files of zebrafish brain activity maps from the paper:

*Brain-wide circuit interrogation at the cellular level guided by online analysis of neuronal function.* [Vladimirov et al, Nat. Methods, 2018]().

The images were acquired using a custom light-sheet microscope (Zebrascope) and post-processed as described in the paper.

## Functional Maps
Functional maps of zebrafish brains during optomotor response behavior, prior to any ablations: 

Fish expressing GCaMP6f in neuronal **nuclei** (paper, Fig.1c, SI Video 1).
Folder `FunctionalMaps/nuc/` contains the following files:
  * [Functional map in RGB color code](FunctionalMaps/nuc/CompositeRGB-gamma0.5-w_range(0-1)-16bit-scaled.tif.zip). The regression-computed weights `w_i (i=1,2,3)` (swimming, forward stimulus, backward stimulus) were linearly scaled into 16-bit image intensities (0,1) -> (0, 65535) and combined into a 3-channel RGB TIFF stack (red, green, blue channel, respectively) (file size: 251 MB).
  * [Maximum intensity projection stack](FunctionalMaps/nuc/MIP_CompositeRGB-w_max0p46.tif) for quick overview of the functional activity (6 MB).
  * [Anatomy stack](FunctionalMaps/nuc/Anatomy-16bit-scaled.tif.zip), an average of 10 imaging stacks from the experiment (raw fluorescence, no post-processing), a 16-bit grayscale TIFF file (47 MB).


Fish expressing GCaMP6f in neuronal **cytosol** (paper, Fig.2a, SI Video 2).
Folder `FunctionalMaps/cyto/` contains the following files:
  * [Functional map in RGB color code](FunctionalMaps/cyto/CompositeRGB-gamma0.5-w_range(0-1)-16bit-scaled.tif.zip).
  * [Maximum intensity projection stack](FunctionalMaps/cyto/MIP-CompositeRGB-gamma0.5-w_max0.46.tif)
  * [Anatomy stack](FunctionalMaps/cyto/Anatomy-16bit-scaled.tif.zip)
 
## Ablation effects on brain activity 
Effect of brain region ablation on the relative fluorescence signal change `dF/F` across the brain (paper, Fig.2c-h). The `dF/F` change was computed relative to pre-ablation conditions. Before averaging across individuals, each fish brain was registered to a reference [Z-brain](http://engertlab.fas.harvard.edu/Z-Brain/#/home) atlas.

  * [ablation fc-RoL (reticulospinal region)](ablationEffects_dFF/C-ablation_RoL-dFFchange(magenta-green)-Zbrain(gray).tif.zip) 
  * [fc-nMLF (another reticulospinal region)](ablationEffects_dFF/D-ablation_nMLF-dFFchange(magenta-green)-Zbrain(gray).tif.zip)
  * [fc-preT ("pretectum")](ablationEffects_dFF/E-ablation_PreT-dFFchange(magenta-green)-Zbrain(gray).tif.zip)
  * [fc-IO ("inferior olive")](ablationEffects_dFF/F-ablation_IO-dFFchange(magenta-green)-Zbrain(gray).tif.zip)
  * [fc-DHB ("dorsal hindbrain")](ablationEffects_dFF/G-ablation_DHB-dFFchange(magenta-green)-Zbrain(gray).tif.zip)
  * [fc-RandOT ("random optic tectum")](ablationEffects_dFF/H-ablation_randOT-dFFchange(magenta-green)-Zbrain(gray).tif.zip)
(each file 26 MB)

## Screenshots 
### Maximum intensity projection of nuclear-expressing GCaMP6f fish:
![nuclear-expressing GCaMP6f fish (paper Fig.1c, SI Video 1)](/FunctionalMaps/nuc/MIP_CompositeRGB-w_max0p46-scale0.5.png "nuclear-expressing GCaMP6f")

### Maximum intensity projection of cytosol-expressing GCaMP6f fish:
![cytosol-expressing GCaMP6f fish (paper SI Video 2)](/FunctionalMaps/cyto/MIP-CompositeRGB-gamma0.5-w_max0.46-scale0.5.png "cytosol-expressing GCaMP6f")

### Maximum intensity projections of ablation effects:
![Ablation Effects in dF/F (Figure 2)](/ablationEffects_dFF/combined-dFFeffect-allAreas.png "ablation effects")

## File downloading
Files are versioned using [Git LFS](https://git-lfs.github.com/) system because of the size. The simplest way to download them is to click on each file and proceed through `Download` button, or clicking `View raw`. For automatic download of all files in the repository, install [Git LFS](https://git-lfs.github.com/) and clone the whole repo.

## Citation
If you use the data, please cite the original paper:

*Brain-wide circuit interrogation at the cellular level guided by online analysis of neuronal function.* [Vladimirov et al, Nat. Methods, 2018]().