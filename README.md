TSF-TypeLib
===========

[![MIT](https://img.shields.io/github/license/736248591/TSF-TypeLib)](LICENSE) [![NuGet](https://img.shields.io/nuget/dt/TSF.TypeLib.Update)](https://www.nuget.org/packages/TSF.TypeLib.Update) ![GitHub](https://img.shields.io/github/issues/736248591/TSF-TypeLib) ![GitHub](https://img.shields.io/github/stars/736248591/TSF-TypeLib?style=social) ![GitHub](https://img.shields.io/github/watchers/736248591/TSF-TypeLib?style=social) ![NuGet](https://img.shields.io/nuget/v/TSF.TypeLib.Update) ![Github Version](https://img.shields.io/github/v/tag/736248591/TSF-TypeLib)

[原项目](https://github.com/NyaRuRu/TSF-TypeLib)

Type Library of Text Services Framework for .NET

开发TSF（输入法）提供C#的库。

# Fork说明

由于最近本人在从事开发输入法方面的工作，发现这个库用起来挺不错的，只是时间已经比较久没关系了，现在修复其中的BUG。

# 修复

## 1.0.3

根据 [《TSF自定义候选词列表界面》](https://www.cnblogs.com/ShengM/p/5620814.html)，修正`tlbimp.cs`文件。

- 修改`IEnumTfInputProcessorProfiles::Next IEnumTfLanguageProfiles：：Next ITfInputProcessorProfiles::GetLanguageList ITfRange::GetText`的签名。



## 1.0.2

- hresult的错误还是可选的处理。之前修正“解决ManagerReturnValues中的错误代码与COMException中错误代码冲突的问题。”的时候引入的BUG，造成了`Marshal.GetExceptionForHR`的错误直接抛出的问题。
- 添加`TF_DEFAULT`和`TS_DEFAULT`的定义。修改`GetSelection`函数。
- 解决ManagerReturnValues中的错误代码与COMException中错误代码冲突的问题。
- ITfContext.GetSelection 产生System.StackOverflowException
- 添加ManagerReturnValues.TF_E_INVALIDARG异常类型