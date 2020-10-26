# Violence Detection From Videos Captured By CCTV
What if a computer will tell you about the presence of violence in a live stream of CCTV video without any interference of human? Yes! It is possible with the help of Deep Learning.

Video is nothing but the sequence of images, and image is nothing but the three-dimensional array. To process video data we need good computation power and well-performing algorithms. We are giving live prediction hence our system should work very fast. All this thing was not possible in the pre-Deep Learning era.

After tremendous growth in Deep Learning algorithms and after the invention of GPU, nowadays Deep Learning is a very popular tool. There are algorithms present that can easily and effectively process video data to get the desired result.

This is a binary classification problem, I am going to build a Deep Learning architecture, which will get trained on pre-collected CCTV violent and nonviolent data. For inference, I will pass live CCTV footage collected for some duration of time and will get a prediction of violence. In this way, we will get the prediction of violence without the visualization of violence.

## Data information:
To design a system that works well in the actual field, data should fulfill the following criteria.

- You should have a sufficient amount of data to train the model.
- Videos you are using for training that should be actual CCTV footage, it should not videos taken from movies or some mobile recorded video.
- Train and validation data should split carefully, there should not be any data leakage problem.
I have taken data from this link. 
 https://github.com/mchengny/RWF2000-Video-Database-for-Violence-Detection/blob/master/README.md

Once you reached the GitHub account, you will see data is not directly available. You have to fill an agreement shit they have provided. After that, you have to send mail on provided mail id with attaching filled agreement sheet. Once you did this they will get back to you with data downloading link.

They have collected raw surveillance videos from YouTube, sliced them into clips within 5s at 30 fps, and labeled each clip as Violent or Non-Violent Behavior.

In this data set, there are 2000 videos given,1000 for violence, and 1000 for non-violence, data is balanced. They have already split data in train and validation, 1600 video in a train, and 400 in validation. You should have to use this data as given because they have split it very carefully. If you mix train and validation then it could create a data leakage problem.

## Understanding file sequence:
1. cs2_EDA.ipynb ==> This file contained all EDA and data visualization.
2. cs2_modeling.ipynb ==> Here you will get model architecture and all methods I have tried. While running this notebook you might need the all_logs_and_models.zip file, it contains all logs and models weights.
3. cs2_analysis.ipynb ==> I did false prediction analysis here.
4. final.ipynb ==> Inference part I have done in this notebook. There is a file final.zip it contains all necessary files for inference. 
5. I have added 3 videos which are the result I got with 3 inference methods.

#### If you have not come here from my blog, then visit the following link. There I have explained everything in detail. It will definitely help to work on this problem.
https://medium.com/@ravinadable16/violence-detection-from-videos-captured-by-cctv-d032a254d489
