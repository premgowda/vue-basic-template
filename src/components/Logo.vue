<template lang="html">
  <div>
    <h1>Logo</h1>
  </div>
</template>

<script>
export default {
  name: 'logo',
  props: {
    size: {
      default: 80
    }
  },
  data: function () {
    return {
      logo_size: this.size
    }
  }
}
</script>
