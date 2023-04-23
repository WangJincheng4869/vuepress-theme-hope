---
title: ECharts
icon: chart-simple
---

让你 VuePress 站点中的 Markdown 文件支持图表。

此插件使用 [ECharts](https://echarts.apache.org/zh/index.html) 提供相应功能。

<!-- more -->

## 配置

::: code-tabs#language

@tab TS

```ts {8}
// .vuepress/config.ts
import { mdEnhancePlugin } from "vuepress-plugin-md-enhance";

export default {
  plugins: [
    mdEnhancePlugin({
      // 启用 ECharts 图表
      echarts: true,
    }),
  ],
};
```

@tab JS

```js {8}
// .vuepress/config.js
import { mdEnhancePlugin } from "vuepress-plugin-md-enhance";

export default {
  plugins: [
    mdEnhancePlugin({
      // 启用 ECharts 图表
      echarts: true,
    }),
  ],
};
```

:::

## 格式

````md
::: echarts 标题

```json
{
  // 此处为 ECharts 图表配置
}
```

:::
````

我们也支持 `js` 和 `javascript` 的代码块，你可以通过 `myChart` 变量获取 echarts 实例，并且你应该通过命名导出 `option` 来导出 echarts 选项。

## 文档

相关详情，详见 [ECharts 文档](https://echarts.apache.org/handbook/zh/get-started/).

## 案例

### 线图

<!-- @include: @echarts/line.snippet.md#demo -->

:::: details 代码

<!-- @include: @echarts/line.snippet.md -->

::::

### 柱状图

<!-- @include: @echarts/bar.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/bar.snippet.md -->

::::

### 饼图

<!-- @include: @echarts/pie.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/pie.snippet.md -->

::::

### 散点图

<!-- @include: @echarts/scatter.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/scatter.snippet.md -->

::::

### 极坐标图

<!-- @include: @echarts/polar.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/polar.snippet.md -->

::::

### 烛台图

<!-- @include: @echarts/candlestick.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/candlestick.snippet.md -->

::::

### 雷达图

<!-- @include: @echarts/radar.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/radar.snippet.md -->

::::

### 热力图

<!-- @include: @echarts/heat-map.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/heat-map.snippet.md -->

::::

### 树图

<!-- @include: @echarts/tree.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/tree.snippet.md -->

::::

### 多图

<!-- @include: @echarts/multiple.snippet.md#demo -->

:::: details Code

<!-- @include: @echarts/multiple.snippet.md -->

::::
