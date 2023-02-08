# Auto-resize Textarea for Vue 3

An in-built auto-resize functionality for a textarea element using the scroll height of a singleton proxy textarea element attached to the document body. This is the 100% accurate implementation and does not break irrespective of the borders, padding, or amount of text.

## Install

`npm install vue3-autoresize-textarea`

## Usage

```vue

import AutoResizeTextarea from 'vue3-autoresize-textarea';


(In your SFC)
<template>
    <AutoResizeTextarea v-model="text" :maxRows="10" :minRows="4" />
</template>

<script setup>
const text = ref('');
</script>

```

## Props

| prop                | type      | description                                                                                                                                                                                                                                        |
| ------------------- | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `maxRows`           | `number`  | Maximum number of rows up to which the textarea can grow                                                                                                                                                                                           |
| `minRows`           | `number`  | Minimum number of rows to show for textarea                                                                                                                                                                                                        |

Apart from these, the component accepts all props that are accepted by `<textarea/>`.
