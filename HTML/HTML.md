# 核心概念

- **_元素_**：开始标签、内容、结束标签三部分组成的整体
- **_属性_**：是写在一个元素的开始标签中的特殊词汇，它们用于控制这个元素的行为

# 常用标签及属性

## “规范性“标签

### `<!DOCTYPE html>`

所有页面都应以其开头，被称为*声明*，确保浏览器尝试满足行业范围的规范

## “功能性”标签

### _`img`_

- 注意它是**自闭合**标签（无结束标签）
- 常用属性：`alt`（替代文本）、`src`

### _`a`_

**_锚点元素（超链接）_**，链接到另一个页面

- 常用属性：`href` 、
  - `target` 规定在何处打开链接
    - `_blank` 在新窗口中打开

### _`ul` & `ol`_

**_无序&有序列表_**

### _`li`_

**_列表项_**

### _`form`_

_表单_

- 常用属性：`action` （指示应将表单数据发送到哪里）

### _`id`_

**_用于标识元素_**

### _`input`_

- 注意它是**自闭合的、内联的**
- 常用属性：`placeholder` ，`required` （注意该属性无属性值，代表“必填”），`checked`（注意该属性无属性值，代表“使该复选框或单选按钮默认被选中”）
  - `type` 创建多种输入
    - text：文本，表单数据将为输入的内容
    - radio：单选，表单数据将为`name` / `value`  属性对
    - checkbox：复选框，表单数据将为`name` / `value`  属性对
  - `name` 指定输入数据的存放位置，或者说指明数据”属性“
    - 可以用于限制单选
  - `value` 设置 input 的数据值
    - 常在`type=radio`时使用

### `label`

帮助将  `input`  元素的文本与  `input`  元素本身关联起来

- 用法
  1. 套在`input`外面
  2. 套在`input`的文本外面，并添加与  `input`  的  `id`  具有相同值的  `for`  属性

### _`button`_

单击没有任何属性的表单按钮的默认行为会将数据提交到表单的  `action`  属性中指定的位置

- 注意它是**内联的**
- 常用属性：`type`

## “美化性”标签

- _`main` 正文_
- _`footer` 页脚_
- _`em`斜体_
- _`strong` 加粗_
- _`figure`独立引用内容_
  - _`figcaption`： 说明_
- _`fieldset` 块级元素_
  - *`legend` ：`fieldset`*  元素中内容的*标题*