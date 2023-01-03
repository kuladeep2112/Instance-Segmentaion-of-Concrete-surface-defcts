# Instance-Segmentaion-of-Concrete-surface-defects
**Data Acquisition:**

•	I collected 300 images from 1500 image data corpus of concrete bridges, dam’s dataset  https://doi.org/10.5281/zenodo.2620293.<br>
•	Above Dataset has only bounding box annotations but for the present task we need image masks to train segmentation models.<br>
•	I Performed Data Augmentations like shear, rotation, flip etc. to increase the dataset dimensions from 300 to 600.<br>
•	I used Roboflow annotations tool to create annotations in .txt format for yolov7 instance segmentation model.<br>
•	For U-Net model I created a helper function that takes in txt file and creates masks and store them in a separate folder with .png extension.<br>

**YoloV7 model training:**

•	We are considering pretrained model of yolov7 for instance segmentation and train for 50 epochs.<br>
•	Model achieved a mAP@ IOU=0.5 score as 0.310 <br>
•	Model accuracy can be further improved by using a greater number of input images for time being I used 300 we can annotate whole dataset of 1500 images.<br>

**U-net Multi Class segmentation:**

1) We trained U-net for 50 epochs to get segmentations on image.
2) We obtained best IOU score as 0.9643.
