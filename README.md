# XunityAutoTranslator-SakuraLLM


本项目通过调用SakuraLLM，实现Unity游戏中日文文本的自动翻译。

## 准备工作

### 1. 安装Sakura_Launcher_GUI
下载链接：[https://github.com/PiDanShouRouZhouXD/Sakura_Launcher_GUI/releases] 以及

下载相关的Sakura模型

### 2. 安装依赖
确保已安装以下软件和库：
- **XUnity.AutoTranslator**
- **Python 3.x**

安装必要的Python库：
```bash
pip install Flask gevent openai
```


### 3. 自定义API配置
如果使用其他模型，请修改以下配置：
```python
# API配置
Base_url = "http://127.0.0.1:8080"     #获取请求地址
Model_Type =  "GalTransl-7B-v2.6-IQ4_XS"     #获取模型类型 Sakura-13B-LNovel-v0.8或者Sakura-13B-LNovel-v0.9
```

## 启动项目

### 1. 启动Python脚本
确保Python脚本成功启动，命令行应显示：
```
服务器在 http://127.0.0.1:4000 上启动
```

### 2. 配置XUnity.AutoTranslator
修改XUnity.AutoTranslator插件的配置文件`AutoTranslatorConfig.ini`或`Config.ini`：
```ini
[Service]
Endpoint=CustomTranslate

[Custom]
Url=http://127.0.0.1:4000/translate
```

## 参考项目
- [XUnity.AutoTranslator-Sakura](https://github.com/as176590811/XUnity.AutoTranslator-Sakura)
- [XunityAutoTranslator-Gemini-API](https://github.com/0001lizhubo/XunityAutoTranslator-Gemini-API)   和  [XUnity.AutoTranslator-deepseek](https://github.com/0001lizhubo/XUnity.AutoTranslator-deepseek) 
---

通过以上步骤，您可以轻松实现Unity游戏中日文文本的自动翻译。如有问题，请参考相关文档或联系开发者。
