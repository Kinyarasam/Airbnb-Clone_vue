<template>
    <div class="cursor-pointer">
        <img :src="src" class="rounded" />
    </div>
</template>

<script>
export default {
    props: [ 'src' ],
    data() {
        return {
            hover: true
        }
    }
}
</script>

<style>
</style>
