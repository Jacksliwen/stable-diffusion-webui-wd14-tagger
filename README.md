# Tagger for [Automatic1111's WebUI](https://github.com/AUTOMATIC1111/stable-diffusion-webui)
使用各种模型（例如 DeepDanbooru）询问单个或多个图像文件的 booru 样式标签。

[英文版](README.en.md)

## 免责声明
我没有制作任何模型，大部分代码大量借用自 DeepDanbooru 和 MrSmillingWolf 的标记器。

## 安装
1. *Extensions* -> *Install from URL* -> Enter URL of this repository -> Press *Install* button
   - 或将此存储库克隆到 `extensions/`
      ```sh
      $ git clone https://github.com/toriato/stable-diffusion-webui-wd14-tagger.git extensions/tagger
      ```

1. *(optional)* 添加询问模型
   - #### [*Waifu Diffusion 1.4 Tagger by MrSmilingWolf*](docs/what-is-wd14-tagger.md)
      第一次运行时会自动从 [HuggingFace repository](https://huggingface.co/SmilingWolf/wd-v1-4-vit-tagger) 存储库下载。

   - #### *DeepDanbooru*
      1. 下面可以找到各种模型文件。
         - [DeepDanbooru models](https://github.com/KichangKim/DeepDanbooru/releases)
         - [e621 model by 🐾Zack🐾#1984](https://discord.gg/BDFpq9Yb7K)
            *(link contains NSFW contents!)*

      1. 将包含模型和配置的项目文件夹移动到 `models/deepdanbooru`

      1. 文件结构应该类似于:
         ```
         models/
         └╴deepdanbooru/
           ├╴deepdanbooru-v3-20211112-sgd-e28/
           │ ├╴project.json
           │ └╴...
           │
           ├╴deepdanbooru-v4-20200814-sgd-e30/
           │ ├╴project.json
           │ └╴...
           │
           ├╴e621-v3-20221117-sgd-e32/
           │ ├╴project.json
           │ └╴...
           │
           ...
         ```

1. 启动或重新启动 WebUI。
   - 或者您可以在询问器下拉框后按刷新按钮。
   - "安装后必须完全关闭稳定扩散并重新运行！"


## 型号对比
[Model comparison](docs/model-comparison.md)

## 截屏
![Screenshot](docs/screenshot.png)

由 [hecattaart](https://vk.com/hecattaart?w=wall-89063929_3767) 制作的艺术品

## 版权

公共领域，借用部分除外（例如 dbimutils.py）
