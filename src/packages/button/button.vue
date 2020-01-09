<template>
  <button class="hrx-button" type="button">
    <slot></slot>
  </button>
</template>

<script>
import { oneOf } from '../../utils/assist'

export default {
  name: 'Button',
  props: {
    type: {
      validator (value) {
          return oneOf(value, ['default', 'primary', 'dashed', 'text', 'info', 'success', 'warning'])
      },
      type: String,
      default: 'default'
    },
    size: {
      validator (value) {
          return oneOf(value, ['small', 'large', 'default'])
      },
      default: 'default'
    }
  }
}
</script>
