# Gamma
十一周
opencv简单实践11：gamma矫正（手动实现）、直方图均衡（三通道）

练习1 实现gamma矫正
遍历所有像素，对所有像素进行进行如下运算
1.像素值归一化到[0,1]之间 2. 3. Intensity=Output*255

查表法
建立查询表数组Lut，size==256，遍历[0，255]
1.下标值归一化到[0,1]之间 2.  3. Lut[i]=Output*255
遍历所有像素，像素值作为下表，直接从Lut中读出变化后的像素值

练习2 直方图均衡
调用直方图均衡函数，进行直方图均衡处理，opencv原函数只能对单通道图像进
行直方图均衡，要求实现可以对3通道图像进行直方图均衡

练习3 
图中有一些字，由于曝光不足无法观察到，请使用gamma矫正，并设置合适参数，
找出隐藏的信息。

我的代码https://github.com/DawnYue/Gamma

老师代码https://github.com/lizhu1126/dip-class-demos/blob/feature11.enhanceHist/dip-class-demos/funtions.cpp#L187
