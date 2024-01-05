<template>
 <NavCom/>
 
<router-view v-slot="{ Component }"> 
  <transition name="fadeUp" mode="out-in">
    <component :is="Component" :key="$route.path">

    </component>
  </transition>
</router-view>
<FooterCom/>
</template>

<script>
import NavCom from "@/components/NavCom.vue";
import FooterCom from "@/components/FooterCom.vue"
export default {
    name: "App",
    components: { NavCom, FooterCom }
}
</script>

<style>
#app {
  
  color: #2c3e50;
}

.fadeUp-enter-active
.fadeUp-leave-active{
  transition: opacity 0.25s, transform 0.25s;
}
.fadeUp-enter,
.fadeUp-leave-to{
  opacity: 0;
  transform: translateY(30%);
}

</style>
