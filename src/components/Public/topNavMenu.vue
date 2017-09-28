<template lang="html">
    <div id="topNavMenu">
        <div class="wrap">
            <el-row type="flex" justify="space-between">
                <el-col :span="4">
                    <img src="src\assets\imgs\logo\1464062976.png" alt="LOGO">
                </el-col>
                <el-col :span="7">
                    <el-menu :default-active="activeIndex" class="el-menu-demo" mode="horizontal" @select="handleSelect">
                        <el-menu-item index="1">首页</el-menu-item>
                        <el-submenu index="2">
                            <template slot="title">产品</template>
                            <el-menu-item index="2-1">CPU</el-menu-item>
                            <el-menu-item index="2-2">RAM</el-menu-item>
                        </el-submenu>
                        <el-menu-item index="3">支持</el-menu-item>
                        <el-menu-item index="4">关于</el-menu-item>
                    </el-menu>
                </el-col>
            </el-row>
        </div>
    </div>
</template>

<script>
export default {
    name: 'topNavMenu'
}
</script>

<style lang="sass">
#topNavMenu
    width: 100%
    height: 60px
    .wrap
        max-width: 1200px
        height: 60px
        margin: 0 auto
        .el-row
            height: 100%
            .el-col
                height: 100%
                img
                    height: 100%
                    width: auto
                .el-menu
                    background: #fff
                    .el-menu-item, .el-submenu__title
                        color: #333
</style>
