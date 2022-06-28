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