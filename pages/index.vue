<template>
  <v-row justify="center" align="center">

           <pixi-renderer :w="800" :h="2000">
      <pixi-container
        :x="200" :y="200"
        msg="pixi container"
      >
        <pixi-sprite :x="400" :y="600" />
        <pixi-sheep :x="400" :y="1200" /> 
        <pixi-dog :x="400" :y="1600" /> 
      </pixi-container>
    </pixi-renderer>
  </v-row>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'
import PixiRenderer from "~/components/PixiRenderer";
import PixiContainer from "~/components/PixiContainer";
import PixiDog from "~/components/PixiDog";
import PixiSprite from "~/components/PixiSprite";
import PixiSheep from "~/components/PixiSheep";
  
export default {
  components: {
    Logo,
    VuetifyLogo,
    PixiRenderer,
    PixiContainer,
    PixiDog,
    PixiSprite,
    PixiSheep
  }
}
</script>
