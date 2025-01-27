import numpy as np
a = np.array([
    [100,200,150,300],
    [50,60,40,80],
    [300,400,350,500],
    [200,250,220,270],
    [80,90,70,100]
])
#1
a.shape
(5, 4)

#2
a.dtype
dtype('int32')

#3
a.size
20

#4
a.nbytes
80

#5
a+20
array([[120, 220, 170, 320],
       [ 70,  80,  60, 100],
       [320, 420, 370, 520],
       [220, 270, 240, 290],
       [100, 110,  90, 120]])

#6
a[2]-10
array([290, 390, 340, 490])

#7
a[:,1]*2
array([400, 120, 800, 500, 180])


#8
max_capacity = 1000
(a/ max_capacity) * 100
array([[10., 20., 15., 30.],
       [ 5.,  6.,  4.,  8.],
       [30., 40., 35., 50.],
       [20., 25., 22., 27.],
       [ 8.,  9.,  7., 10.]])

#10
np.sum(a,axis = 1)
array([ 750,  230, 1550,  940,  340])

#11
np.sum(a,axis = 0)
array([ 730, 1000,  830, 1250])

#12
np.max(a,axis = 0)
array([300, 400, 350, 500])

#13
np.min(a,axis = 1)
array([100,  40, 300, 200,  70])

#14
np.mean(a,axis = 1)
array([187.5,  57.5, 387.5, 235. ,  85. ])

#15
a[1]
array([50, 60, 40, 80])

#16
a[:,3]
array([300,  80, 500, 270, 100])

#17
a[0:3,0:2]
array([[100, 200],
       [ 50,  60],
       [300, 400]])

#18
stock = a[4,2]
print(stock)
70

#19
products = [0, 3]  
locations = [0, 2]  

stock_levels = a[products, locations]

print(stock_levels)
[100,220]

#20
a[1, 3] = 100  
print(a)
[[100 200 150 300]
 [ 50  60  40 100]
 [300 400 350 500]
 [200 250 220 270]
 [ 80  90  70 100]]
