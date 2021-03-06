Training tiny-yolo-v2 on heart scans to detect left ventricles. 
**Take a look at the [WIKI](https://github.com/ell-hol/training-yolo-heart/wiki)**.

![alt text](https://github.com/ell-hol/training-yolo-heart/blob/master/Results/final_preprocessing_result.PNG)




Decompressed data is in png format. For each training image there's a corresponding mask segmenting the heart (left ventricle in grey, right ventricle in white) from the rest:


![alt text](https://github.com/ell-hol/training-yolo-heart/blob/master/Results/001.png)

The jupyter notebook script preprocessing.ipynb filters out the white area...

![alt text](https://github.com/ell-hol/training-yolo-heart/blob/master/Results/002.png)

...Leaving only the region of interest (left ventricle) and then generates the appropriate BoundingBox :

![alt text](https://github.com/ell-hol/training-yolo-heart/blob/master/Results/final_result.png)

All Bounding boxes corresponding to each training image are saved in [one .csv file](https://github.com/ell-hol/training-yolo-heart/blob/master/data/labels_bbox.csv)

