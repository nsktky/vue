<template>
<div>
  <LikeHeader></LikeHeader>
  <LikeNumber></LikeNumber>
</div>
</template>

<script>
import LikeHeader from './components/LikeHeader.vue';

// componentのlocal設定
export default {
  components: {
    LikeHeader: LikeHeader
  }
}
</script>

<style scoped>
    div {
        border: 2px solid blue;
    }
</style>