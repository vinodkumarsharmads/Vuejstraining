<template>
  <div class="contact">
    <img alt="Vue logo" src="../assets/logo.png" />
    <ContactDetail :msg="msg" :data="data" />
  </div>
</template>
<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ContactDetail from "@/components/ContactDetail.vue"; // @ is an alias to /src

@Component({
  components: {
    ContactDetail
  }
})
export default class Contact extends Vue {
  data() {
      return {
        data:{
          Mobile:'9529653423',
          Email:'vinod@yoapmail.com',
          Address:'J5 DS'
        },
        msg:'Welcome to DS'
      }
  }
}
</script>
