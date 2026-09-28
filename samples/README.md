# Reactor Core samples

[English](README.md) | [简体中文](README.zh-CN.md)

[hello.norm](hello.norm) creates a finite Flux, filters and maps its value, then observes the final value through Reactor's `blockLast(Duration)` terminal operation. The bounded wait keeps the example deterministic. It is a standalone consumer with its own `Module module()` dependency.

From the repository root, run:

```sh
norm run samples/hello.norm
```

Expected output: `Hello, norm`. [module.norm](../reactor/core/module.norm) defines the public API and pins Reactor Core 3.8.7.

The [acceptance example](../examples/sample/reactor/core/Main.norm) checks the Reactive Streams publisher type projection.
