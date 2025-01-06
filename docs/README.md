<div style="width: 100%; text-align:center;">
    <img src="_images/logo.png" />
</div>

# UAI Editor：有爱文档，有爱、有AI。

> UAI Editor 是一个面向 AI 的、现代 UI 风格的下一代富文本编辑器。开箱即用、支持所有前端框架。


## 安装运行

### 软件安装

```bash
npm install uai-editor --registry https://registry.npmjs.org/
```

### 与VUE集成

```vue
<template>
  <div ref="editorDiv"/>
</template>

<script lang="ts">
import { UAIEditor } from "uai-editor";
import "uai-editor/dist/style.css"
export default {
  mounted(){
    new UAIEditor({
      element: this.$refs.editorDiv as Element,
      content: 'UAI Editor 是一个面向 AI 的、现代 UI 风格的下一代富文本编辑器。开箱即用、支持所有前端框架。',
    })
  }
}
</script>
```