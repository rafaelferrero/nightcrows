<template>
    <q-page class="flex flex-center">
        <img alt="Background" src="~assets/Crows-at-Night-15001.jpg">

        <div class="q-pa-md fit row items-start q-gutter-md">
            <div class="col">
            <q-card class="my-card">
                <q-item>
                    <q-item-section avatar>
                        <q-avatar>
                            <img src="https://cdn.quasar.dev/img/avatar2.jpg">
                        </q-avatar>
                    </q-item-section>

                    <q-item-section>
                        <q-item-label>Title</q-item-label>
                        <q-item-label caption>Subhead</q-item-label>
                    </q-item-section>
                </q-item>
                <img src="https://cdn.quasar.dev/img/parallax2.jpg">
            </q-card>
            </div>
            <div class="col">
            <q-card class="my-card">
                <q-item>
                    <q-item-section avatar>
                        <q-avatar>
                            <img src="https://cdn.quasar.dev/img/avatar2.jpg">
                        </q-avatar>
                    </q-item-section>

                    <q-item-section>
                        <q-item-label>Title</q-item-label>
                        <q-item-label caption>Subhead</q-item-label>
                    </q-item-section>
                </q-item>

                <img src="https://cdn.quasar.dev/img/parallax2.jpg">
            </q-card>
            </div>
            <div class="col">
            <q-card class="my-card">
                <q-item>
                    <q-item-section avatar>
                        <q-avatar>
                            <img src="https://cdn.quasar.dev/img/avatar2.jpg">
                        </q-avatar>
                    </q-item-section>

                    <q-item-section>
                        <q-item-label>Title</q-item-label>
                        <q-item-label caption>Subhead</q-item-label>
                    </q-item-section>
                </q-item>

                <img src="https://cdn.quasar.dev/img/parallax2.jpg">
            </q-card>
            </div>
        </div>
          <q-page-scroller position="bottom-right" :scroll-offset="150" :offset="[18, 18]">
            <q-btn fab icon="keyboard_arrow_up" color="accent" />
          </q-page-scroller>
    </q-page>
</template>

<script>
export default {
  name: 'PageIndex'
}
</script>
