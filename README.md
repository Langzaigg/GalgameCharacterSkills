# Galgame Character Skills

一个简单的Skills生成器。给定一段文本（Galgame剧情脚本/小说/任何单个长文本文件），自动将其中一个角色蒸馏为skills。

也支持生成适用于SillyTavern的角色卡。在提供VNDB信息时，会自动使用对应的立绘合并一份.png角色卡。

最好自行对生成结果进行一定程度的调整或是检查，即使有VNDB提供的信息也不保证符合实际。尤其是那些不属于VN的角色。

只测试过几个Galgame剧情文本，一般来说不要把多路线的所有内容一股脑塞进来，是没问题的。

## 安装

```bash
pip install -r requirements.txt
```

## 使用

```bash
python main.py
```

启动后自动打开浏览器访问 `http://127.0.0.1:5000`。

## 配置 LLM

在 Web 界面中填写：
- **Base URL**: API 地址，如 `https://api.openai.com/v1` 或 `http://localhost:11434`
- **Model Name**: 模型名称，如 `gpt-4` 或 `ollama/llama2`
- **API Key**: 你的 API 密钥

然后选择运行模式与对应文件开始处理。
