<template>
    <div class="container">
        <div :class="$style.red"></div>
    </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
    layout: "dark",
});
</script>

<style module src="./index.less" lang="less"></style>
