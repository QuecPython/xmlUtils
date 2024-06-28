# QuecPython XML解析组件

中文 | [English](README.md)

## 概述

QuecPython XML解析组件使用类似ElementTree的方式进行XML数据解析，最终解析出一个表示XML结构的字典(XML 指可扩展标记语言(eXtensible Markup Language))

该组件的实现主要根据不同的字符处理xml字符串来生成出一个字典。主要涉及引号、小于号、大于号、空格等字符的处理，通过对这些字符的处理来判断生成xml树结构的属性、节点、值等。


## 用法

- [API 参考手册](./docs/zh/API参考手册.md)

## 贡献

我们欢迎对本项目的改进做出贡献！请按照以下步骤进行贡献：

1. Fork 此仓库。
2. 创建一个新分支（`git checkout -b feature/your-feature`）。
3. 提交您的更改（`git commit -m 'Add your feature'`）。
4. 推送到分支（`git push origin feature/your-feature`）。
5. 打开一个 Pull Request。

## 许可证

本项目使用 Apache 许可证。详细信息请参阅 [LICENSE](LICENSE) 文件。

## 支持

如果您有任何问题或需要支持，请参阅 [QuecPython 文档](https://python.quectel.com/doc) 或在本仓库中打开一个 issue。
