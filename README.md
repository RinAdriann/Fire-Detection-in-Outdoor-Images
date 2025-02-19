# Fire-Detection-in-Outdoor-Images

This was a project for the Digital Image Processing course, focuing on the detection of wildfires.

## Team Members
1. Rindra Adriansyah      [Created the model and notebook]
2. Rakai Andaru Priandra  [Created the report]
3. Bagus Aryajatmiko      [Created the report]
4. Dzaki Dzikril Hakim    [Literature review and created the report]
   
## Dataset
These were dataset used on this project,
Training [1000 images]: NASA Space Apps Challenge Fire Dataset [https://www.kaggle.com/datasets/phylake1337/fire-dataset]
Testing [380 images]: A. Khan and B. Hassan, "Dataset for Forest Fire Detection," Version 1 [https://doi.org/10.17632/gjmr63rz2r.1]

We utilized an SVM model with the process below,

## Pre-Process
1. Implemented an improved otsu thresholding using a weighted scheme by by Hui-Fuang Ng, Cheng-Wai Kheng and Jim-Min Lin in 2015
2. Applied color-based segmentation using HSV classification on top of the otsu
## Feature Extraction
1. Extracted the color moments and the shannon entropy of the images (highlighting the differences between fire and non-fire images)
## Modelling
1. Split the dataset into 80:20 for training and testing
2. Used an SVM Classifier model with only the 'linear' kernel as parameter
3. Did not utilize any hyperparameter tuning
## Evaluation and Results
1. Achieved 97% F1 Accuracy on average with 98% on fire and 94% on non-fire (training and testing)
2. Achieved 96% of mean cross validation score (used 5 folds)
3. Achieved 90% F1 Accuracy on average with 90% on fire and 89% on non-fire (unseen data)

## References
[1] NASA Space Apps Challenge Fire Dataset. (2018). Kaggle. Fire Dataset. [Online]. Available: https://www.kaggle.com/datasets/phylake1337/fire-dataset
[2] A. Khan and B. Hassan, "Dataset for Forest Fire Detection," Version 1, 27 Aug. 2020. [Online]. Available: https://doi.org/10.17632/gjmr63rz2r.1
[3] M. Jamali, N. Karimi, and S. Samavi, "Saliency based fire detection using texture and color features," in Proc. IEEE Int. Conf. on Electrical Engineering (ICEE), 2020, pp. 1-5, doi: 10.1109/ICEE50131.2020.9260659.
[4] H. F. Ng, "A weighting scheme for improving Otsu method for threshold selections," J. Comput. (Taiwan), vol. 27, pp. 12-21, 2016.
[5] A. Gidudu, G. Hulley, and T. Marwala, "Classification of images using support vector machines," 2007.
[6] S. M. T. Mohammed, M. F. N. M. Sap, and R. B. Arshad, "Fire detection system using support vector machine and image segmentation," Proceedings of the 2016 International Conference on Computer and Communication Engineering, pp. 48-52, 2016.
[7] F. A. A. M. Zainal, S. B. R. Abdullah, and K. J. Lim, "Real-time fire detection using color segmentation and SVM," IEEE Transactions on Industrial Electronics, vol. 60, no. 7, pp. 2539-2546, 2017.
[8] Kukuk, S. B., and Z. H. Kilimci. "Comprehensive analysis of forest fire detection using deep learning models and conventional machine learning algorithms." International Journal of Computational and Experimental Science and Engineering, 2021. 
[9] S. M. T. Mohammed, M. F. N. M. Sap, and R. B. Arshad, "Fire detection system using support vector machine and image segmentation," Proceedings of the 2016 International Conference on Computer and Communication Engineering, pp. 48-52, 2016.
[10] S. G. Manogaran and R. P. S. Chithra, "A novel fire detection method in video surveillance using color segmentation and support vector machine," Journal of Electrical Engineering & Technology, vol. 11, no. 3, pp. 932-938, 2016.
