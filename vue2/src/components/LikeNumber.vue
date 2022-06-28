<template>
<!-- templateの中身は一つの要素でないといけない -->
<div>
    <p>いいね({{ halfNumber }})</p>
</div>
</template>

<script>
export default{
    // 親componentからのデータを受け取るにはpropsを使用.propsは配列をとる.
    // propsはキャメルケースで表記
    // バリデーションするときはpropsをオブジェクトで指定.
    props: {
        // 型でバリデーション.違う型のときは警告が出る
        totalNumber: {
            type: Number,
            // 値が必ず必要な場合はtrue.
            // required: true
            default: 8
        }

    },
    computed: {
        halfNumber: function (){
            // 親componentから渡されたプロパティはdataのようにあつかう.
            return  this.totalNumber / 2
        }
    }
};
</script>

<!-- このcomponent内の要素だけにCSS適用させるには,scopedをつける -->
<style scoped>
    div {
        border: 2px solid red;
    }
</style>