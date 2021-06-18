# 静态手势识别
深度学习课设
一共识别5种手势动作
1. 剪刀动作  2.石头动作 3.布动作  4.OK动作  5.good动作

项目文件列表如下：
1. `data`：存放训练集、测试集，实时保存的图像（用于在线检测）。
2. `ges_ico`：存放UI窗口使用的各种图标。
3. `log`：存放训练的CNN网络的模型参数。
4. `CallFrame.py`：界面窗口的逻辑文件，用来调用界面文件并编写信号与槽函数。
5. `Frame.py`：界面窗口的界面文件，通过PyQt5的designer工具生成。
6. `GetTestImage.py`：利用OpenCV获取图片并标记，用来制作测试集。
7. `GetTrainImage.py`：利用OpenCV获取图片并标记，用来制作训练集。
8. `SaveGesture.py`：利用OpenCV实时获取图片，并进行预处理，用于在线检测手势。
9. `TestGesture.py`：将实时获取的图片送入已训练好的CNN中判断其手势动作。
10. `TestInTest.py`：将测试集送入已训练好的CNN中判断该网络模型的准确率。
11. `Train.py`：训练CNN模型函数，并将训练好的模型参数保存在本地。
12. `Train_inputdata.py`：用来读取数据集的图像和标签，并打包成batch形式。
13. `Train_model.py`：模型结构，采用AlexNet结构。

环境要求如下：
1. Python3.7
2. numpy1.20.1
3. OpenCV3.4.5.20
4. scikit-learn 0.20.2
5. TensorFlow 1.15.0
