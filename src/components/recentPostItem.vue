<script setup>
import {FieldTimeOutlined,ContainerOutlined} from '@ant-design/icons-vue'
</script>

<template>
    <div class="recent-post-item">
        <div class="post-cover-left">
            <a href="/" >
                <img src="./icons/butterfly-docs-01-cover.png" alt="" class="post-img">
            </a>
        </div>
        <div class="recent-post-info">
            <a href="" class="article-title">Gen-Blog使用文檔(一) 快速開始</a>
            <div class="artical-meta-wrap">
                <span class="post-meta-date">
                    |<field-time-outlined />发表于 2023-05-06
                </span>
                <span class="post-kinds">
                    |<container-outlined /> 教程类
                </span>
            </div>
            <div class="content">
                本教程更新於 2023 年 04 月 10 日，教程的內容針對最新穩定版而更新（如果你是舊版，教程會有些出入，請留意）
            </div>
        </div>
    </div>
</template>

<style>
.recent-post-item{
    display: flex;
    flex-direction: row;
}
.post-cover-left {
    overflow: hidden;
    width: 44%;
    height: 100%;
    box-sizing: border-box;
}

.recent-post-info {
    padding: 0 40px;
    width: 57%;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: white;
    text-align: center;
}

.post-img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.article-title{
    font-size: 2em;
}

.recent-post-item{
    box-sizing: border-box;
    border-radius: 8px;
    background: var(--card-bg);
    margin-top: 20px;
    box-shadow: 3px 3px 3px rgb(232, 226, 226);
    
}

.artical-meta-wrap{
    color:#858585
}
</style>