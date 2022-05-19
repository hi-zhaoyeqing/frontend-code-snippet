# frontend-code-snippet （前端代码片段）
> 数组去重

```
  // [1,2,3,4,5,1]--->[1,2,3,4,5]
  Array.from(new Set([1,2,3,4,5,1]))
```

> 字符串反转

```
   // 'hello world!' ---> '!dlrow olleh'
  'hello world!'.split("").reverse().join("")
```

> 数字排序

```
  // 从小到大 [2,1,3,4,5,6] ---> [1,2,3,4,5,6]
  [2,1,3,4,5,6].sort((a, b) => a — b)
  
  // 从大到小 [2,1,3,4,5,6] ---> [6,5,4,3,2,1]
  [2,1,3,4,5,6].sort((a, b) => b — a)
```
> 网站定时变灰

```
  const nowTime = new Date().getTime();
  const overTime = new Date("2022/05/12 00:00:00").getTime();
  const endTime = new Date("2022/05/13 00:00:00").getTime();
  if (nowTime > overTime && nowTime < endTime) {
    document.documentElement.style.cssText = "filter: grayscale(100%);";
  }
```
