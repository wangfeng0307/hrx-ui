---
title: Button
---

# 按钮
<script>
export default {
  data() {
    return {
      button: '默认'
    }
  }
}
</script>

<template>
  <hrx-button>{{button}}</hrx-button>
  <hrx-button type="primary">主色</hrx-button>
  <hrx-button type="success">成功</hrx-button>
  <hrx-button type="info">提示</hrx-button>
</template>


### 使用
```html
<hrx-button>默认</hrx-button>
<hrx-button type="primary">主色</hrx-button>
<hrx-button type="success">成功</hrx-button>
<hrx-button type="info">提示</hrx-button>
```