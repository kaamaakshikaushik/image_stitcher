# Image Tile Stitching Project

This Python project splits a panorama image into overlapping tiles and then stitches them back together.

## What It Does

Takes a panorama image, splits it into 4 tiles with 40% overlap, then reconstructs the original image using alpha blending.

## Requirements

opencv-python
numpy
matplotlib


Install with: `pip install -r requirements.txt`

## How to Run

### In Google Colab
1. Upload your panorama image
2. Run the notebook cells
3. Check the output folder for results


## Output

The program creates:
- Individual tile images (tile_1.jpg through tile_4.jpg)
- Stitched result (stitched_result.jpg)
- Comparison visualization (comparison.png)

## How It Works

1. Split: Divides the image into overlapping tiles
2. Blend: Uses alpha blending to merge overlapping regions
3. Reconstruct: Combines tiles back into the full panorama

The overlap ensures smooth transitions between tiles without visible seams.

## Files

- `image_stitcher.ipynb` - Main notebook with the implementation
- `requirements.txt` - Python dependencies
- `README.md` - This file
-  'panoroma.jpg' - In Data Folder

## Notes

- Works best with wide panorama images
- Default is 4 horizontal tiles with 40% overlap
- Can adjust overlap percentage and number of tiles in the code
