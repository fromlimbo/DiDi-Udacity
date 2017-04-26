# DiDi-Udacity
3D point cloud detection 

Discussion: https://discussions.udacity.com/t/put-your-starter-code-here/234860
Dataset:http://www.semantic3d.net/

Part1:https://medium.com/@hengcherkeng/part-1-didi-udacity-challenge-2017-car-and-pedestrian-detection-using-lidar-and-rgb-fff616fc63e8 

Part2:https://medium.com/@hengcherkeng/part-2-didi-udacity-challenge-2017-car-and-pedestrian-detection-using-lidar-and-rgb-bb8e28f6d987 

Part3:https://medium.com/@hengcherkeng/part-3-didi-udacity-challenge-2017-car-and-pedestrian-detection-using-lidar-and-rgb-e86490774ec6 

Part4a:https://medium.com/@hengcherkeng/part-4-didi-udacity-challenge-2017-car-and-pedestrian-detection-using-lidar-and-rgb-6f6a964b94b5 

Part4b:https://medium.com/@hengcherkeng/part-4b-didi-udacity-challenge-2017-car-and-pedestrian-detection-using-lidar-and-rgb-9f8b910562fc


4.25: 下载了源码，尝试按照Anaconda下虚拟环境运行tensorflow的方法。具体按照 https://github.com/hengck23/didi-udacity-2017/issues/1 中zdx3578给的步骤来。但是有一些要注意到：

      1）在tensorflow虚拟环境下，opencv3.2.0 的python库名称为cv2.cpython-35m-x86_64-linux-gnu.so,所以要用cv2.so软链接一下
           才能用import cv2
      
      2）设置了cuda的lib路径后要source一下，否则会链接不到
      
      3）修改了一下作者的data.py和train.py里的一系列原始路径
      
      4）make.sh里面的TF_INC的路径改成了tensorflow虚拟环境下的路径
      ~/anaconda3/envs/tensorflow/lib/python3.5/site-packages/tensorflow/include/
        
      5）重新生成roi_pooling层的时候把make.sh里面的psroi_pooling的内容注释掉了
      
      6）运行python3 train.py的时候注意要开启tensorflow虚拟环境
      
      
