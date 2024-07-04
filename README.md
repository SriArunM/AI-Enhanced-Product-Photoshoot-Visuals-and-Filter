# AI-Enhanced Product Photoshoot Visuals and Filter
## Overview
This project aims to develop an AI solution to enhance e-commerce product presentation by generating stunning product photoshoot visuals and implementing a filter to identify specific products within a given list of objects. The solution leverages Grounding DINO, YOLO models for zero-shot object detection, SAM model for segmentation and masking, and Stable Diffusion (inpainting) for generating visually appealing images.

## Key Objectives

### Generative AI for Visuals:
Use Stable Diffusion (inpainting) to create realistic and visually appealing product photoshoot visuals.
Simulate various lighting conditions, backgrounds, and angles commonly used in product photography.

### Product Recognition Filter:
Utilize Grounding DINO and YOLO models for zero-shot object detection to identify specific products within images.
Enhance identified product features while maintaining overall image integrity using the SAM model for segmentation and masking.

### Exclusion of Non-Relevant Images:
Implement a mechanism to filter out images that do not contain any of the specified products, ensuring that only relevant visuals are processed and enhanced.

## Code

### AutoDetect_Segment_StableDiffusion_Filter.ipynb
Use YOLO_world model with Efficient SAM and stable diffusion to implement the three key objectives of the project.
GenAI visuals-To create image based on the prompt along with various lightning,background and angle.
Product Recognition Filter -To recognise the products in the image,segment and enhance the segmented regions
Batch Filter-To Filter the image datasets which doesn't has the mentioned objects in the problem statement.

### AI_Enhanced_Product_Photoshoot.ipynb 
Combination of the above three key features as a single end product with Grounding DINO model instead of YOLO_world
The flow is to detect the specified objects in the problem statement,segment,create mask,invert the mask and then fed the masked image into the inpainting model along with original image.It creates visuals in the image apart from the masked area.These masked area represents the specified object in the problem statement.

## Usage

Clone the repo
```bash
  !git clone https://github.com/SriArunM/AI-Enhanced-Product-Photoshoot-Visuals-and-Filter
```
Run the .ipynb files 

## Results




