<template>
    <div>
        <van-sticky :offset-top="0">
            <!-- header -->
            <div class='header'>
                <input type="text" class="search" placeholder="请输入商家或商品名称">
            </div> 
        </van-sticky>
        <category></category>
        <div class="title-box">附近商家</div>
    </div>
</template>

<script>
import category from './category'
    export default {
        components:{
            category,
        }
    }
</script>

<style lang="scss" scoped>
    .header{
        background-color: #1c1b20;
        padding: 0.2rem;
        .search{
            width: 100%;
            border: none;
            height: 0.6rem;
            line-clamp: 0.6rem;
            border-radius: 0.3rem;
            padding: 0 0.2rem;
            box-sizing: border-box;
        }
    }
    .title-box{
        font-size: 0.34rem;
        font-weight: 800;
        text-align: center;
        margin: 0.3rem 0 0.1rem;
        height: 0.46rem;
        line-height: 0.46rem;
    }
</style>