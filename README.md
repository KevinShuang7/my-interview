# 面试问题整理

## 自我介绍问题

## CSS

### 动画的实现方法及其区别

transition animation requestAnimationFrame
JavaScript 修改几何属性的话，会导致浏览器的回流和回流
同时由于 JavaScript 运行在浏览器的主线程中，主线程中还有其他的重要任务在运行，因而可能会受到干扰导致线程阻塞，从而丢帧
而 CSS 的动画是运行在合成线程中的，不会阻塞主线程，并且在合成线程中完成的动作不会触发回流和重绘
当然还有一个重要的点：JS 动画运行在 CPU，而 CSS 动画运行在 GPU
总的来说，CSS 动画的渲染成本小，并且它的执行效率高于 JavaScript 动画

### 媒体查询

[媒体查询](https://juejin.cn/post/7036628713571614750);

```css
@media screen and (max-width: 240px),
  (min-width: 360px) and (max-width: 700px) {
  .box1 {
    background-color: burlywood;
  }
}
```

### padding 的相对问题

[链接](https://juejin.cn/post/7012400693025718308);

### flex 布局

[flex](https://www.ruanyifeng.com/blog/2015/07/flex-grammar.html);

### grid 布局

## TypeScript

### type、interface 的区别

### any、never、unknown 的区别

### infer

### 逆变与协变

### 函数返回值推断

```typescript
function foo() {
  return 1;
}

type fooReturnType = ReturnType<typeof foo>;
```

## JavaScript

### es5 继承

### 原型、原型链

### async/await 实现

## React 相关问题

### 常见的 hooks 有哪些

### useEffect 的作用

### 不可变数据结构

[不可变数据结构](https://juejin.cn/post/6844903859618332680)

## 算法

### 冒泡、快排
