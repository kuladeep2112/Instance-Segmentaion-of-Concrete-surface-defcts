# Instance-Segmentaion-of-Concrete-surface-defects
** Data Acquisition:**

•	I collected 300 images from 1500 image data corpus of concrete bridges, dam’s dataset  https://doi.org/10.5281/zenodo.2620293.
•	Above Dataset has only bounding box annotations but for the present task we need image masks to train segmentation models.
•	I Performed Data Augmentations like shear, rotation, flip etc. to increase the dataset dimensions from 300 to 600.
•	I used Roboflow annotations tool to create annotations in .txt format for yolov7 instance segmentation model.
•	For U-Net model I created a helper function that takes in txt file and creates masks and store them in a separate folder with .png extension.
![image](https://user-images.githubusercontent.com/85028576/210315243-4ed9cc1d-f792-434a-afba-53a0dee29003.png)
