<template>
    <div class="wrapper">
        <div class="left">
            <text class="leftTxt" v-if="leftBtn">{{leftBtn.name}}</text>
        </div>
        <text class="tlt">{{title}}</text>
        <div class="right">
            <text class="rightTxt" v-if="rightBtn">{{rightBtn.name}}</text>
        </div>
    </div>
</template>
<script>
export default {
    props: ['title', 'leftBtn', 'rightBtn'],
}
</script>
<style scoped>
.wrapper {
    height: 70px;
    background-color: #fafafa;
    opacity: .99;
    flex-wrap: nowrap;
    flex-direction: row;
    justify-content: space-around;
    border-bottom-width: 1px;
    border-bottom-color: #d9d9d9;
}

.tlt {
    flex: 1;
    font-size: 36px;
    padding-top: 10px;
    color: #333;
    text-align: center;
}

.left,
.right {
    height: 80px;
    width: 120px;
    padding-top: 10px;
}

.leftTxt,
.rightTxt {
    font-size: 30px;
    text-align: center;
}
</style>