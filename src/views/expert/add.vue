<template>
    <div class="app-container">
        <el-form ref="expert_form" :model="exp_info" label-width="100px">
            <el-form-item label="姓名" >
                <el-input v-model="exp_info.name_ch"></el-input>
            </el-form-item>
            <el-form-item label="英文名">
                <el-input v-model="exp_info.name_en"></el-input>
            </el-form-item>
            <el-form-item label="工作单位">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="职称">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="职业">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="最高学历">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="毕业院校">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="所学专业">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="性别">
                <el-radio-group v-model="exp_info.sex">
                    <el-radio label="男"></el-radio>
                    <el-radio label="女"></el-radio>
                </el-radio-group>
            </el-form-item>
            <el-form-item label="出生年份">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="国籍">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="民族">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="移动电话">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="办公电话">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="邮箱">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="政治面貌">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="籍贯">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="研究方向">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="推荐来源">
                <el-select v-model="exp_info.origin" placeholder="请选择推荐来源">
                    <el-option label="原专家库" value="原专家库"></el-option>
                    <el-option label="网信办" value="网信办"></el-option>
                    <el-option label="爬取" value="爬取"></el-option>
                    <el-option label="中心" value="中心"></el-option>
                </el-select>
            </el-form-item>
            <el-form-item label="状态">
                <el-select v-model="exp_info.status" placeholder="请选择专家状态">
                    <el-option label="新推荐专家" value="原专家库"></el-option>
                    <el-option label="入库专家" value="网信办"></el-option>
                    <el-option label="撤销专家" value="爬取"></el-option>
                </el-select>
            </el-form-item>
            <el-form-item label="部门">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="教授课程">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="所在地">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="邮编">
                <el-input v-model="exp_info.unit"></el-input>
            </el-form-item>
            <el-form-item label="技术标签" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="业务标签" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="工作经历" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="社会兼职" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="主要成就" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="教材" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="主要论文" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="主要专利" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="国家级项目" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item label="基金" prop="desc">
                <el-input type="textarea" v-model="exp_info.name"></el-input>
            </el-form-item>
            <el-form-item>
                <el-button type="primary" >立即创建</el-button>
            </el-form-item>
        </el-form>
    </div>
</template>
<script>
export default {
    name: "expert_add",
    data() {
        return {
            exp_info: {
                name_ch: "",
                name_en: "",
                sex: "",
                unit: "",
                origin: "",
                status: ""
            }
        }
    },
    methods: {
       
    }
}
</script>
<style lang="css">
    .app-container{
        padding: 20px 10px;
        text-align: left;
        overflow: hidden;
    }
    .app-container .el-form .el-form-item{
        width: 100%;
    }
    .app-container .el-form .el-form-item .el-input{
        width: 200px;
    }
    .app-container .el-form .el-form-item .el-textarea{
        width: 400px;
    }
    .app-container .el-form-item__label{
        color: black;
    }
</style>