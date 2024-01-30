<template>
  <button class="button" @click="handleClick">
    {{ label }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    label: {
      type: String,
      required: true
    },
    person: {
      type: String,
      required: true
    }
  },
  methods: {
    handleClick() {
      alert('Button clicked ' + this.person)
    }
  }
}
</script>

<style scoped>
.button {
  /* Button styles here */
}
</style>
