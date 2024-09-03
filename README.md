# Image-Segmentation

  ## 1. Download the Dataset.  
 
• dataset used: 
http://www.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/BSR/BSR_bsds500.tgz 

• Reading images & ground truth 
 
  ## 2. Visualize the image and the ground truth segmentation. 
 
• Plotting actual picture with its ground truth

  ## 3. Segmentation using K-means 
 
• K-Means Clustering 
• Segmentations as Colored Images 
▪ Check this [Google Drive link]([url](https://drive.google.com/drive/folders/1unBvbmhuKVGbSCnSKSvmiF_SD5zH5ZhW)) for all the output images we got from our K-means 
clustering. Also, here’s a sample of the first two images and the resulted segmentation.
![image](https://github.com/user-attachments/assets/3bce7f24-94c1-4378-aa22-d1295fe09d04)
• Evaluation 
  ▪ we generate a list for each cluster containing the indices of the pixels that belong to that cluster. We also do the same for the ground truth segmentation that we are going to compare with.
  ▪ All the evaluation results can be found in the excel sheets in the repo
  ## 4. Big Picture 
 
• Ground truth vs K-means. 
  ▪ Printing every picture into google drive after clustering using the K-means function for every K = {3,5,7,9,11}. 
  ▪ Selected a set of five images and displayed their corresponding ground truth against our segmentation using K-means at K = 5.
  ![image](https://github.com/user-attachments/assets/19ab9a48-747e-4eee-93c7-385728e8607b)

• Ground truth vs Normalized-cut. 
  ▪ Implemented our own Normalized-cut function and applied it to the selected set of five pictures for 5-nn graph at K = 5. 
  ▪ Displayed their corresponding ground truth against our segmentation. 
  ![image](https://github.com/user-attachments/assets/aca094f1-f779-4451-ac90-593851b53ab0)

• K-means vs Normalized-Cut 
  ▪ Displayed our segmentation using k-means at K=5 vs Normalized-cut t for the 5 NN graph, at K=5. 
  ![image](https://github.com/user-attachments/assets/88c4731a-ae09-487f-913c-adaee5c7d9c6)

  ## 5. Extra

• Added a new column to the images array with each pixel’s distance from a reference point, which is (0,0). This resulted in significantly better F-measure and conditional entropy evaluation results.
  The following plots show how much the results change, where the red color is for the results with the new spatial layout.
  ![image](https://github.com/user-attachments/assets/ecfb9aa1-ca4b-4bab-bc10-ac238802a817)

