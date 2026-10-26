# reactor.core Skill

Use this skill to work with Norm module `reactor.core` version 6. Use only declarations listed below.

## `reactor.core`

Source: `CorePublisher.norm`

### `CorePublisher`

```norm
interface CorePublisher<T> extends Publisher<T>
```

Type parameters:

- `T`

## `reactor.core.org.reactivestreams`

Source: `org/reactivestreams/Publisher.norm`

### `Publisher`

```norm
interface Publisher<T>
```

Type parameters:

- `T`

## `reactor.core.publisher`

Source: `publisher/Flux.norm`

### `Flux`

```norm
class Flux<T> implements CorePublisher<T>
```

Type parameters:

- `T`

#### `Flux`

```norm
Flux(__JarBindingToken token)
```

Parameters:

- `token`: `__JarBindingToken`

#### `blockLast`

```norm
T? blockLast(Duration? arg0)
```

Parameters:

- `arg0`: `Duration?`

Returns: `T?`

#### `filter`

```norm
Flux<T>? filter(Function<Boolean(T?)>? arg0)
```

Parameters:

- `arg0`: `Function<Boolean(T?)>?`

Returns: `Flux<T>?`

#### `map`

```norm
Flux<V>? map<V>(Function<V?(T?)>? arg0)
```

Type parameters:

- `V`

Parameters:

- `arg0`: `Function<V?(T?)>?`

Returns: `Flux<V>?`

#### `take`

```norm
Flux<T>? take(Long arg0)
```

Parameters:

- `arg0`: `Long`

Returns: `Flux<T>?`

### `fluxEmpty`

```norm
Flux<T>? fluxEmpty<T>()
```

Type parameters:

- `T`

Returns: `Flux<T>?`

### `fluxError`

```norm
Flux<T>? fluxError<T>(Throwable? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `Throwable?`

Returns: `Flux<T>?`

### `fluxJust`

```norm
Flux<T>? fluxJust<T>(T? arg0)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `T?`

Returns: `Flux<T>?`

