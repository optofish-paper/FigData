# Processed light-sheet used in Figures

## Figure 2D
Functional maps of zebrafish brains: 

`/nuc`, nuclear-expressing GCaMP6f fish (manuscript Fig.2D, left)

`/cyto`, cytosol-expressing GCaMP6f fish (manuscript Fig.2D, right)

Folders contain the following files:
  * Functional maps in RGB representation: `CompositeRGB-gamma0.5-w_range(0-1)-16bit-scaled.tif.zip`. The regression coefficients $w_i (i=1,2,3) $ were linearly scaled into 16-bit image intensities (0,1) -> (0, 65535) and combined in a 3-channel 16-bit TIFF file (size: 251 MB).
  * Anatomy stacks: `Anatomy-16bit-scaled.tif.zip`, made of raw imaging stacks averaged over 20 time points, saved as 16-bit grayscale TIFF file (47 MB).
  * Maximum intensity projection stacks: `MIP_...tif`, for low-dimensional representation of the files above.


