<template>
  <div class="container">
    <Breadcrumb :items="breadcrumb" />

    <main>
      <Conditions />
    </main>
  </div>
</template>

<script>
  import { breadcrumb } from "./scripts/data";

  import Breadcrumb from "./common/snipets/breadcrumb/Breadcrumb";
import Conditions from "./contents/Conditions.vue";

  export default {
    components: {
      Breadcrumb,
      Conditions
    },
    data() {
      return {
        breadcrumb
      }
    }
  };
</script>

<style>
</style>
