## How to attach annotations to prepared images

### Provided datasets
**3D-location-size-developmental-cells.csv** --> Normalized location for all developmental cells (undifferentiation cells directly observed in the images).

**adult-developmental-cell-identity-mappings.csv** --> Provides a link between developmental cells and identities for adult cells (a differentiation identity for the observed developmental cells). Adult cells are also functionally annotated, so we know what their function and tissue contribution will be.

**developmental-cells-3D-normalized-position-divisions-size.csv** --> adult cell identities with number of divisions since the 1-cell stage (fertilization), normalized position, and size estimate (deviation from median size of mother cell, or the origin of the current cell identity). 

### Bounding Box method
All cells in the image can be defined by using a bounding box to delimit the size and location of the signal (contrast differences from background) in the provided images. A cluster of signal typically represents a single cell. Some of the images might be noisy (extraneous signal), so double-check images to ensure that the cell annotations make sense.

### Cell identity annotation
TBA

### Preprocessing images for annotation
Rotate images 90 degrees to the right, then use the center of the image as x=0, y=0. Coordinates listed in the provided datasets (.csv files) provide normalized coordinates (median values centered on 0). Find the center of a bounding box, and estimate its diplacement from the center. These values can then be compared with the x,y positions in the provided datsets and linked to the cell IDs, size estimates, and annotations.
