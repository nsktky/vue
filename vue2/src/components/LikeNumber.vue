<template>
<!-- templateの中身は一つの要素でないといけない -->
<div>
    <p>いいね({{ number }})</p>
</div>
</template>

<script>
export default{
    data: function(){
        return {
            number: 5
        };
    }
};
</script>

<!-- このcomponent内の要素だけにCSS適用させるには,scopedをつける -->
<style scoped>
    div {
        border: 2px solid red;
    }
</style>