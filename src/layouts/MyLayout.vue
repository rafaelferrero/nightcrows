<template>
    <q-layout view="lHh Lpr lff">
      <q-header reveal elevated class="bg-primary glossy">
        <q-toolbar>
          <q-btn flat @click="drawer = !drawer" round dense icon="menu" />
          <q-toolbar-title>Nightcrows</q-toolbar-title>
         </q-toolbar>
      </q-header>
      <q-footer reveal elevated class="bg-primary">
        <q-toolbar>
          <q-toolbar-title>We are the Night Crows Crew !!!</q-toolbar-title>
          <div><small>Powered by</small> Quasar v{{ $q.version }}</div>
        </q-toolbar>
      </q-footer>

      <q-drawer
          v-model="drawer"
          content-class="bg-accent"
          side="left"
          behavior="mobile"
          overlay
      >
        <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px;">
          <q-list padding>
            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="home" />
              </q-item-section>

              <q-item-section>
                Back Home
              </q-item-section>
            </q-item>
            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="star" />
              </q-item-section>

              <q-item-section>
                Our Blog
              </q-item-section>
            </q-item>
            <q-item clickable v-ripple>
              <q-item-section avatar>
                <q-icon name="email" />
              </q-item-section>

              <q-item-section>
                Contact us!
              </q-item-section>
            </q-item>
          </q-list>
        </q-scroll-area>

        <q-img class="absolute-top bg-primary center" style="height: 150px">
          <div class="absolute-center text-center bg-transparent">
            <q-avatar size="90px" class="q-mb-sm">
              <img src="~assets/images.png">
            </q-avatar>
            <div class="text-weight-bold">@nightcrows</div>
          </div>
        </q-img>
      </q-drawer>

      <q-page-container>
        <router-view />
      </q-page-container>
    </q-layout>
</template>

<script>
export default {
  name: 'MyLayout',

  data () {
    return {
      drawer: false
    }
  }
}
</script>
