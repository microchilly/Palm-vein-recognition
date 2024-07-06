# PalmprintRecognition
采用两级级联神经网络进行关键点预测，提取ROI后进行图像处理，再利用Resnet和Efficientnet进行迁移学习的训练，测试和预测
# 模块如下
`extraROI.py`：初始的图像处理函数

`key_point_positioning.py`： 两级神经网络级联检测训练

`testphoto.py`：预测图像的特征点，进行输出

`proROI.py`：高级的图像处理函数，采用两级神经网络级联检测获取特征点，输出图像处理后的图像

`DataLoad_Twoinputs.py`：数据集加载和数据集处理函数

`model.py`：Resnet和EfficientNet模型的修改，构建，用于进行迁移学习
`Train`：对模型进行训练

`testmodel`：对模型进行测试

`predict.py`：对图像进行预测

`mainUI.py`：用pyqt5构建界面，集成训练，测试，预测，图像处理的功能
