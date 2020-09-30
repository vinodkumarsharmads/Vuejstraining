<template>
     <div class="containt">
        <div class="row">
        	<div class="col-md-12">
                
                    <category :list="CateList" />
            </div>
        </div>
        
    </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import axios from "axios";
import category from "@/components/category.vue"; // @ is an alias to /src

@Component({
  components: {
    category
  }
}) 
export default class Home extends Vue {
  data() {
      return {
        CateList:[
          {
            "img": "img/cat_social.png",
            "name": "SOCIAL",
            "description": "Feds open formal probe into Tesla electric ship"
          },
          {
            "img": "img/technology.png",
            "name": "TECHNOLOGY",
            "description": "Nielsen forecasts smaller Black Friday crowds"
          },
          {
            "img": "img/business.png",
            "name": "BUSINESS",
            "description": "Butterball talks turkey Fewer fresh birds this"
          },
          {
            "img": "img/sports.png",
            "name": "SPORTS",
            "description": "Premier League: the race for the title (and Europe)"
          }
        ]
      }
  }
}
</script>
