---
category: Pro Components
cols: 1
subtitle: 分页
type: Navigation
title: Pagination
---

采用分页的形式分隔长列表，每次只加载一个页面。

## 何时使用

- 当加载/渲染所有数据将花费很多时间时；
- 可切换页码浏览数据。

## API

### Pagination

| 参数 | 说明 | 类型 | 默认值 |
| --- | --- | --- | --- |
| total | 总数 | number |  |
| page | 当前页 | number |  |
| pageSize | 分页数 | number |  |
| onChange | 页码改变的回调，参数是改变后的页码及每页条数 | (page, pageSize) => void |  |
| pageSizeOptions | 指定每页可以显示多少条 | string\[] | \['10', '20', '50', '100'\] |
| showSizeChanger | 是否显示分页大小选择器 | boolean | true |
| showQuickJumper | 是否显示快速跳转至某页 | boolean | false |
| showSizeChangerLabel | 是否显示分页大小选择器的标签 | boolean | true |
| showTotal | 显示总数 | boolean | true |
| showPager | 显示数字按钮 | boolean | false |
| itemRender | 按钮渲染。`type` - 按钮类型，可选值：`first` `last` `prev` `next` `jump-prev` `jump-next` | (page, type) => ReactNode |  |
| sizeChangerPosition | 分页大小选择器的位置，可选值: `left` `right` | string | left |
| sizeChangerOptionRenderer | 分页大小选择器的选项渲染器 | ({ dataSet, record, text, value}) => ReactNode | ({ text }) => text |

更多属性请参考 [DataSetComponent](/components-pro/core/#DataSetComponent)。
