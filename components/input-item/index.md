---
category: UI Controls
type: UI Controls
chinese: 文本输入
english: InputItem
---


### 定义／Definition
文本框允许用户输入一行文本。通常可以使用文本框来收集用户的少量文本信息并执行一些直接作用，例如搜索操作。

### 规则 / Rule
- 文本框的左侧一般用于表述文本框的含义，而右侧用于展示附加的功能，如书签。
- 输入内容超出视窗宽度时，文本内容向前缩进。


## API


| 成员        | 说明           | 类型     |     可选值        | 默认值       |
|------------|----------------|--------------------|--------------|
| prefixListCls    |         | String | |  `am-list`  |
| type    |  格式  | String | 银行卡输入`bankCard`,手机号输入`phone`（此时最大长度固定为11,`maxLength`设置无效）,密码输入`password`,文本输入`text`, 数字输入`number`（尽量唤起数字键盘） |  `text`  |
| name    | input的name        | String | |  无  |
| value    | value值        | String | 是否设置value,决定了该InputItem是否是受控组件,详情请参考https://facebook.github.io/react/docs/forms.html |  无  |
| defaultValue    | 设置初始默认值        | String | |  ''  |
| editable    | 是否可编辑        | bool | |  true  |
| disabled    | 是否禁用        | bool | |  false  |
| placeholder      | placeholder        | String |  | 无  |
| clear      |  是否带清除功能 | bool | 仅`editable`为`true`,`disabled`为`false`,`value`设置才生效 | false  |
| maxLength      |  最大长度      | number | |  无  |
| onChange    | input change事件触发的回调函数,参数是value | Function | 当组件是受控组件时生效 |  无  |
| onBlur     | input blur事件触发的回调函数,参数是value | Function |  | 无  |
| onFocus    | input focus事件触发的回调函数,参数是value | Function |  | 无  |
| extra       | 右边注释   | string or node | |  ''  |
| onExtraClick      | extra点击事件触发的回调函数,参数是event对象 | Function |  | 无  |
| error       | 报错样式        | bool | |  false  |
| onErrorClick       | 点击报错icon触发的回调,        | Function | |  无  |
| labelNumber        | 标签字数（一个表单页面中,通常有多个InputItem,需要统一标签字数以便统一宽度,保持页面整洁、美观）        | number | `2`, `3`, `4`, `5`, `6`, `7`|  `4`  |
| size(本期不实现)       | 尺寸        | string | `large`,`small` |  `large`  |
| labelPosition(本期不实现)        | 标题方向        | string | `left`,`top` |  `left`  |
| textAlign(本期不实现)        | 文本对齐        | string | `left`,`center` |  `left`  |
