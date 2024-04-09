# PyautoVanguard
> PyAutoVanguard

## 项目介绍

`PyAutoVanguard` 是一个结合了行为驱动开发（BDD）和页面对象模式（POM）的Python自动化测试框架。它旨在提供一套结构清晰、易于维护和扩展的测试解决方案，特别适用于具有复杂UI和交互的应用程序。该框架使用`pytest`作为测试运行器，支持API测试、UI测试等多种测试类型，并集成了OCR、图像处理等实用工具库。


## 特性

- 基于BDD和POM的设计理念，提高测试用例的可读性和可维护性。
- 支持API测试、Web应用测试、移动应用测试等多种测试类型。
- 集成OCR、图像处理等工具库，以处理复杂的UI交互和验证场景。
- 使用`pytest`作为测试运行器，支持丰富的插件生态系统和参数化功能。
- 提供清晰的目录结构和模块划分，便于团队协作和项目管理。
- 生成详细的测试报告，包括Allure报告和自定义Web报告。
- 可与Jenkins等CI/CD工具集成，实现持续集成/持续部署。



---

## 目录结构说明

```
pyautovanguard/
├── README.md                   # 项目说明文档
├── config/                     # 配置文件目录
├── data/                       # 测试数据目录
├── features/                   # BDD特性文件目录
├── pages/                      # 页面对象目录
├── report/                     # 测试报告目录（可能为空，测试运行后生成）
├── requirements.txt            # Python依赖文件
├── steps/                      # 步骤定义目录
├── tests/                      # 测试用例目录
└── webReport/                  # Web报告相关文件和配置目录
```

- `README.md`：项目的说明文档，包含项目的简介、安装指南、使用方法等。
- `config/`：存放项目的配置文件，如`config.yaml`。
- `data/`：测试数据目录，可根据需要划分，例如：`api_data/`、`app_data/`等子目录。
- `features/`：BDD特性文件目录，存放以`.feature`为扩展名的Cucumber特性文件。
- `pages/`：页面对象目录，存放页面对象的Python文件。
- `report/`：测试报告目录，测试运行后生成测试报告文件。
- `requirements.txt`：Python依赖文件，列出了项目所需的第三方库及其版本。
- `steps/`：步骤定义目录，存放与BDD，Cucumber文件中场景相对应的步骤定义Python文件。
- `tests/`：测试用例目录，存放测试用例的Python文件。
- `webReport/`：Web报告相关文件和配置目录，包含生成Web报告的脚本和配置文件。


## 安装指南

1. 克隆本仓库到本地：`git clone https://github.com/alarmsday/PyautoVanguard.git`
2. 进入项目目录：`cd pyautovanguard`
3. 创建并激活Python虚拟环境（可选）
4. 安装依赖：`pip install -r requirements.txt`

## 使用方法

1. 编写或更新测试用例：在`features/`目录下编写BDD特性文件（`.feature`），在`steps/`目录下编写对应的步骤定义文件（`.py`），并在`pages/`目录中创建或更新页面对象。
2. 运行测试：使用`tests/run.py`运行测试用例，例如：`python tests/run.py`
3. 查看测试报告：测试运行后，在`report/`目录下生成测试报告文件。你还可以使用Allure生成更详细的报告，并通过`webReport/`目录下的脚本将其部署为Web应用。


## 贡献与反馈

我们欢迎任何形式的贡献和反馈！如果你在使用过程中遇到问题或有改进建议，请随时提交issue。

## 作者

**刘昊然** - 
邮箱: 849271288@qq.com




## 致谢

提前感谢所有为该项目做出贡献的人员.


## 许可证

本项目使用MIT许可证进行开源。请参阅LICENSE文件以获取更多信息。

