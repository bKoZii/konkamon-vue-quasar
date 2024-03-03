<template>
  <div class="full-width row wrap justify-around items-center content-center q-mb-lg">
    <div class="col-5">
      <h3 class="q-my-md text-weight-bold">กรกมล ศรีอ่อน</h3>
      <p class="text-subtitle2">สวัสดีค้าบ ท่านสมาชิก ชมรมคนชอบ Vue วันพระวันเจ้าไม่เว้นกันเลย อยากจะเขียนแต่
        Vue<br>ไม่เข้าใจจริงๆ เลย ตะโกนหา สรรหาแต่ Vue เป็นอะไรกัน เห้ย! ทั้งวันเลยวันนี้ ไปเรียน มีแต่ Vue
        โผล่มาทั้งวันเลย เขียนไปแล้วก็ยังจะอยากเขียนอีก มันหมายความว่าอะไร คนที่ไหนคนจังหวัดอะไรพวกท่านเนี่ย หืม?.....
        <q-btn label="อ่านต่อ" color="primary" text-color="black" padding="3px" @click="QBarDialog = true" />
      </p>
      <q-separator spaced color="primary" />
      <p class="text-body1">Powered by <span class="text-primary">Vue</span> / <span class="text-blue-5">Quasar</span>
        !!</p>
    </div>
    <div class="col-auto">
      <q-img :src="'me-rmutsv.jpg'" spinner-color="white" width="10em" height="auto" :ratio="4 / 5"
        class="rounded-borders" />
    </div>
  </div>
  <q-dialog v-model="QBarDialog" persistent draggable>
    <q-card>
      <q-bar>
        <q-btn dense flat round icon="lens" size="8.5px" color="red" @click="QBarDialog = false" />
        <q-btn dense flat round icon="lens" size="8.5px" color="dark" />
        <q-btn dense flat round icon="lens" size="8.5px" color="dark" />
        <div class="col text-center text-weight-medium">
          ชมรมคนชอบ Vue
        </div>

      </q-bar>


      <q-card-section id="cardSection">
        <p>
          สวัสดีค้าบ ท่านสมาชิก ชมรมคนชอบ Vue วันพระวันเจ้าไม่เว้นกันเลย อยากจะเขียนแต่
          Vue ไม่เข้าใจจริงๆ เลย ตะโกนหา สรรหาแต่ Vue เป็นอะไรกัน เห้ย! ทั้งวันเลยวันนี้ ไปเรียน มีแต่ Vue
          โผล่มาทั้งวันเลย เขียนไปแล้วก็ยังจะอยากเขียนอีก มันหมายความว่าอะไร คนที่ไหนคนจังหวัดอะไรพวกท่านเนี่ย หืม?</p>
        <p>
          เฮ้ยตายแล้ว! ศึกษาวิชาอื่นมั่งดิ วิชา <span class="text-blue-5">Data Structure, สัมมนา, Cloud App,
            ประมวลผลภาพ,
            วิศวกรรมซอฟต์แวร์</span>
          ศึกษาเป็นบ้างหรือเปล่า เขียนแต่ Vue ใกล้ปลายภาคแล้วนะ Vue ละเขียนทั้งวันทั้งคืนเลย
          ไม่เข้าใจเลยพวกท่านเป็นยังไง
          จัดมาดิ ขอเว็บแบบเบิ้มๆ ล่ะน่ะ คือลือน่ะ
          เฮ้ยคนที่ไหนพวกท่านเป็นคนจังหวัดอะไรเกิดวันไหนเกิดปีไหนเกิดปีจอหรือปีอะไรครับผมไม่เข้าใจ ตายแล้วว
          นั่งเรียนทั้งวันละ
          Vue โผล่มาทั้งวันเลย55555 ผมไม่เข้าใจจริงๆ เลย โอ้ยตายแล้วพวกท่านมวยกูมาละลาก่อน เขียน Vue ไปก่อนผมจะดูมวย
        </p>
      </q-card-section>
    </q-card>
  </q-dialog>

</template>

<script setup lang="ts">
import { ref } from 'vue';

const QBarDialog = ref(false);
</script>

<style>
.indexHero {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  align-items: center;
}

p.text-subtitle2,
#cardSection p {

  text-indent: 3em;
  word-wrap: break-word;
}
</style>
