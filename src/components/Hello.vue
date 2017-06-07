<template>
    <div class="main-wrapper">
        <div class="title">
            <div class="nav-logo-wrapper">
                <img src="../../static/img/rxxt_03.png" width="30" height="20" alt="">
            </div>
            <span>绿茵乳腺关爱社区</span>
        </div>
        <div class="logo-wrapper">
            <img src="../../static/img/rxxt_06.png" width="100%" height="150" alt="">
        </div>
        <div class="tab-wrapper">
            <div class="tab-item tab-bb">
                <div class="tab-img">
                    <img src="../../static/img/rxxt_09.png" width="60" height="50" alt="">
                </div>
                <span class="tab-font">健康教育</span>
            </div>
            <div class="tab-item">
                <div class="tab-img">
                    <img src="../../static/img/rxxt_11.png" width="50" height="50" alt="">
                </div>
                <span class="tab-font">专业课程</span>
            </div>
        </div>
        <div class="content-wrapper">
            <!-- <router-link :to="{name:'content',params:{'contentItem',content}}" tag="div" class="content-item">
                <img :src="" alt="">
            </router-link> -->
        </div>
    </div>
</template>
<script>
import Data from '../../data.json';
console.log(Data);
export default {
    data() {
        return {
            content: Data
        }
    }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-wrapper .title {
    height: 58px;
    line-height: 58px;
    font-size: 16px;
    color: #333;
}

.main-wrapper .title .nav-logo-wrapper {
    box-sizing: border-box;
    float: left;
    padding-left: 10px;
    margin-top: -3px;
}

.main-wrapper .title .nav-logo-wrapper img {
    vertical-align: middle;
}

.logo-wrapper {
    width: 100%;
    height: 150px;
    overflow: hidden;
}

.tab-wrapper {
    display: flex;
    margin-top: 20px;
    font-size: 14px;
}

.tab-wrapper .tab-item {
    flex: 1;
    padding-bottom: 10px;
    border-bottom: 1px solid rgba(175, 175, 175, .15);
}

.tab-wrapper .tab-item .tab-img {
    margin-bottom: 3px;
}

.tab-wrapper .tab-item.tab-bb {
    color: #dd328d;
    border-bottom: 1px solid #dd328d;
}
</style>
