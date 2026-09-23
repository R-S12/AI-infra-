# AI-infra-
结合AIInfraGuide教程学习的AI infra学习日志

2026.9.21
**第一章 变量对象引用**
**python变量名字绑定对象**
- 如图所示，此种写法a,b是指向同一个列表，所以更新是一起更新的。（a is b则是验证两变量是否指向同一个对象）
- 如果需要两变量指向对象不同，得b=a.copy()
- 对应浅拷贝copy.copy()指向同一地址、深拷贝copy.deepcopy()指向不同地址
<img width="1081" height="457" alt="image" src="https://github.com/user-attachments/assets/43b92529-fd35-45dd-a82c-2dea45610ed1" />
如图所示，在函数中**变量赋值≠修改变量**</br>
当修改变量append时，形参和实参指向同一个地址；当函数中的形参重新赋值时，形参和实参指向的就是不同地址
<img width="1117" height="416" alt="image" src="https://github.com/user-attachments/assets/1ed39a26-aace-440a-9add-117ded08c6cf" />
- 如图所示，第一个错误是因为每次调用函数都是指向同一个列表
- 第二个则是如果没有指定列表，那每次调用函数就是指向新的列表;如果有指定列表，那就在这个指定列表里进行更新
<img width="1121" height="547" alt="image" src="https://github.com/user-attachments/assets/4111e95b-849e-475d-9ca7-7cc443acf146" />
