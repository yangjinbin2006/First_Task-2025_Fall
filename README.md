# 2025秋 AI-NLP组第一次考核任务

关于此作业的完整描述，请参阅知识库内考核文档：

如果你在作业讲义或代码中发现任何问题，请随时提交 GitHub issue 或发起一个包含修复的 pull request。

---

## 配置

## 环境

我们使用 `uv` 来管理我们的环境，以确保可复现性、可移植性和易用性。
请[在此处](https://github.com/astral-sh/uv)安装 `uv`（推荐），或者运行 `pip install uv`/`brew install uv`。
我们建议你[在此处](https://docs.astral.sh/uv/guides/projects/#managing-dependencies)阅读一些关于在 `uv` 中管理项目的信息。

现在，你可以使用以下命令来运行仓库中的任何代码：

```sh
uv run <python_file_path>
```

环境将在必要时被自动解析和激活。

## 运行单元测试

```sh
uv run pytest
```

最初，所有的测试都应该因为 `NotImplementedError` 而失败。
要将你的实现连接到测试，请在 [./tests/adapters.py](./tests/adapters.py) 中补完相应的函数。

## 下载数据

下载 TinyStories 数据集

```sh
mkdir -p data
cd data

wget https://huggingface.co/datasets/roneneldan/TinyStories/resolve/main/TinyStoriesV2-GPT4-valid.txt

cd ..
```

---

感谢CS336课程为本次作业提供的帮助：[CS336](https://stanford-cs336.github.io/spring2025/)