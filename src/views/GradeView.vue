<template>
  <div class="grade-page">
    <Grade_Eva />
  </div>
</template>

<script>
  import Grade_Eva from '@/components/grade/Grade.vue'

  export default {
    name: 'Grade',
    components: {
    Grade_Eva
  }
    
  }
</script>

<style>
.grade-page {
  min-height: 100vh;
  background: #eeeeee;
}
</style>