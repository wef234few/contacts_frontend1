# 前端代码规范

基于 [Google HTML/CSS/JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html) 和主流前端开发最佳实践。

## HTML 规范

### 文档结构
- 使用 HTML5 文档类型：`<!DOCTYPE html>`
- 包含必要的 meta 标签：charset、viewport
- 使用语义化标签（header、nav、main、section、footer等）

### 代码格式
- 使用 2 个空格缩进
- 标签和属性使用小写字母
- 属性值使用双引号
- 自闭合标签不加斜杠（`<br>` 而不是 `<br />`）

### 可访问性
- 为 img 标签添加 alt 属性
- 为表单元素添加 label
- 使用有意义的标题结构（h1-h6）

## CSS 规范

### 命名规范
- 使用短横线命名法（kebab-case）：`.contact-list`
- 避免使用元素选择器（如 div、span）
- 类名要有语义化意义

### 代码组织
- 使用 2 个空格缩进
- 选择器嵌套不超过 3 层
- 相关属性分组排列（布局 → 盒模型 → 文本 → 视觉）
- 使用 flex/grid 进行现代布局

### 响应式设计
- 使用移动优先的媒体查询
- 使用相对单位（rem、em、%）而非绝对单位（px）

## JavaScript 规范

### 变量和函数
- 使用 `const` 和 `let`，避免 `var`
- 使用驼峰命名法（camelCase）
- 函数和变量名要有描述性
- 使用箭头函数保持上下文

### 异步处理
- 使用 `async/await` 替代回调函数
- 使用 Promise 处理异步操作
- 添加错误处理（try-catch）

### 代码质量
- 语句末尾使用分号
- 使用 === 和 !== 而非 == 和 !=
- 避免全局变量污染
- 函数长度不超过 50 行

## 项目结构规范

### 文件组织
- 每个组件有独立的文件夹，包含 HTML、CSS、JS 文件
- 静态资源（图片、字体等）放在 `assets` 文件夹
- 组件之间的依赖关系要清晰，避免循环引用