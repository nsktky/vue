<template>
<div>
  <LikeHeader></LikeHeader>
  <h2>{{ number }}</h2>
  <!-- 子componentにデータを渡すには、propsで指定した値を属性のように表記.動的に扱いたい場合はv-bind. -->
  <!-- ケバブケースで書いた方がよい. -->
  <!-- 子componentから値を受け取るときはカスタムイベントを使用する.$eventでdataを受け取る. -->
  <LikeNumber :total-number='number' @my-click="number = $event"></LikeNumber>
  <!-- カスタムイベントは関数にしてもよい. -->
  <LikeNumber :total-number='number' @my-click="increment"></LikeNumber>
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
  },
  methods: {
    // 子からdata受け取る関数.引数を設定し,dataとして取り扱う.
    increment: function (value) {
      this.number = value
    }

  }
}
</script>
