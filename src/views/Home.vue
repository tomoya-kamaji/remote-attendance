<template>
  <div class="home">
    <Calender/>
  </div>
</template>

<script>
// @ is an alias to /src
import Calender from '@/components/Calender.vue'


export default {
  name: 'Home',
  components: {
    Calender
  }
}
</script>
