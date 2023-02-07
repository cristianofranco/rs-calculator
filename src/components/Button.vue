<template>
  <button :class="[
    'w-16 h-16 shadow-lg rounded-full flex items-center justify-center text-2xl cursor-pointer',
    { 'operator-bg-shadow': isOperator },
    { 'equals-bg-shadow': isEquals },
    ]" :style="{ color: computedTextColor }">
    <template v-if="iconPath">
      <img :src="iconPath" :alt="label" :style="{ width: iconWidth }">
    </template>
    <template v-else>
      {{ label }}
    </template>
  </button>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: ''
    },
    textColor: {
      type: String,
      default: '#fff'
    },
    iconPath: {
      type: String,
      default: '',
    },
    isCE: {
      type: Boolean,
      default: false
    },
    isOperator: {
      type: Boolean,
      default: false
    },
    isEquals: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    computedTextColor() {
      return this.isCE ? '#975DFA' : this.textColor;
    }
  }
}
</script>