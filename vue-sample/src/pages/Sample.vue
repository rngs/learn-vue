<template>
  <div class="container">
    <Breadcrumb :items="breadcrumb" />
  </div>
</template>

<script>
  import { breadcrumb } from "./scripts/data";

  import Breadcrumb from "./common/snipets/breadcrumb/Breadcrumb";

  export default {
    components: {
      Breadcrumb
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
