# Cell Tracking and Mitosis Detection
#### Coursework project for Computer Vision
![Cell%20Tracking%20and%20Mitosis%20Detection.png](https://github.com/melmarsezio/Computer-Vision/blob/master/Cell%20Tracking%20and%20Mitosis%20Detection.png) 
Three groups of microscopies with different acquisition techniques

Differential Interference Contrast (DIC) images, Fluorescent (Fluo) images, and Phase-contrast (PhC) images [from left to right] 
## Instruction
1. Run [*`Tophat_UltimateErosion_Watershed_Phc_Fluo.ipynb`*](https://github.com/melmarsezio/Computer-Vision/blob/master/Tophat_UltimateErosion_Watershed_Phc_Fluo.ipynb) to get the labels of original image for Fluo and PhC datasets. The labels will be saved as `.npy` file, it could take up to hours to label the entire dataset. Enviroment settings are as [*`requirements.txt`*](https://github.com/melmarsezio/Computer-Vision/blob/master/requirements.txt)
2. Run [*`MU-Lux-CZ`*](https://github.com/melmarsezio/Computer-Vision/tree/master/MU-Lux-CZ) U-Net model to obtain labels for DIC dataset. The labels will be saves as `.tif` image file. Enviroment settings are as [*`DL_requirements.txt`*](https://github.com/melmarsezio/Computer-Vision/blob/master/DL_requirements.txt)
2. Run [*`project_total.ipynb`*](https://github.com/melmarsezio/Computer-Vision/blob/master/project_total.ipynb) to generate output videos. [*`project_total.ipynb`*](https://github.com/melmarsezio/Computer-Vision/blob/master/project_total.ipynb) will try to read labels generated from first and second step, and base on the labels to track and detect mitosis. The trajectory history will also be saved as `.pkl` file for the purpose of motion analysis.
3. To get motion analysis information, manual inspect the cell coordinates (the key of trajectory stored in `.pkl` file) and pass the coordinate and trajectory to task3 function

## Report
The report of the experiment on the proposed method is discussed in [*`COMP9517 Report.pdf`*](https://github.com/melmarsezio/Computer-Vision/blob/master/COMP9517%20Report.pdf) in detail and properly referenced for any literature reviewed and cited
