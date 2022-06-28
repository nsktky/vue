<template>
<!-- templateの中身は一つの要素でないといけない -->
<div>
    <p>いいね({{ number / 2 }})</p>
</div>
</template>

<script>
export default{
    // 親componentからのデータを受け取るにはpropsを使用.propsは配列をとる.
    props: ['number'],
};
</script>

<!-- このcomponent内の要素だけにCSS適用させるには,scopedをつける -->
<style scoped>
    div {
        border: 2px solid red;
    }
</style>