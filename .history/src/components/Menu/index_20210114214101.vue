<!--  -->
<template>
    <div>
        <h2>菜单管理页面</h2>
        <el-table :data="arr">
            <el-table-column label="编号" prop="id"></el-table-column>
        </el-table>
    </div>
</template>

<script>
import axios from 'axios';
export default {
    data () {
        return {
            arr:[]
    };
    },

    components: {},

    computed: {},

    mounted(){
        axios.get("/api/menulist").then((res)=>{
            // console.log(res);拿到了数据
            this.arr.push(res.data.list)
            console.log(this.arr);
        })
    },

    methods: {}
}

</script>
<style  scoped>
</style>