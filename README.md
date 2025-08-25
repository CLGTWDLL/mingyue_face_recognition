重庆大学24级明月科创实验班线性代数课程项目。人脸识别部分使用了PCA和SVM，PCA部分使用了小矩阵技巧和大矩阵特征向量转换以提高准确率。  
在此感谢 [@icebear-yy](https://github.com/icebear-yy)对svm模块的贡献。他调出来的SVM模型非常好用，在项目测试时的实时识别部分发挥了巨大作用  
同时感谢[@bravezmz](https://github.com/bravezmz)对APP页面的设计，没有他就没有这么有艺术性的APP页面  
操作说明：1，使用前下载MATLAB Support Package for USB Webcams工具箱，否则无法正常使用摄像头  
2，更改路径（在代码视图中修改回调函数）  
3，作者原本的测试集和训练集和训练SVM模型的数据均采用的是班里同学的人脸，为了保护他们的隐私，本仓库里的测试集和训练集是从网上下载的  
使用前需要做的：
1.将图片中的路径改为自己的路径用来存放经过APP第一页图像处理部分处理后的文件
<img width="717" height="230" alt="image" src="https://github.com/user-attachments/assets/edd55a1f-195b-47d4-82ac-e6b9d3956389" />  
2.将图片中的路径改为自己下载下来后的自己的“创意小功能图片”的路径
<img width="981" height="344" alt="image" src="https://github.com/user-attachments/assets/185e5920-68cb-42bc-a771-7ad90886be36" />  
3.图中的音乐创意小功能中要用，请将图片中的路径改为自己下载下来后的自己的“音乐文件”的路径（该部分和上一张图片里的都在同一个回调下）
<img width="902" height="285" alt="image" src="https://github.com/user-attachments/assets/b695d3ce-e789-4fd0-8885-a0eabe65842c" />  
4.在这里将训练svm要用到的训练集换成自己训练集的地址（模型训练的部分在app中有）注意，此处的训练集应该是被一个大文件夹存储的。代码的回调写的是读取文件夹下的文件夹
<img width="1055" height="305" alt="image" src="https://github.com/user-attachments/assets/2d5c85e4-9495-4005-99e8-b9ded435420f" />  
<img width="1880" height="997" alt="image" src="https://github.com/user-attachments/assets/f21b7622-b7d7-4b48-a8ad-70f91107ab57" />

一，操作演示（图像处理）
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/a91068c6-8d53-4613-b258-fdc1fe03d992" />
第一步，点“打开文件”，选择一张图片文件
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/6a127041-7a7e-4dae-922a-c2fa266d3d8a" />
第二步，图片加载到页面后点击按钮就可以操作
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/b08e659f-a347-42d6-9cad-a955b400cc6e" />
效果预览，其余的也是如此
二，操作演示（PCA）
先拖动“贡献率”滑块使得贡献率达到85%及以上
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/f828de69-1134-4569-bcc9-970a01760820" />
然后点击“启动PCA”，先选择训练集
<img width="1907" height="979" alt="image" src="https://github.com/user-attachments/assets/68a5fe0a-4d3d-4034-b069-b8417ce67f31" />
等待一段时间，当APP页面出现“平均脸”时，再在弹窗中选择自己的测试集
<img width="1906" height="976" alt="image" src="https://github.com/user-attachments/assets/72d651c2-4623-4565-a4f0-537c5150b016" />
然后APP会自动把测试集的人脸和训练集的人脸匹配并显示在APP中，效果如图
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/d2cb946f-8fe1-4762-b61c-b0bf6d58443a" />
操作演示（摄像头）
点击“启动摄像头”，然后从弹窗中选择自己的训练好的SVM模型，这里推荐选线性核，选好后摄像头会自动启动并开始人脸识别。
<img width="1920" height="976" alt="image" src="https://github.com/user-attachments/assets/0c0b41fc-142a-4e47-b3e1-652a0d53793d" />
演示图片里的SVM模型是作者用同学们的数据训练的，为了保护隐私同样也没有上传。需要的同学可以自己从APP中自带的模型训练页面用自己的训练集训练新的模型
三，操作演示（PCA过程）
此处是为了展示PCA训练的流程而设计的，按序号依次点击APP页面的按钮
<img width="1904" height="967" alt="image" src="https://github.com/user-attachments/assets/8790af48-028f-46cd-a54d-091bc311675b" />
训练完毕后会弹出如图所示的弹窗，点击“确定”
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/c462bc8b-bfd7-41e9-a528-451b40ff7f8e" />
然后点击第二个按钮，选择刚刚训练完得到的变量
<img width="1920" height="981" alt="image" src="https://github.com/user-attachments/assets/ff59ddee-d608-43a8-bff8-e61f7232ba75" />
训练完毕后会弹出如图所示的弹窗，点击“确定”
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/d602c67e-91db-4c05-81c9-61d5e9878d46" />
以此类推，点击第三个按钮时选择第二次训练完得到的变量，点击第四个按钮时选择第三次训练完得到的变量，最终会以弹窗的形式展示人脸识别的结果
四，操作演示（SVM训练）
先点击自己的核（这里以线性核作为演示）
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/bf950535-1496-461b-abc2-e43f96cafe9f" />
点击完毕后依次输入参数（此处的参数仅作为演示，不保证可靠性）
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/5483c291-a5ea-4116-977f-20936e2f8f56" />
输入完毕后点击“训练模型并保存”，点击后耐心等待
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/3eee182e-a782-47f0-bbd5-eda88ea87473" />
出现如下变化和弹窗说明训练完成
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/adec2da3-dfff-4b0c-8c01-fa2b641eba32" />
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/16ffb55a-52a9-45b0-9a8d-1406b150463a" />
训练得到SVM模型会默认存储在该app所在的文件夹下，此模型可用于摄像头实时识别
<img width="1285" height="584" alt="image" src="https://github.com/user-attachments/assets/8709c523-0337-4597-824b-63823379faaa" />
五，操作演示（创意小功能）
点击“加载文件”
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/9f6c1502-6797-43de-a373-29574ac0c9ce" />
选择一张图片，点击“打开”
<img width="1902" height="994" alt="image" src="https://github.com/user-attachments/assets/49c5cb91-e6aa-4808-9ca3-0c979dd54551" />
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/42ec9a3f-18d4-4dad-ad3c-408879b235c8" />
在“想说的”处输入文本
<img width="1502" height="989" alt="image" src="https://github.com/user-attachments/assets/d8f0a520-df6d-4827-a206-2a7b6b36cf29" />
随后再点击“创意小功能”，会有好玩的事情发生




























