<script setup>
import search from './search.vue';
import { HomeOutlined, SolutionOutlined ,LoginOutlined,LogoutOutlined,EditOutlined} from '@ant-design/icons-vue';
</script>

<template>
    <nav class="container">

        <div id="blog-info">
            <a href="/">
                <span class="site name">Gen-Blog</span>
            </a>
        </div>

        <div id="menus">
            <span id="search-button">
                <search></search>
            </span>
            <span id="menus-items">
                <span>
                    <home-outlined />首页
                </span>
                <span><solution-outlined />个人主页</span>
                <span><edit-outlined />创作中心</span>
                <span><login-outlined />登录</span>
                <span><logout-outlined />注册</span>
            </span>
        </div>
    </nav>
    
</template>


<style>
.container {
    display: flex;
    height: 60px;
    margin: 0;
    padding: 0;
    align-items: center
}

#blog-info {
    font-size: 1.5em;
    font-weight: bold;
    width: 25%;
    margin: 0 .5em;
}

#menus {
    display: flex;
    justify-content: flex-end;
    width: 70%;
    align-items: center;
    font-size:1.1em
}

span {
    margin: 0 .5em;
}

a {
    color: var(--light-grey);
}
</style>