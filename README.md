# vue-digital-transform

一个基于 Vue 的数字切换动效库

## Install

```bash
npm install vue-digital-transform
```

## Example

```html
<template>
  <DigitalTransform :value="num" dislocation :interval="200"></DigitalTransform>
</template>
```

```js
import DigitalTransform from "vue-digital-transform";

export default {
  components: {
    DigitalTransform
  },
  data() {
    return {
      num: 0
    };
  }
};
```

## Config

| prop                  | type          | description                                   | default   |
| --------------------- | ------------- | --------------------------------------------- | --------- |
| value                 | Number,String | 需要切换的数字，只能由 0-9 . , 组成           | undefined |
| dislocation           | Boolean       | 单个数字是否过渡时间是否不一致                | false     |
| interval              | Number        | 单个数字过渡时间（ms）                        | 500       |
| useGrouping (v1.1.0+) | Boolean       | 是否开启分隔符(对 value 为 Number 类型的有效) | false     |
