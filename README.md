# Introductory-teaching
kaggle 上手小教程
最近在看黄佳的《零基础学机器学习》，入门时讲到kaggle的使用，我试着随着佳哥的教程走一遍，奈何上来导入文件这一块就出了不少错。
####先演示一下错误示范及其原因：
![image](https://github.com/0-0-1y/Introductory-teaching/assets/91407389/491e3588-b153-4b6e-bd91-1b92dab7a609)
可以发现它报错说时URL有问题，我又缝缝补补改改换换也没能解决URL有误的问题。
后面又从左上角的File上的uplode中输入这段URL然后发现确实能上传这个CSV资源到当前的Notebook上。
![image](https://github.com/0-0-1y/Introductory-teaching/assets/91407389/affbb3b4-c7b0-4a30-bef2-e864b7b771e1)
不过当我运行代码时发现还是无法运行，报错原因同上。
翻阅了kaggle官方文档后发现原来是我上载了文件后，在Notebook中读取文件要使用上载后的文件路径，再用url也没用，而上载后文件的url可以通过界面右侧的input获取，在input中找到我们要在程序中要使用的文件，双击它，在页面下方就会显示这个文件在当前Notebook中的文件路径：
![image](https://github.com/0-0-1y/Introductory-teaching/assets/91407389/fcb76481-5378-4a88-b414-911408732780)
![image](https://github.com/0-0-1y/Introductory-teaching/assets/91407389/06d1dfa4-22d5-4dfb-ad33-07db53dd104a)
接下来就在源代码中将文件路径改为这个路径，程序就能运行成功了
![image](https://github.com/0-0-1y/Introductory-teaching/assets/91407389/9b08a38d-5f27-4f0c-ab2e-7e49994c3c01)
