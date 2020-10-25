# Options 初始化参数

```javascript
const zxEditor = new ZxEditor(selector, options)
```
> [!TIP|label:selector]

> `id` 、`className` 选择器，或 `DOM元素`。

### editable

类型：`boolean`

默认：`true`

说明：内容是否可以被编辑。

### placeholder

类型：`string`

默认：`Enter...`

说明：编辑器内容为空时，显示的提示文字。

### placeholderColor

类型：`string`

默认：`#ccc`

说明：placeholder文字颜色。

### lineHeight

类型：`number/string`

默认：`1.5`

说明：正文内容行高。

### paragraphTailSpacing

类型：`string`

默认：`10px`

说明：段落尾部间距。

paragraph tail spacing, default 10px

### cursorColor

类型：`string`

默认：`#333`

说明：光标颜色(不一定兼容所有浏览器)。

### offsetTop

类型：`number`

默认:`30`

说明：输入内容时，光标位置距顶部距离。

### speed

类型：`number`

默认：`0`

说明：位置检测，输入可视区域元素移动速度，单位毫秒(ms)。

### toolbarBeenFixed

类型：`boolean`

默认：`true`

说明：底部工具栏是否始终固定。

### toolbarHeight

类型：`number`

默认：`50`

说明：底部工具栏高度。

### toolbarBtns

类型：`array`

默认：`['select-picture', 'text-style']`

说明：底部工具栏显示图标及顺序。

### customPictureHandler

类型：`boolean`

默认：`false`

说明：自定义图片处理，即不使用默认插入图片逻辑。

### imageMaxWidth

类型：`number`

默认：`750`

说明：正文中插入图片的最大宽度，大于该尺寸的图片将被等比缩放至宽度为设置值。单位 `px`。

### imageMaxSize

类型：`number`

默认：`20480`

说明：正文中插入图片的最大文件大小，默认20480Kib（20M），单位 `Kib`。

### imageSectionTemp

类型：`string`

默认：`<section class="child-is-picture"><img src="{url}"></section>`

说明：正文中插入图片元素html模板，`{url}`字符串会被替换成图片base64数据，或url地址。

### ignoreGif

类型：`boolean`

默认：`true`

说明：插入图片为gif，不做转换和裁剪等处理。注意，gif等比缩放或裁剪过程中只会取其第一帧，所以处理后的gif无动态效果。

### forceImageResize

类型：`boolean`

默认：`false`

说明：原图片尺寸小于目标尺寸时，强制缩放或裁剪图片。

Force the width/height of the picture, even if the width/height of the picture is smaller than the target width/height

### textStyleColors

类型：`array`

默认：`['#333', '#d0d0d0', '#ff583d', '#fdaa25', '#44c67b', '#14b2e0', '#b065e2']`

说明：文字样式扩展面板，可选颜色值列表。

> [!WARNING|style:flat|label:提示]

> 为空数组时，不显示颜色栏。

### textStyleTitle

类型：`string`

默认：`Set Style`

说明：文字样式扩展面板，标题。

### textStyleHeadLeftBtnText

类型：`string`

默认：`Clear style`

说明：文字样式扩展面板，标题栏左侧按钮文字内容。

### textStyleHeadAlign

类型：`string`

默认：`center`

说明：文字样式扩展面板，标题栏对齐方式。可选值 `left/center/right`。

### mainColor

类型：`string`

默认：`#00c1b7`

说明：编辑器主题色。

### borderColor

类型：`string`

默认：`#ddd`

说明：边框颜色。