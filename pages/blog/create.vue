<template>
  <div>
    <div>1 cái form có data rất nhiều</div>
    <div>
      <pre>{{ $data }}</pre>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Create',
  data() {
    return {
      model: {
        id: '',
        name: '',
      },
    }
  },
}
</script>

<style scoped></style>
