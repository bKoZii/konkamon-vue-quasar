<template>
  <h3 class="text-weight-bold">Tech Stack</h3>
  <div class="fit row wrap justify-start items-start content-start q-col-gutter-sm">
    <div class="col-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
      <q-card class="my-card" flat>
        <q-img src="/vue.jpg">
          <div class="absolute-bottom ">
            <!-- <q-item>
              <q-item-section>
                <q-item-label class="text-h6">Vue.JS</q-item-label>
              </q-item-section>
              <q-item-section side center>
                <q-icon name="home" color="primary" href="ddd" />
              </q-item-section>
            </q-item> -->
            <q-toolbar class="text-white q-pa-none">
              <!-- <q-btn flat round dense icon="assignment_ind" /> -->
              <q-toolbar-title class="text-h6">
                Vue.JS
              </q-toolbar-title>
              <q-btn flat round dense icon="home" class="q-mr-xs" href="https://vuejs.org" target="_blank" />
            </q-toolbar>
            <!-- Vue.js -->

          </div>
        </q-img>

        <q-card-section>
          <p>Vue เป็น Front-End Progressive Framework ที่จะเน้นในการสร้าง User Interface โดยจะมีหน้าที่เป็น View ใน
            MVC(Model View Controller)</p>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
      <q-card class="my-card" flat>
        <q-img src="/quasar.jpg">
          <div class="absolute-bottom text-h6">
            <q-toolbar class="text-white q-pa-none">
              <!-- <q-btn flat round dense icon="assignment_ind" /> -->
              <q-toolbar-title class="text-h6">
                Quasar
              </q-toolbar-title>
              <q-btn flat round dense icon="home" class="q-mr-xs" href="https://quasar.dev" target="_blank" />
            </q-toolbar>
          </div>
        </q-img>
        <q-card-section>
          <p class="text-body2">Quasar เป็น UI Framework ที่มีพื้นมาจาก Vue และยังรองรับแอปหลากหลายรูปแบบ เช่น SPA,
            SSR, PWAs, Mobile App
            และอื่นๆ
          </p>
        </q-card-section>
      </q-card>
    </div>
    <div class="col-4 col-lg-4 col-md-4 col-sm-12 col-xs-12">
      <q-card class="my-card" flat>
        <q-img src="/firebase.jpg">
          <div class="absolute-bottom text-h6">
            <q-toolbar class="text-white q-pa-none">
              <!-- <q-btn flat round dense icon="assignment_ind" /> -->
              <q-toolbar-title class="text-h6">
                Firebase
              </q-toolbar-title>
              <q-btn flat round dense icon="home" class="q-mr-xs" href="https://firebase.google.com" target="_blank" />
            </q-toolbar>
          </div>
        </q-img>

        <q-card-section>
          <p>Firebase เป็น Platform ที่รวบรวมเครื่องมือต่างๆ สำหรับการจัดการในส่วนของ Server side
            ซึ่งทำให้สามารถพัฒนา Web Application ได้อย่างมีประสิทธิภาพ</p>
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.q-img__content>div {
  padding: 0 15px;
}
</style>
