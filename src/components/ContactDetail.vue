<template>
  <div class="ContactDetail">
    <h1>{{ msg }}</h1>
    <p v-for="(value, index) in data">
      {{index}} : {{ value }}
    </p>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class ContactDetail extends Vue {
  @Prop() private msg!: string;
  @Prop() private data!: [];
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus">
h3
  margin 40px 0 0

ul
  list-style-type none
  padding 0

li
  display inline-block
  margin 0 10px

a
  color #42b983
</style>
