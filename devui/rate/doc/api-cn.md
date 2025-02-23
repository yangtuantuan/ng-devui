# 如何使用
在module中引入：
```ts
import { RateModule } from 'ng-devui/rate';
```

在页面中使用：
```html
<d-rate [ngModel]="value" [count]="5"></d-rate>
```
# Rate

## d-rate 参数

|   参数    |              类型               | 默认值  | 描述                                                     | 跳转 Demo                                              |全局配置项| 
| :----------------: | :-------: | :-----------------------------: | :---: | :------------------------------------------------------- | ------------------------------------------------------ |
|   readonly    |            `boolean`            | false | 可选，设置是否为只读模式，只读模式无法交互               | [只读模式](demo#read-only-mode)           |
|   count   |            `number`             |   5   | 可选，设置总等级数                                       | [只读模式](demo#read-only-mode)           |
|   ~~type~~    | `'success'\|'warning'\|'error'` |  --   | 可选，设置当前评分的类型，不同类型对应不同颜色（`已废弃，建议使用color`）           | [设置颜色](demo#using-the-type-parameter) |
|   color   |            `string`             |  --   | 可选，星星颜色                                           | [动态模式-自定义](demo#dynamic-mode-Custom)      |
|   ~~icon~~    |            `string`             |  --   | 可选，评分图标的样式，只支持 devUI 图标库中所有图标（`已废弃，建议使用character`）      | [动态模式](demo#dynamic-mode)             |
| character |            `string\|TemplateRef`             |  --   | 可选，评分图标的样式，支持传入文本或模板 | [动态模式-自定义](demo#dynamic-mode-Custom)      |
| allowHalf |            `boolean`             |  false   | 可选，动态模式下是否允许半选 | [半选模式](demo#rate-half)      |
