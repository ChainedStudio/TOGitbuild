# SanityEvents.change

## Basic info

- Valid script types: [SERVER]

- Has result? ✔

- Event class: SanityChangeEventJS (third-party)

```
Handle Sanity Change Event caused by Passive Events.```

### Available fields:

| Name | Type | Static? |
| ---- | ---- | ------- |

Note: Even if no fields are listed above, some methods are still available as fields through *beans*.

### Available methods:

| Name | Parameters | Return type | Static? |
| ---- | ---------- | ----------- | ------- |
| getEntity |  |  | LivingEntity | ✘ |
| getSanity |  |  | float | ✘ |
| addSanity | float |  | void | ✘ |
| setSanity | float |  | void | ✘ |
| unclampNorm | float |  | float | ✘ |
| getPreviousSanity |  |  | float | ✘ |
| approximation | float, int |  | float | ✘ |
| clampNorm | float |  | float | ✘ |
| hasGameStage | String |  | boolean | ✘ |
| addGameStage | String |  | void | ✘ |
| removeGameStage | String |  | void | ✘ |
| getPlayer |  |  | Player | ✘ |
| getLevel |  |  | Level | ✘ |
| getServer |  |  | MinecraftServer | ✘ |
| exit | Object |  | Object | ✘ |
| exit |  |  | Object | ✘ |
| success | Object |  | Object | ✘ |
| success |  |  | Object | ✘ |
| cancel | Object |  | Object | ✘ |
| cancel |  |  | Object | ✘ |


### Documented members:

- `float getSanity()`
```
Get the sanity value
```

- `void addSanity(float var0)`

  Parameters:
  - var0: float

```
Increase sanity
```

- `void setSanity(float var0)`

  Parameters:
  - var0: float

```
Set the sanity value to a specific number (0-100)
```

- `float unclampNorm(float var0)`

  Parameters:
  - var0: float

```
Convert the value between 0 and 1 into a readable number
```

- `float getPreviousSanity()`
```
Get the sanity value before the change
```

- `float approximation(float var0, int var1)`

  Parameters:
  - var0: float
  - var1: int

```
Truncate a number to n significant decimal places (rounding mode)
```

- `float clampNorm(float var0)`

  Parameters:
  - var0: float

```
Convert a number to a value between 0 and 1
```

- `boolean hasGameStage(String var0)`

  Parameters:
  - var0: String

```
Checks if the player has the specified game stage
```

- `void addGameStage(String var0)`

  Parameters:
  - var0: String

```
Adds the specified game stage to the player
```

- `void removeGameStage(String var0)`

  Parameters:
  - var0: String

```
Removes the specified game stage from the player
```

- `Object exit(Object var0)`

  Parameters:
  - var0: Object

```
Stops the event with the given exit value. Execution will be stopped **immediately**.

`exit` denotes a `default` outcome.
```

- `Object exit()`
```
Stops the event with default exit value. Execution will be stopped **immediately**.

`exit` denotes a `default` outcome.
```

- `Object success(Object var0)`

  Parameters:
  - var0: Object

```
Stops the event with the given exit value. Execution will be stopped **immediately**.

`success` denotes a `true` outcome.
```

- `Object success()`
```
Stops the event with default exit value. Execution will be stopped **immediately**.

`success` denotes a `true` outcome.
```

- `Object cancel(Object var0)`

  Parameters:
  - var0: Object

```
Cancels the event with the given exit value. Execution will be stopped **immediately**.

`cancel` denotes a `false` outcome.
```

- `Object cancel()`
```
Cancels the event with default exit value. Execution will be stopped **immediately**.

`cancel` denotes a `false` outcome.
```



### Example script:

```js
SanityEvents.change((event) => {
	// This space (un)intentionally left blank
});
```

