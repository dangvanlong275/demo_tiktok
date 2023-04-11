<template>
    <div :class="cx('wrapper')">
        <div :class="cx('container')">
            <sidebar-item/>
            <div :class="cx('content')">
                <slot></slot>
            </div>
        </div>
    </div>
</template>
<script setup>
import classNames from "classnames/bind";
import styles from "@/assets/css/Header/DefaultLayout.module.scss";

const cx = classNames.bind(styles);


</script>

<script>
import SidebarItem from "./Sidebar/Sidebar.vue"

export default {
    name: "DefaultLayout",
    components: {
        SidebarItem
    }
}
</script>