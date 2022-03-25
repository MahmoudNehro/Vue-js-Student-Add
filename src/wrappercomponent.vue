<template>
  <div class="container my-1">
    <div class="row g-0">
      <div class="col-12 py-2">
        <!-- <headercomponent :branch="{ name: 'Smart', Capacity: 1000, tracks: 5 }"> -->
          <!-- inject html from wrapper to child using slots-->
          <!-- <template v-slot:top> -->
            <!-- <h5 class="text-center">Information technology institute</h5> -->
          <!-- </template> -->
        <headercomponent/>
      </div>
    </div>
    <div class="row g-0 my-1">
      <div class="col-4">
        <linkscomponent />
      </div>
      <div class="col-8">
        <bodycomponent />
      </div>
    </div>
    <div class="row g-0">
      <div class="col-12 text-light p-2 bg-secondary"><footercomponent /></div>
    </div>
  </div>
</template>
<script>
import Bodycomponent from "./components/bodycomponent.vue";
import Footercomponent from "./components/footercomponent.vue";
import headercomponent from "./components/headercomponent.vue";
import Linkscomponent from "./components/linkscomponent.vue";
// import headercomponent from './components/headercomponent.vue';
// import headercomponent from "./components/headercomponent.vue";
export default {
  components: {
    headercomponent,
    Linkscomponent,
    Bodycomponent,
    Footercomponent,
  },
};
</script>