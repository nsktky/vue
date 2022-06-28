<template>
<div>
  <LikeHeader></LikeHeader>
  <h2>{{ number }}</h2>
  <!-- 子componentにデータを渡すには、propsで指定した値を属性のように表記.動的に扱いたい場合はv-bind. -->
  <LikeNumber :number='number'></LikeNumber>
  <LikeNumber :number='number'></LikeNumber>
</div>
</template>

<script>
import LikeHeader from './components/LikeHeader.vue';

// componentのlocal設定
export default {
  data: function() {
    return {
      number: 10
    }
  },
  components: {
    LikeHeader: LikeHeader
  }
}
</script>
