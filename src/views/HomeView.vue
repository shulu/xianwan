<template>
  <div class="home">
    <HeaderModal />
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderModal from '@/components/Header.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderModal
  }
}
</script>
