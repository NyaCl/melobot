# OneBot 事件预处理

## 预处理简介

melobot 的 OneBot 支持中提供了一些常用的工具，用来在事件处理前进行一些特定的操作。

这些操作一般称为预处理。以下是内置的预处理支持。

## 检查（校验）

检查当前事件是否满足某些条件，如果满足则通过检查。

## 匹配

检查当前消息事件的消息内容，是否满足某些匹配条件。例如：以 `xxx` 起始，包含 `xxx` 或可以通过指定的正则表达式匹配等。

## 解析

对当前消息事件的消息内容进行解析，并返回一个包含解析结果的 {class}`.ParseArgs` 对象。

```{admonition} 重要提示
:class: attention
内置的所有预处理支持，**都不是异步安全的**。
```
