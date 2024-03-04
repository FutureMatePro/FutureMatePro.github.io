<template>
  <div class="home text-center">

    <div>测试123</div>
    <div class="hua">
      <img src="@/assets/img/hua.svg" id="animat" />
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
export default defineComponent({
  name: "HomePgae",
  components: {
    HelloWorld,
  },
  data() {
    return {

    };
  },
  methods: {
    changeColor() {

    },
    handleClick() {

    },
    initTime() {

    },
  },
  created() {

  },
  beforeUnmount() {

  },
});
</script>

<style>
.home{
  width: 100%;
  height: 100%;
}
.hua{
  width: 85.3333%;
  height: auto;
  position: absolute;
  left: 7.99167%;
  top: 23.4597%;

}
#animat{
  position:relative;
  animation:mymove 5s infinite;
  -webkit-animation:mymove 5s infinite; /*Safari and Chrome*/
  animation-direction:alternate;/*轮流反向播放动画。*/
  animation-timing-function: ease-in-out; /*动画的速度曲线*/
  /* Safari 和 Chrome */
  -webkit-animation:mymove 5s infinite;
  -webkit-animation-direction:alternate;/*轮流反向播放动画。*/
  -webkit-animation-timing-function: ease-in-out; /*动画的速度曲线*/
}
@keyframes mymove
{
  0%{
    transform: scale(1);  /*开始为原始大小*/
  }
  25%{
    transform: scale(1.1); /*放大1.1倍*/
  }
  50%{
    transform: scale(1);
  }
  75%{
    transform: scale(1.1);
  }

}

@-webkit-keyframes mymove /*Safari and Chrome*/
{
  0%{
    transform: scale(1);  /*开始为原始大小*/
  }
  25%{
    transform: scale(1.1); /*放大1.1倍*/
  }
  50%{
    transform: scale(1);
  }
  75%{
    transform: scale(1.1);
  }
}
</style>
