// edit by +n 2024/06/30==========
//面特徵先計算光達深度值，先檢查window內的x的深度為是否類似，再檢查y的梯度相同，y軸也相同方法。
//最後剩餘點再用高斯模糊後的影像作強度的比較，高斯模糊的window分別為21*41與41*21的大小。
//線特徵則是利用sobel算法找出邊緣，再進行點雲曲率的匹配。

//以下為kitti data的誤差值
sequence		
0	1.257	0.0066
1	2.5345	0.0047
2	1.5174	0.005
3	1.1189	0.006
4	1.3262	0.0039
5	0.8161	0.0035
6	0.6415	0.0034
7	0.8293	0.008
8	1.2255	0.0044
9	1.1479	0.0037
10	1.3751	0.0066
Avg	1.253581818	0.005072727273