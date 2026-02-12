## Project 1 – Brain Tumor Segmentation (Otsu vs Sauvola)

### Dataset

- **Dataset Name:** BRISC 2025 – Brain MRI Tumor Dataset  
- **Source:** https://www.kaggle.com/datasets/briscdataset/brisc2025  
- **Task:** Binary Brain Tumor Segmentation  


### Evaluation
- Dice Coefficient  
- Jaccard Index (IoU)


### Methods

- Otsu Thresholding - Global threshold selection

- Sauvola Thresholding - Local adaptive thresholding


### Results

| Method   | Dice Score | Jaccard Score |
|----------|------------|---------------|
| Otsu     | 0.098      | 0.053         |
| Sauvola  | 0.069      | 0.037         |


### Insights

- Otsu performed slightly better than Sauvola.
- Both methods produced very low accuracy.
- Tumor regions occupy a very small portion of the image.
- MRI images contain noise.
- Adaptive thresholding (Sauvola) over-segments edges and produces noisy masks.



### Conclusion

This shows that these processing techniques are not sufficient for accurate brain tumor segmentation.  
