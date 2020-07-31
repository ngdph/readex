<template>
    <div :class="$style.sidebar">
        <a-menu
            style="width: 250px;"
            :default-selected-keys="['1']"
            :open-keys.sync="openKeys"
            mode="inline"
            @click="handleClick"
            theme="dark"
            :class="$style.menu"
        >
            <a-menu-item :class="$style.item" key="1">
                Load book
            </a-menu-item>
            <!-- <a-menu-item :class="$style.item" key="2">
                Option 2
            </a-menu-item>
            <a-menu-item :class="$style.item" key="3">
                Option 3
            </a-menu-item> -->
        </a-menu>
    </div>
</template>

<script lang="ts">
import Vue from "vue";

export default {
    data() {
        return {
            current: ["mail"],
            openKeys: ["sub1"],
        };
    },
    watch: {
        openKeys(val: any) {
            console.log("openKeys", val);
        },
    },
    methods: {
        handleClick(e: any) {
            console.log("click", e);
        },
        titleClick(e: any) {
            console.log("titleClick", e);
        },
    },
};
</script>

<style module src="./ReadexSidebar.less" lang="less"></style>
