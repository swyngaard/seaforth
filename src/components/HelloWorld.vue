<template>
  <div>
    <b-jumbotron>
      <template v-slot:header>BootstrapVue</template>

      <template v-slot:lead>
        This is a simple hero unit, a simple jumbotron-style component for calling extra attention to
        featured content or information.
      </template>

      <hr class="my-4">

      <p>
        It uses utility classes for typography and spacing to space content out within the larger
        container.
        {{ msg }}
      </p>

      <b-button v-b-modal.my-modal variant="primary" href="#">Show Modal</b-button>
      <b-button variant="success" href="#">Do Something Else</b-button>
      <b-modal id="my-modal">Hello From My Modal!</b-modal>
    </b-jumbotron>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
