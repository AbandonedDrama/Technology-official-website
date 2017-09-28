<template lang="html">
    <div id="frame">
        <topNavMenu></topNavMenu>
    </div>
</template>

<script>
import topNavMenu from './components/Public/topNavMenu.vue'
export default {
    name: 'frame',
    data() {
        return {
            msg: 'Welcome to Your Vue.js App'
        }
    },
    components: { topNavMenu }
}
</script>

<style lang="scss">
*{
    margin: 0;
    padding: 0;
}
#frame {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
}

h1,
h2 {
    font-weight: normal;
}

ul {
    list-style-type: none;
    padding: 0;
}

li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: #42b983;
}
</style>
