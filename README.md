# 词云统计应用

这是一个简单易用的词云统计应用，可以帮助用户快速生成文本的词云图像。

## 功能特点

- 支持文本输入：用户可以直接输入或粘贴文本内容，支持区域大小调整
- 文件导入：支持导入txt文本文件
- 智能过滤：自动过滤标点符号、语气词、虚词等干扰词
- 词频统计：显示排名前10的高频词及其出现次数，支持区域大小调整
- 交互式过滤：词频统计后可添加自定义停用词，实时查看过滤效果
- 词云显示：生成美观的词云图像，支持区域大小调整
- 结果导出：可以将生成的词云图片保存为PNG格式
- 一键重置：支持快速初始化所有内容，方便开始新的分析
- 自动依赖管理：首次运行时自动检查并安装所需的依赖包
- 灵活布局：
  - 左右分栏设计，可通过拖动分隔线调整两侧比例
  - 每个功能区域支持独立调整大小
  - 所有区域位置可拖动重新排列
  - 自适应窗口大小变化

## 使用方法

1. 运行应用后，程序会自动检查并安装所需的依赖包
2. 安装完成后会打开图形界面，界面分为左右两栏：
   - 左侧栏：包含文本输入和词频统计区域
   - 右侧栏：包含词云显示和停用词管理区域
   - 可以通过拖动分隔线调整左右两栏的宽度比例
3. 每个功能区域都支持自由调整：
   - 拖动区域之间的分隔线可以调整各区域的大小
   - 拖动区域的标题栏可以改变区域的位置
   - 双击分隔线可以快速展开/收起相应区域
4. 在文本输入区域：
   - 直接输入或粘贴要分析的文本
   - 点击"导入文件"按钮选择txt文件
   - 点击"初始化"按钮可以清空所有内容，重新开始
5. 应用会自动过滤以下内容：
   - 标点符号（中英文）
   - 语气词（啊、哎、嗯等）
   - 虚词（的、了、着等）
   - 代词（这、那、什么等）
   - 单个字符和纯数字
6. 点击"生成词云"按钮，应用将自动分析文本并显示：
   - 词频统计结果（显示前10个高频词）
   - 初始词云图像
   - 自定义停用词管理区域
7. 在自定义停用词区域可以进行交互式过滤：
   - 查看词频统计后，可以选择需要过滤的词语
   - 在输入框中输入要过滤的词语，点击"添加停用词"按钮
   - 在列表中选择已添加的停用词，点击"删除选中的停用词"按钮可以取消过滤
   - 每次修改停用词后，词云会自动更新
8. 点击"保存图片"按钮可以将生成的词云保存到本地
9. 如需重新开始新的分析：
   - 点击"初始化"按钮
   - 所有内容将被清空
   - 应用将回到初始状态

## 技术栈

- Python 3.8+
- tkinter：GUI界面
- jieba：中文分词
- wordcloud：词云生成
- PIL：图像处理

## 运行应用

```bash
python wordcloud_app.py
```

注意：首次运行时，程序会自动检查并安装所需的依赖包，这可能需要一些时间。如果自动安装失败，程序会提示需要手动安装的包及其版本。 