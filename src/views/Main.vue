<template>
  <div id="wrap">
    <Header />
    <main>
      <!-- mainCont -->
      <section id="mainCont">
        <div class="main_cont">
          <div>{{msg1}}</div>
          <div>{{msg2}}</div>
          <div>{{msg3}}</div>
          <div>{{msg4}}</div>
        </div>
      </section>
      <!-- //mainCont -->
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header.vue';

export default {
  components: {
    Header,
  },
  data(){
    return {
      msg1 : "we provide",
      msg2 : "visual coding",
      msg3 : "solutions",
      msg4 : "for you webs",
    }
  }
}
</script>

<style lang="scss" scoped>
#mainCont {
  height: 100vh;
  background: #000;
  display: flex;
  justify-content: center;
  align-items: center;

  .main_cont {
    color: #fff;
    font-size: 10vw;
    line-height: 0.85;
    letter-spacing: -0.0275em;
    transition: all 2s;
    text-transform: uppercase;
    font-family: serif;
    font-family: "Saol Display Regular";
  }
}
</style>
