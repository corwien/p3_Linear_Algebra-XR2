# p3_Linear_Algebra-XR2
完成了填空和第一次更改

线性代数：修正之第二版

大致修改要点：
- 逆的证明，迹运算的证明
-plot绘制直线
- 范数的计算
- 求逆：np.linalg.inv
- 奇异值分解的原理

------------
仍不太明白：
＃第一处：
＃1.1.2 TODO
th1 = plt.text（l1 [0]，l1 [1]，'y = 2 * x + 1'，fontsize = 16，
               rotation = angle1，rotation_mode ='anchor'）
math.degrees（math.atan（2））直线上文字的旋转角度有点奇怪，如果atan（1）就可以刚好贴上线

＃第二处
最后运行的结果所代表的含义我没用看懂
＃请在U，d，V变量完成的情况下调用此测试程序，不要修改此处
plt.figure（figsize =（16,6））
for i，topk in enumerate（[5,10,15,20,30,50]）：
    reconstimg = np.matrix（U [：，topk]）* np.diag（D [：topk]）* np.matrix（VT [：topk，：]）
    plt.subplot（231 + I）
    plt.imshow（reconstimg，cmap ='gray'）
    title =“n =％s”％（（i + 1）* 5）
    plt.title（标题）
plt.show（）
