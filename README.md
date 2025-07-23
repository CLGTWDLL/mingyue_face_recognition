<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/da4f16b1-ceb0-4c2e-ae9a-c230ab754375" /># mingyue_face_recognition
重庆大学24级明月科创实验班线性代数课程项目。人脸识别部分使用了PCA和SVM，PCA部分使用了小矩阵技巧和大矩阵特征向量转换以提高准确率。
操作说明：1，使用前下载MATLAB Support Package for USB Webcams工具箱，否则无法正常使用摄像头
2，更改路径（在代码视图中修改回调函数）
<img width="717" height="230" alt="image" src="https://github.com/user-attachments/assets/edd55a1f-195b-47d4-82ac-e6b9d3956389" />
将图片中的路径改为自己的路径用来存放经过处理后的文件
<img width="981" height="344" alt="image" src="https://github.com/user-attachments/assets/185e5920-68cb-42bc-a771-7ad90886be36" />
将图片中的路径改为自己下载下来后的自己的“创意小功能图片”的路径
<img width="902" height="285" alt="image" src="https://github.com/user-attachments/assets/b695d3ce-e789-4fd0-8885-a0eabe65842c" />
图中的音乐创意小功能中要用，请将图片中的路径改为自己下载下来后的自己的“音乐文件”的路径（该部分和上一张图片里的都在同一个回调下）
<img width="909" height="177" alt="image" src="https://github.com/user-attachments/assets/ed473642-efbc-401f-b72c-38dd4ecdf81c" />
在这里将svm要用到的模型换成自己训练的模型的地址（模型训练的部分在app中有）
3，操作演示（图像处理）
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/a91068c6-8d53-4613-b258-fdc1fe03d992" />
第一步，点“打开文件”，选择一张图片文件
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/6a127041-7a7e-4dae-922a-c2fa266d3d8a" />
第二步，图片加载到页面后点击按钮就可以操作
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/b08e659f-a347-42d6-9cad-a955b400cc6e" />
效果预览，其余的也是如此
4，操作演示（PCA）
点击“启动PCA”，然后选择自己的“train”（训练集文件）
<img width="1757" height="997" alt="image" src="https://github.com/user-attachments/assets/8506fa6b-751b-4445-95fd-803961b652cb" />
当完成对训练集的计算，得到平均脸时，会再次弹出弹窗，此时点击自己的“test”（测试集文件）
<img width="1756" height="992" alt="image" src="https://github.com/user-attachments/assets/1467ed73-02b5-4a04-b1fa-eda7c5cafffb" />






