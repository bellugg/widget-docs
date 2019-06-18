---
id: listening-for-changes
title: Listening for form value changes
sidebar_label: Listening for changes
---

After you have done widget loading on your web application, the next step is adding a listener for form value changes. Code snippets below are examples for popular JavaScript frameworks:

## Plain JavaScript

```js
document.querySelector('bellugg-widget')
  .addEventListener('change', function (event) {
    console.log('Info from widget', event.detail[0]);
  });
```


## jQuery

```js
$('bellugg-widget').on('change', function (event) {
  console.log('Info from widget', event.detail[0]);
});
```

## Vue

```html
<template>
  <bellugg-widget @change="changeCallback"></bellugg-widget>
</template>
<script>
  export default {
    methods: {
      changeCallback(event) {
        console.log('Info from widget', event.detail[0]);
    }
  };
</script>
```
