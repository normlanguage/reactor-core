# Reactor Core 示例

[English](README.md) | [简体中文](README.zh-CN.md)

[hello.norm](hello.norm) 创建有限 Flux，过滤并转换其值，然后通过 Reactor 的 `blockLast(Duration)` 终结操作取得最后一个值。有界等待让结果确定。示例通过自己的 `Module module()` 声明依赖，是独立的模块消费者。

在仓库根目录运行：

```sh
norm run samples/hello.norm
```

预期输出：`Hello, norm`。[module.norm](../reactor/core/module.norm) 定义 v3 API，并指定 Reactor Core 3.8.7。
