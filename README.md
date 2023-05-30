# multi-label-classification
## Image processing and labeling
A public database was used, provided by Peking University through a global grand challenge named "International Competition on Ocular Disease Intelligent Recognition (ODIR)" (https://odir2019.grand-challenge.org).  This dataset collects fundus images from the left and right eyes of 5000 patients and diagnostic keywords from doctors at different hospitals and medical centers in China. Demographic data for each patient, including age and sex, is also provided in the dataset. Eight categories of disease labels are provided for each patient, which refer to normal, DR, glaucoma, cataract, AMD, hypertension, myopia, and other abnormal diseases/abnormalities.
Before the network training, we processed the fundus images in the ODIR database to confirm that the images were of sufficient quality for the experiment. Firstly, the study removed the poor-quality images for the left or right eye. According to the diagnostic keywords of the left eye and right eye, exclusion criteria for images followed some rules. A total of 2824 images were abandoned from the total of 10,000 fundus images in the ODIR database, leaving 7176 images. According to the diagnostic keywords of the left eye and right eye, eight categories of labels were assigned to each fundus image to reduce the complexity of network construction, which enabled the model to detect the fundus disease of an individual eye. After image processing and labeling, the remaining 7176 images were used for training and testing. Among these 7176 images, 966 fundus images from the off-site testing set were used as the testing set, and 6210 images remained. To achieve the goal of single label training and multi label prediction, the study only retained single label images from the training set, totaling 5571 images.In addition to the normal, DR, and other abnormal diseases of 4185 images, the other categories of 1386 images were only duplicated four or seven times to obtain 4675 images. The normal, DR, and other abnormal diseases of 4185 images integrating the augmented other categories of 4675 images resulted in 10246 fundus images for network training and validation with a ratio of 9:1, or 9221: 1025.

# Download:
public database: https://github.com/nkicsl/OIA;
model and code: 链接: https://pan.baidu.com/s/1uRmLmwbf5-N6J61cuZtg-w 提取码: dw5s
