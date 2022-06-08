<template>
  <HeaderModal />
  <GoodsModal />
</template>

<script>
// @ is an alias to /src
import HeaderModal from '@/components/Header.vue'
import GoodsModal from '@/components/Goods.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderModal,
    GoodsModal
  }
}
</script>
