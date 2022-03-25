<template>
  <div class="col-12 py-2 bg-info">
      <!-- <slot name="top"/> -->
      <!-- <slot></slot> default slot  -->
    <h4 class="alert text-center">
      Welcome in our app
      <!-- <p> {{branchname}} Branch </p> -->
      <!-- <p>Capacity: {{ branch.Capacity }}</p>
      <p>Tracks: {{ branch.tracks }}</p>
      <p
        :class="[
          branch.name == 'Mansoura' ? 'mansoura' : '',
          branch.name == 'Alexandria' ? 'alex' : '',
          branch.name == 'Smart' ? 'smart' : '',
        ]"
      >
        Name: {{ branch.name }}
      </p> -->
    </h4>
  </div>
</template>
<script>
export default {
  props: ["branch"],
  // data:()=>({

  // }),
  //    components:{

  //    }
  // components:{

  // }
};
</script>
<style>
.mansoura {
  color: red;
}
.alex {
  color: blue;
}
.smart {
  color: blueviolet;
}
</style>