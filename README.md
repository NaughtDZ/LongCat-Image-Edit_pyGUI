# LongCat-Image-Edit_pyGUI

pyGUI for LongCatImageEdit

单个脚本实现的  https://huggingface.co/meituan-longcat/LongCat-Image-Edit   项目的GUI用户界面

推荐首先使用uv venv venv 创建venv虚拟环境，然后激活虚拟环境

紧接着使用uv pip install pip 安装pip，防止官方的脚本pip安装报错

接下来使用uv pip install git+https://github.com/huggingface/diffusers  安装项目

然后把GUI.py放到venv同级目录

记得补充安装 pytorch (https://pytorch.org/get-started/locally/),建议还是通过uv pip install 安装

然后安装uv pip install transformer (是的，官方脚本不会自动安装)

最后记得安装uv pip install accelerate (是的，官方脚本还是不会自动安装)

然后在虚拟环境中运行gui.py (建议使用V2版本，因为官方的程序并不会自动缩放图片导致可能的oom，v2有安全缩放逻辑 如果输入图太大（长边 > 1344 或总像素 > 1.8M）会自动钳制图片大小)

好好享受！

(有个需要GUI界大哥帮忙的事情，跑图时候UI会无响应，影响拖放窗口什么的，有大哥会修复的欢迎修复)
