# Tumor Nuclei Segmentation and Classification

Nuclei segmentation and classification using hematoxylin and eosin-stained histology images is a challenging task due a variety of issues, such as color inconsistency resulting from non-uniform manual staining operations, clustering of nuclei and blurry and overlapping nuclei boundaries. Existing approaches involve segmenting nuclei by drawing their polygon representations or by measuring the distances between nuclei centroids. In contrast, we leverage the fact that morphological features (appearance, shape and texture) of nuclei vary greatly depending upon the tissue type on which it is located. We exploit this information by extracting tissue specific (TS) features from raw histopathology images using our tissue specific feature distillation (TSFD) backbone. Then our bi-directional feature pyramid network (BiFPN) generates a robust hierarchical feature pyramid using these TS features. Next, our interlinked decoders jointly optimize and fuse these features to generate final predictions. We also propose a novel loss combination for joint optimization and faster convergence of our proposed network. Extensive ablation studies are performed to validate the effectiveness of each component of TSFD-Net. TSFD- Net achieves state-of-the-art performance on PanNuke dataset having 19 different tissue types and up to 5 clinically important tumor classes. 


## Results

The Table below compare quantitative results of different models.


<!--![alt text](https://gitfront.io/r/talha/6869f722e912f647c023710f40c958495046fca9/TSFD/raw/screens/results.png)-->
![alt text](https://github.com/oliveira-mtcode/Tumor-Nuclei-Segmentation/blob/master/screens/results.png)

  
## Visual Results
The figure below shows some qualitative results.


<!--![alt text](https://gitfront.io/r/talha/6869f722e912f647c023710f40c958495046fca9/TSFD/raw/screens/img3.png)-->
![alt text](https://github.com/oliveira-mtcode/Tumor-Nuclei-Segmentation/blob/master/screens/img3.png)



