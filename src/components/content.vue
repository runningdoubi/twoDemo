<template>
    <div class="main-wrapper">
        <div class="img-wrapper">
            <img :src="contentItem.image" alt="" width="100%">
        </div>
        <div class="content-wrapper">
        	<h3 class="title">{{contentItem.content1Title}}</h3>
        	<p class="content">{{contentItem.content1}}</p>
        	<h3 class="title" v-if="contentItem.content2Title != ''">{{contentItem.content2Title}}</h3>
        	<p class="content" v-if="contentItem.content2 != ''">{{contentItem.content2}}</p>
        </div>
    </div>
</template>
<script type="text/javascript">
export default {
    data() {
            return {
                contentItem: {}
            }
        },
        created() {
            this.contentItem = this.$route.params.contentItem;
        }
}
</script>
<style rel="stylesheet" scoped>
.img-wrapper {
    width: 100%;
    height: 190px;
    font-size: 0;
}
.content-wrapper{
	text-align: left;
	padding: 0 10px 0 10px;
}
.content-wrapper .content{
	text-indent: 2em;
	line-height: 1.8;
}
</style>
