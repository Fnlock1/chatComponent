<template>
<div class="headCard"
     v-for="item in 7"
     :class="{
         'end' : item % 2 === 0
     }"
>
<!--    头部-->
    <div class="headImg">
        <img src="https://avatars.githubusercontent.com/u/81659426?v=4"
             alt="">
    </div>

<!--    消息内容-->
    <div
        class="headCardMsg"
    >现在很多APP在用户截图时会自动提示用户是否要进行分享。这个时机确实抓的很棒，一般来说，用户截图大多数时候都是为了分享给他人，少部分是为了留底备份。
        分享时机，在不同的时机分析用户是否有分享的意愿，提供给他们合适的分享内容，能让分享的效果更好。
        在常用的社交分享组件中，微信（微信好友和朋友圈）、微博、QQ（QQ好友和QQ空间）是三大主要平台，而其中微信凭借高达9.38亿的月活跃用户以及高达29%的日均手机应用使用率，成为各款APP选择最多、排位最靠前的分享途径。即便同样是腾讯系下的QQ，也在QQ空间中加入了分享到微信好友和朋友圈的功能。
        我们从分享时机、分享形式、分享动机、分享场景4个维度来聊聊「社交分享」的那些事儿。
        用户分享内容到社交媒体或好友，不应该是一种粗暴的强制行为，我们应该在保证产品本身内容有吸引力的核心前提下，仔细揣摩用户心理，结合产品本身的特色，在不同情境下提供给用户最合适的分享平台及方式，让用户分享成为一种水到渠成的自然行为，甚至在某些时候还能给用户带来一些小的惊喜就更棒了。
        下面我们...</div>
</div>
</template>

<script setup>
import {ref} from "vue";

let user = ref(1);
</script>


<style >
body{
    background: #9ca3af;
}
.headCard{
    display: flex;
    width: 100%;
    flex-wrap: nowrap;
}
.headImg{
    width: 50px;
    height: 50px;
}
.headImg * {
    width:100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
}

.headCardMsg{
    width: 50%;
/*    超过五行 省略*/
    overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-line-clamp: 5;
    -webkit-box-orient: vertical;
    background: white;
    border-radius: 10px;
    padding: 4px;
    margin-top: 20px;
    margin-left: 10px;
    font-size: 14px;
}

.end{
    flex-direction: row-reverse;
}
</style>
