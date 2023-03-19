# 使用google colab免费在线运行stable-diffusion-webui

`stable-diffusion-webui`项目地址：[stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)

使用google colab在线运行stable-diffusion-webui，可以通过上传models和extensions至网盘实现快速快速使用，需要注意的是网盘空间大小要足够

可将stable-diffusion-webui生成的图片保存到网盘的outputs目录下


### 准备Google Drive（如有必要）

- 在根目录中创建一个名为`stable-diffusion-webui`的文件夹。

- 在`stable-diffusion-webui`文件夹中创建两个名为`models`和`extensions`的文件夹。
![image](https://user-images.githubusercontent.com/51420323/226169034-a3478906-b77a-436c-89d3-6def3b7cdfdc.png)


### 执行脚本

使用当前脚本[v1/run_stable_diffusion](https://github.com/zc0125/colab-stable-diffusion-webui/blob/main/v1/run_stable_diffusion.ipynb)在google colab中执行

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

