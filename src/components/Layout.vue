<template>
  <v-app id="app" :dark="dark">
    <AsideBar/>
    <HeadToolsBar/>
    <v-content>
      <v-container fluid fill-height class="grey lighten-4">
        <v-layout justify-center align-center>
          <v-flex shrink>
            <v-tooltip right>
              <v-btn
                slot="activator"
                :href="source"
                icon
                large
                target="_blank"
              >
                <v-icon large>code</v-icon>
              </v-btn>
              <span>Source</span>
            </v-tooltip>
          </v-flex>
        </v-layout>
      </v-container>
    </v-content>
    <Footer/>
  </v-app>
</template>

<script>
    import AsideBar from './AsideBar'
    import Footer from './Footer'
    import HeadToolsBar from "./HeadToolsBar";

    export default {
        name: "Layout",
        components: {
          HeadToolsBar,
          Footer,
          AsideBar
        },
    }
</script>

<style scoped>

</style>
