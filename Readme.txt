I will explain my code by each block of jupyter notebook.
1-In 1st block i have import libraries 
2-In second block i have read images of task1 dataset.
3-In 3rd block i have resize all images of task1 dataset and convert into grey scale image.
4-In 4th block i have create a function of mouse right click that function will save my x and y axis of input image.
5-In 5th block i am recovering transformation using two images. First i take correspondence points of image 1 and image 2 using mouse click function. Then i used
thes points and convert into afine matrix after that i apply pseudo inverse and generate matrix. In warp affine i am passing matrix and image 2 in which i want to apply 
warping. it will generate Trandformed image. after that i find out mean square error between image 1 and transformed image using each pixel and correspondence.
6-In 6th block i apply recover transformation on mecca 2 task1 dataset.
7-In 7th block i apply recover transformation on station 2 task1 dataset.
8-In 8th block i read images of Task 2 for image registeration.
9-In 9th block same function of mouse click and compute image x and y axis and sorting function of x and y axis i have declared.
10-In 10th block i have create register image function in which i am reading two images and first i am getting width and heiht of both images
then i am taking points of both images using mouse click function image_points. after that i am creating two matrix of both points. After this step i am
creating matrix A and matrix b of projective transformation using 4 points.After applying formula i am generating matrix 3x3 and passing it into warp perspective function that is returning me
image after fitting exact location in base image. after that in next steps i am creating mask and combining both base image and transformed image that is returning me resultant image.
11-In 11th block i am applying this register image function on qlibold and qlib new image in task 2 dataset.
12-In 12th block i am applying this register image function on faisalMosque evening and faisal mosque night image in task 2 dataset.
13-In 13th block i am applying this register image function on test1 and test2 image in task 2 dataset.
14-In 14th block i am reading images of task 3 from task 3 dataset.
15-In 15th block i have created function of image stiching in which  am taking two images as input and applying sift detect and compute on both images that is returning me features and descriptor.
After that i am matching these point using knn and computing NNDR that is nearest neighbour distance. After that i am drawing these matches and applying RANSAC to find homography.using these point i am transforming these images and joining these two images.In returning function
i am returning sift point image, image match , line match and transformed image.
16-In 16th block i am applying on two images for stiching in task 3 set 1.
17-In 17th block i am applying on three images for stiching in task 3 set 2.
18-In 18th block i am applying on Four images for stiching in task 3 set 3.
19-In 19th block i am applying on Five images for stiching in task 3 set 3.
20-In 20th block i am applying on three images for stiching in task 3 set 4.
21-In 21st block i am applying on two images for stiching in task 3 set 5.
22-In 22nd block i am applying on four images for stiching in task 3 set 6.
