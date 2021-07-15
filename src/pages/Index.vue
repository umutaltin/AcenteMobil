<template>
  <q-page class="text-grey-8 q-pa-md">
    <!-- User Name -->
    <section>
      <p class="q-ma-none" style="font-size: 16px">Hi Yavuz.</p>
      <p class="text-bold text-grey-10" style="font-size: 18px">Get In Shape</p>
    </section>
    <!-- Notifi Card -->
    <section>
      <q-card class="orange-card text-white">
        <q-card-section>
          <q-btn dense unelevated rounded style="background : #ffffff30" text-color="white" class="text-capitalize q-px-md" label="Entry Level" />
          <p class="q-mt-sm q-mb-none" style="font-size: 28px">Sholder Press</p>
          <p style="font-size: 16px; color : #ffffff90">
            16 sholder workout <br>
            vidios for you
          </p>
        </q-card-section>
        <q-card-section class="q-pt-none">
         <div class="round q-pa-xs inline-block" style="background : #ffffff30; border-radius : 60px">
            <q-icon name="play_circle_filled" color="white" size="xl" />
         </div>
         <span class="q-pa-sm" style="font-size : 16px">34 Minutes</span>
        </q-card-section>
        <div class="img" />
      </q-card>
    </section>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "PageIndex",
});
</script>

<style lang="scss">

.orange-card{
  background-color: $card-orange;
}

.img{
  position: absolute;
  background-image: url("../assets/travel.svg");
  background-size: 350px;
  background-repeat: no-repeat;
  bottom: -55px;
  right: -110px;
  width: 350px;
  height: 350px;
}

</style>



