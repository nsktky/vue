<template>
<div>
  <LikeHeader></LikeHeader>
  <LikeNumber></LikeNumber>
</div>
</template>

<script>
import LikeHeader from './LikeHeader.vue';

// componentのlocal設定
export default {
  components: {
    LikeHeader: LikeHeader
  }
}
</script>