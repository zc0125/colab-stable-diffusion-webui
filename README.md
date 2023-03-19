# [使用google colab在线运行stable-diffusion-webui](https://github.com/zc0125/colab-stable-diffusion-webui)

`stable-diffusion-webui`项目地址：[stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)

使用google colab在线运行stable-diffusion-webui，可以通过上传models和extensions至网盘实现快速快速使用，需要注意的是网盘空间大小要足够

可将stable-diffusion-webui生成的图片保存到网盘的outputs目录下


### 准备Google Drive（如有必要）

- Google Drive [地址](https://drive.google.com/drive/my-drive)

- 在根目录中创建一个名为`stable-diffusion-webui`的文件夹（和stable-diffusion-webui的运行目录层次相同）。

- 在`stable-diffusion-webui`文件夹中创建两个名为`models`和`extensions`的文件夹

- model文件夹下创建需要使用的model分类文件夹
![image](https://user-images.githubusercontent.com/51420323/226169034-a3478906-b77a-436c-89d3-6def3b7cdfdc.png)
![image](https://user-images.githubusercontent.com/51420323/226173991-42c13d16-584f-47a3-8129-b71efd9c6870.png)


### 执行脚本

使用当前脚本[v1/run_stable_diffusion](https://github.com/zc0125/colab-stable-diffusion-webui/blob/main/v1/run_stable_diffusion.ipynb)在google colab中执行
![image](https://user-images.githubusercontent.com/51420323/226174230-5a401105-e878-4e30-97a0-f34b2aebabad.png)


1. 执行当前脚本初始化运行目录
![image](https://user-images.githubusercontent.com/51420323/226173252-f34cc9bc-2c7f-44f0-a945-cec14639b4e6.png)

2. 运行
![image](https://user-images.githubusercontent.com/51420323/226173332-7a5f51d1-f798-4508-b0c1-c427b6a52f36.png)

3. 如果之前云盘没有extensions和outputs路径，可以运行当前命令同步到云盘，如果云盘存在extensions和outputs文件夹则会自动同步

![image](https://user-images.githubusercontent.com/51420323/226173925-5e5e2af6-df5a-4a8c-8a71-9b6f10614027.png)


4. 同步model，如果运行过程中有新下载的模型，可以同步到网盘
![image](https://user-images.githubusercontent.com/51420323/226173791-8b40b6cd-370d-4ec9-a756-a4ed7bcbac67.png)


4. 云盘上传的新的model，需要在本次运行时，重新同步model至运行
![image](https://user-images.githubusercontent.com/51420323/226173551-ab28bde8-1c6d-45cf-9e89-e7d120762bad.png)



### 简体中文包
简体中文插件脚本已经下载安装，当前使用的[简体中文包](https://github.com/VinsonLaro/stable-diffusion-webui-chinese)

点击"Settings"，左侧点击"User interface"界面，在界面里最下方的"Localization (requires restart)"，选择"Chinese-All"或者"Chinese-English"

### 分享

- 我的model模型和拓展（需要保存文件到对应文件夹，软链不行）：
[google drive models/Stable-diffusion](https://drive.google.com/drive/folders/1wSpxGyqD3rGY6LDKfFXYYwxtd1_amjuS?usp=sharing)
[google drive models/Lora](https://drive.google.com/drive/folders/1BTmTJesXW9j2ZtLgUMlvqMup8QIAVaFJ?usp=sharing)
[google drive extensions](https://drive.google.com/drive/folders/1Wrta7OGFNs-7Us7h4CIh-wCHYKu1bgqt?usp=sharing)

- ControlNet模型：
```
https://huggingface.co/webui/ControlNet-modules-safetensors/tree/main
https://huggingface.co/lllyasviel/ControlNet/tree/main/models
```

- 相关网站
```
https://civitai.com/
https://ai.dawnmark.cn/
https://arthub.ai/
https://www.krea.ai/
https://tags.novelai.dev/
```

更多好用的模型或者拓展可以在Issues中共享出来，感谢分享。

