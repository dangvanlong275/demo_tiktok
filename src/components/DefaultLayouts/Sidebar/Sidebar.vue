<template>
    <aside :class="cx('wrapper')">
        <h2>Sidebar</h2>
    </aside>
</template>
<script setup>
import classNames from "classnames/bind";
import styles from "@/assets/css/DefaultLayouts/Sidebar.module.scss";

const cx = classNames.bind(styles);


</script>

<script>
export default {
    name: "SidebarItem"
}
</script>