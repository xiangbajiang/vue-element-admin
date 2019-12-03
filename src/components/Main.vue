<template>
    <div class="container">
        <tags />
        <div class="contents">
        <transition name="fade-transform" mode="out-in">
            <router-view></router-view>
        </transition>
        </div>
    </div>
</template>

<script>
import Tags from './Tags.vue'
export default {
    name: "Main",
    components:{
        Tags
    }
}
</script>
<style lang="css">
.container {
    height: calc(100vh - 50px);
    position: relative;
    overflow: hidden;
    width: 100%;
    overflow: hidden;
}
.container .contents{
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
}
</style>