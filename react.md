### [LifeCycle] getDerivedStateFromProps

```
getDerivedStateFromProps exists for only one purpose. 

It enables a component to update its internal state as the result of changes in props.

Derived state should be used sparingly

你可以在渲染过程中更新 state, React 会立即退出第一次渲染并用更新后的 state 重新运行组件以避免耗费太多性能。

```

### All problems with _getDerivedStateFromProps_ were caused by
1. unconditionally updating state from props
2. updating state whenever props and state don't match.

### [Hooks] useEffect
```
07:41:22.910 index.js:1452 Warning: useEffect function must return a cleanup function or nothing. 
Promises and useEffect(async () => …) are not supported, 
but you can call an async function inside an effect.. 
```


### [Hooks] It sees the props & state & variables defined in component.
```
If we apply the same substitution principle, each render “sees” its own count:

Every function inside the component render 
(including event handlers, effects, timeouts or API calls inside them) 
captures the props and state of the render call that defined it.
```
