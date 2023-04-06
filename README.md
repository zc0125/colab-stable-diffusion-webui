# [使用google colab在线运行stable-diffusion-webui](https://github.com/zc0125/colab-stable-diffusion-webui)

`stable-diffusion-webui`项目地址：[stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)

使用google colab在线运行stable-diffusion-webui，可以通过上传models和extensions(尽量不要使用，在线下载很快)，至网盘实现快速快速使用，需要注意的是网盘空间大小要足够

可将stable-diffusion-webui生成的图片保存到网盘的outputs目录下，用于同步生成图片


## 准备Google Drive（如有需要）

- Google Drive [地址](https://drive.google.com/drive/my-drive)

- 在根目录中创建一个名为`stable-diffusion-webui`的文件夹（和stable-diffusion-webui的运行目录层次相同）。

- 在`stable-diffusion-webui`文件夹中创建名为`models`、`extensions`和`outputs`的文件夹，用于保存自己的数据

- model文件夹下创建需要使用的model分类文件夹（如果没有要同步的内容，就不需要创建）

![image](https://user-images.githubusercontent.com/51420323/226169034-a3478906-b77a-436c-89d3-6def3b7cdfdc.png)

![image](https://user-images.githubusercontent.com/51420323/226173991-42c13d16-584f-47a3-8129-b71efd9c6870.png)


## 执行脚本（具体操作可见脚本注释）

使用当前脚本[v1/run_stable_diffusion](https://github.com/zc0125/colab-stable-diffusion-webui/blob/main/v1/run_stable_diffusion.ipynb)在google colab中执行

![image](https://user-images.githubusercontent.com/51420323/226174230-5a401105-e878-4e30-97a0-f34b2aebabad.png)


1. 执行当前脚本初始化运行目录

![image](https://user-images.githubusercontent.com/51420323/226173252-f34cc9bc-2c7f-44f0-a945-cec14639b4e6.png)

2. 运行

![image](https://user-images.githubusercontent.com/51420323/226173332-7a5f51d1-f798-4508-b0c1-c427b6a52f36.png)

3. 如果之前云盘没有extensions和outputs路径，可以运行当前命令同步到云盘，如果云盘存在extensions和outputs文件夹则会自动同步

![image](https://user-images.githubusercontent.com/51420323/226173925-5e5e2af6-df5a-4a8c-8a71-9b6f10614027.png)


4. 同步model，如果运行过程中有新下载的模型，可以同步到网盘（目前是同步到对应的`back_文件夹`，后续启动会自动使用）

![image](https://user-images.githubusercontent.com/51420323/227580634-46a33936-09bf-4c1e-90a3-3e8887495b10.png)


5. 云盘上新的model，需要在本次运行时，重新同步model至运行目录

![image](https://user-images.githubusercontent.com/51420323/226174360-d54ecd00-e72b-47e2-9f90-3eae4f406f41.png)

6. 在线下载model资源同步保存到drive，更快，请使用脚本进行下载


## 推荐插件

### 简体中文包

简体中文插件脚本已经下载安装，当前使用的[简体中文包](https://github.com/VinsonLaro/stable-diffusion-webui-chinese)

点击"Settings"，左侧点击"User interface"界面，在界面里最下方的"Localization (requires restart)"，选择"Chinese-All"或者"Chinese-English"

### 推荐提示词

已经整合到启动脚本中，默认使用中文提示词

自己的简体中文翻译版本：[点击跳转](https://github.com/zc0125/webui-tagcomplete/tree/branch/chinese-ex)

也可使用原作者项目自行进行翻译

## 科学上网

如果你没有一个合适的vpn来访问谷歌，并且经常使用，可以自己购买合适的vps，参考一键搭建教程，这里推荐v2ray

也可以购买现有的节点代理，这里推荐，[地址](https://www.paopao.dog/#/register?code=CExwfq3w)，如果可以，请填写我的邀请码`CExwfq3w`,这里有永久和其他多种套餐，很便宜，适合不大量使用和下载的用户

## 分享模型

使用别人分享的网盘链接，创建快捷方式到自己的网盘，占用极少的内存空间，原理上可以使用很多的模型，跳出磁盘大小的限制。

- 我的model模型（需要保存文件到对应文件夹，比如`Lora`，可以是`Lora_1`、`Lora2`等`Lora`开头的，运行时都能进行同步）：

如需更多模型请自行下载或联系我共享（之前分享的模型链接一直有问题，本次更新链接）

  - [google drive models/Stable-diffusion](https://drive.google.com/drive/folders/1kaYPZsdagb3JV5D5Ac1NB_3ZvEvWZghB?usp=sharing)

  - [google drive models/Lora](https://drive.google.com/drive/folders/1gADy8nIzW8OUF4NB5klyoKg6H9LUq87s?usp=sharing)
  
  使用共享模型时尽量不要引入太多模型，在线链接过多的快捷方式会导致运行缓慢，如果确定要要使用的模型建议复制到自己的网盘中，并同步到运行时的磁盘，可以大大提高运行速度。

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

