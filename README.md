Prerequisites:

Grounded Segment Anything - https://github.com/IDEA-Research/Grounded-Segment-Anything.git
IP Adapter - https://github.com/tencent-ailab/IP-Adapter


Instructions:
1. Install both Submodules
2. Move all contents of `GroundingDINO` and `segment-anything` from `Grounded-Segment-Anything` to root dir
3. Run `generate_masks.ipynb`. Set the following values as needed:
   `image_path_foreground` - path to image to tack on
   `image_path_background` - path to image being tacked on with new item
   `foreground_prompt` - prompt for segmenting the image in the foreground
   `background_prompt` - prompt for segmenting the image in the background
   `output_dir` - output directory
4. Run `try_on.ipynb`