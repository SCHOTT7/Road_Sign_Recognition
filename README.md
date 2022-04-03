# Traffic Sign Recognition

## The DataSet

We used a dataset from Kaggle available at this link : *https://www.kaggle.com/datasets/shanmukh05/traffic-sign-cropped*

In this dataset we find a total of 27 000 train images and 12 630 test images. Images are cropped and converted to .jpg format.

There is a total of 43 classes, which means that we have 43 different traffic signs: 

![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00002.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00008.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00018.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00019.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00024.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00025.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00026.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00027.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00000_00028.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00001_00000.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00001_00006.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00001_00007.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00001_00012.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00001_00020.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00002_00013.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00002_00024.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00002_00027.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00003_00007.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00003_00021.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00003_00023.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00003_00026.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00004.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00025.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00026.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00027.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00028.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00004_00029.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00005_00019.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00005_00020.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00005_00023.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00005_00025.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00006_00000.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00006_00024.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00006_00029.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00007_00009.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00007_00021.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00008_00001.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00008_00027.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00008_00028.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00008_00029.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00010_00024.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00010_00025.jpg?raw=true)
![img_example](https://github.com/SCHOTT7/Road_Sign_Recognition/blob/main/Signs_Classes/00024_00028.jpg?raw=true)


## The implementation 

To speed up the training process and allow the use of GPU, we ran this project of Google Collab. 

We used Pytorch to design our model and our datasets class

We tried different model trying different number of hidden layers, different hidden layers's width and different convolution net. 

The following results were obtain with 20 fully connected hidden layers of size 150. We added as activation, the Tahn function at each node, and used the dropout feature with a value of 0.5 
Here's the detail of the convolotion net and the neural net:

```{python}
SignClassification(
  (c1): Sequential(
    (0): Conv2d(3, 5, kernel_size=(2, 2), stride=(1, 1), padding=(1, 1))
    (1): BatchNorm2d(5, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
    (2): ReLU()
    (3): AvgPool2d(kernel_size=2, stride=1, padding=1)
  )
  (c3): Sequential(
    (0): Conv2d(5, 10, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
    (1): BatchNorm2d(10, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
    (2): ReLU()
    (3): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
  )
  (c5): Sequential(
    (0): Conv2d(10, 28, kernel_size=(2, 2), stride=(1, 1))
    (1): BatchNorm2d(28, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
    (2): ReLU()
  )
  (c7): Sequential(
    (0): Conv2d(4, 7, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1))
    (1): BatchNorm2d(7, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
    (2): ReLU()
    (3): MaxPool2d(kernel_size=2, stride=1, padding=0, dilation=1, ceil_mode=False)
  )
  (layers): Sequential(
    (0): Linear(in_features=1372, out_features=60, bias=True)
    (1): ReLU()
    (2): Linear(in_features=60, out_features=60, bias=True)
    (3): ReLU()
    (4): Linear(in_features=60, out_features=60, bias=True)
    (5): ReLU()
    (6): Linear(in_features=60, out_features=60, bias=True)
    (7): ReLU()
    (8): Dropout(p=0.3, inplace=False)
    (9): Linear(in_features=60, out_features=60, bias=True)
    (10): ReLU()
    (11): Linear(in_features=60, out_features=43, bias=True)
  )
)
```
