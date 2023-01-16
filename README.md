# yolo-v4-handgun-detection

We built a weapon detection model using the YOLO V4 Algorithm and were trained over the dataset of gun images that we collected. The model can detect handguns in real-time precisely. By creating the YOLO V4 weapon detection model, we propose to replace the existing surveillance systems that use slow object detection algorithms to our model. These replacements ensure that the people that use these surveillance systems will feel an improvement in monitoring performance so that they can respond to unwanted situations faster than before.

## Results

![image](https://user-images.githubusercontent.com/62060147/212740260-8c633b75-5d7f-4ed5-ad52-87cffc5ed55b.png)

A YOLO V3 model was created to serve as a benchmark for the proposed model. Both models were trained and tested using the same amount of images from the same datasets. The two models were compared, and based on the table above, the V4 model performs better than the V3 model.

![image](https://user-images.githubusercontent.com/62060147/212740397-48ef6489-d7f7-4b0a-ab10-5accae141830.png)

Table above shows that the proposed model, which uses the yolov4 framework, has obtained an average mAP of 94.045 %, which outperformed the benchmark model, which has only obtained a 90.617 % mAP. The dataset is divided into two data sources: the Google Images and the Test dataset. We performed Stratified K-fold validation in each dataset, and the results are plugged in the test of significance. To perform the test of significance, we have used the paired two-tailed T-test. Based on the results of the test, it indicates that the proposed model is statistically significant from the benchmark model with a p-value of 0.01323 and a significance level of 0.05.

## Sample Test

![image](https://user-images.githubusercontent.com/62060147/212739878-bf165a97-1545-445d-a993-9c0df194514d.png)

![image](https://user-images.githubusercontent.com/62060147/212740079-9d2fc723-e546-4be3-ad80-f6d8f1367ebe.png)

## Dataset
The image dataset containing guns was gathered from the Kaggle website. The dataset is split into train and test datasets, which have gun/s with different orientations and exposure, as shown in Figure 1. The training dataset contains 3000 images. The researchers split the dataset into 70% training and 30% testing.

![image](https://user-images.githubusercontent.com/62060147/212739093-1fee42f4-7a44-401e-81dc-442876c4a3a2.png)
