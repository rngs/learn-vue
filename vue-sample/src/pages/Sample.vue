<template>
  <div class="container">
    <Breadcrumb :items="breadcrumb" />
  </div>
</template>

<script>
  import Breadcrumb from "./common/snipets/breadcrumb/Breadcrumb";

  export default {
    components: {
      Breadcrumb
    },
    data() {
      return {
        breadcrumb: [
          {
            text: 'Admin',
            href: '#'
          },
          {
            text: 'Manage',
            href: '#'
          },
          {
            text: 'Library',
            active: true
          }
        ]
      }
    }
  };
</script>

<style>
</style>
