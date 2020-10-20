TSF-TypeLib
===========

[原项目](https://github.com/NyaRuRu/TSF-TypeLib)

Type Library of Text Services Framework for .NET

开发TSF（输入法）提供C#的库。

# Fork说明

由于最近本人在从事开发输入法方面的工作，发现这个库用起来挺不错的，只是时间已经比较久没关系了，现在修复其中的BUG。

# 修复

## 2020年10月20日

- ITfContext.GetSelection 产生System.StackOverflowException
- 添加ManagerReturnValues.TF_E_INVALIDARG异常类型