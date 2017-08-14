<template>
    <div id="app">
        <md-toolbar>
            <h1 class="md-title">
                <img src="./assets/img/PaperNote.png" alt="Logo">
                PaperNote
            </h1>
        </md-toolbar>
        <router-view></router-view>
    </div> <!-- #app -->
</template>

<script type="text/javascript">
// Import Material UI component
import Vue from 'vue'
import VueMaterial from 'vue-material'
Vue.use(VueMaterial)

// Import essential CSS
import 'vue-material/dist/vue-material.css'
import 'material-design-icons/iconfont/material-icons.css'
import 'roboto-fontface/css/roboto/roboto-fontface.css'

// Create theme for Material component
Vue.material.registerTheme({
    default: {
        primary: {
            color: 'light-green',
            hue: 700
        },
        accent: {
            color: 'teal',
            hue: 100
        }
    }
})

export default {
    name: 'app'
}
</script>

<style type="text/css">
    h1.md-title img {
        max-height: 36px;
    }
</style>
