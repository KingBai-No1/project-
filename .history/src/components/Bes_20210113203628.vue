<!--  -->
<template>
<!-- 外部容器 -->
    <el-container class="box">
        <el-header>head</el-header>
        <el-container class="pag">
            <el-aside style="width:200px">Aside</el-aside>
            <el-main><main></main></el-main>
        </el-container>    
        <el-footer>foot</el-footer>
    </el-container>
</template>

<script>
export default {
    data () {
        return {
    };
    },

    components: {},

    computed: {},

    mounted(){},

    methods: {}
}

</script>
<style  scoped>

.box{
    width: 100vw;
    height: 100vh;
}
.el-header{
    background-color: skyblue;
}
.pag{
    background-color: gray;
}
.el-footer{
    background-color: #B3C0D1;
}
</style>