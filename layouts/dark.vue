<template>
    <div :class="$style.dark">
        <ReadexSidebar></ReadexSidebar>
        <Nuxt />
    </div>
</template>

<script>
import Vue from "vue";

import ReadexSidebar from "../components/main/ReadexSidebar.vue";

export default {
    components: {
        ReadexSidebar,
    },
};
</script>

<style module src="./dark.less" lang="less"></style>
