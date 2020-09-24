<template>
  <v-app>
    <v-toolbar app>
      <v-toolbar-side-icon @click="openSideMenu"></v-toolbar-side-icon>
      <v-toolbar-title class="headline text-uppercase">
        <span>カレンダーアプリ</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
    </v-toolbar>
    <SideNav/>


    <v-content>
    </v-content>
  </v-app>
</template>

<script>
import SideNav from './components/SideNav'
export default {
  name: 'App',
  components: {
    SideNav
  },
  data () {
    return {
      //
    }
  },
  methods:{
    openSideMenu(){
      this.$store.dispatch('toggleSideMenu')
    }
  }
}
</script>
