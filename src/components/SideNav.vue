<template>
  <v-layout wrap style="height: 200px;">

    <v-navigation-drawer v-model="$store.state.drawer" absolute temporary>
      <v-list class="pa-1">
        <v-list-tile avatar>
          <v-list-tile-avatar>
            <img src="https://avatars2.githubusercontent.com/u/1363954?s=460&v=4">
          </v-list-tile-avatar>

          <v-list-tile-content>
            <v-list-tile-title>Tomoya Kamaji</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>

      <v-list class="pt-0" dense>
        <v-divider></v-divider>

        <v-list-tile v-for="item in items" :key="item.title" >
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>

          <v-list-tile-content>
            <v-list-tile-title>{{ item.title }}</v-list-tile-title>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
  </v-layout>
</template>

<script>
// コメント
export default {

  data () {
    return {
      
      items: [
        { title: '本社出勤', icon: 'list' }
      ]
    }
  }
}
</script>