<template>
    <header :class="cx('wrapper')">
        <div :class="cx('inner')">
            <div :class="cx('logo')">
                <img src="@/assets/images/logo.svg" alt="" />
            </div>
            <div :class="cx('search')">
                <input type="text" placeholder="Search accounts and videos" />
                <button>
                    <font-awesome-icon :icon="faCircleXmark" />
                </button>
                <button :class="cx('search-btn')">
                    <i class="fa-light fa-magnifying-glass"></i>
                </button>
            </div>
            <div :class="cx()"></div>
        </div>
    </header>
</template>
<script setup>
import classNames from "classnames/bind";
import styles from "@/assets/css/Header/Header.module.scss";

const cx = classNames.bind(styles);
</script>

<script>
import FontAwesomeIcon from "@fortawesome/vue-fontawesome"
import { faCircleXmark } from "@fortawesome/free-solid-svg-icons";
export default {
    name: "HeaderItem",
    components: {
        FontAwesomeIcon,
    },
};
</script>
