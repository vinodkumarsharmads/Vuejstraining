<template>
  <div class="category">
    <div class="row">
      <div v-for="cat in list" :key="cat.name" class="col-sm-6 col-md-12 dis_block">
        <div class="cat_item_box">
          <img :src="cat.img" alt />
          <span class="cat-name b_yellow">{{cat.name}}</span>
          <span class="cat-lines">
            <a href="#" class="yellow">
              {{cat.description}}
              <span class="bar"></span>
            </a>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class category extends Vue {
  @Prop() private list!: Array<any>;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="stylus"></style>
