Prerequisites:

Grounded Segment Anything - https://github.com/IDEA-Research/Grounded-Segment-Anything.git
IP Adapter - https://github.com/tencent-ailab/IP-Adapter
Development machine runs on `cpu`, so a local version of IP-Adapter with `dtype=float16` removed was needed


Instructions:
1. Install deps in `requirements.txt`
2. Install Submodules (`gsa` and `ipadapter`)
3. Move `generate_masks` to the `gsa` dir
4. Run `generate_masks.ipynb`. Set the following values as needed:
   `image_path_foreground` - path to image to tack on
   `image_path_background` - path to image being tacked on with new item
   `foreground_prompt` - prompt for segmenting the image in the foreground
   `background_prompt` - prompt for segmenting the image in the background
   `output_dir` - output directory
5. Run `try_on.ipynb`. Set input values appropriately