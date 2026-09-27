# Reactor Core

[English](README.md) | [简体中文](README.zh-CN.md)

An adapter for the common `Flux` creation, transformation, filtering, truncation, and bounded terminal observation APIs of Reactor Core 3.8.7. The package declaration is in [module.norm](reactor/core/module.norm). `Flux<T>` interoperates with frameworks using Reactive Streams through the standard `std.concurrent.Publisher<T>`.

[Samples](samples/README.md) include a standalone consumer that observes a finite Flux.
