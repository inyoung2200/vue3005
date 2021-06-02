<template>
  <div id="wrap">
    <Header />
    <main>
      <!-- mainCont -->
      <section id="mainCont">
        <div class="main_cont">
          <div v-for="todo in todos" v-bind:key="todo.text">
            {{ todo.text }}
          </div>
        </div>
      </section>
      <!-- //mainCont -->
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  components: {
    Header,
  },
  data: function () {
    return {
      todos: [
        { text: "we provide" },
        { text: "visual coding" },
        { text: "solutions" },
        { text: "for you webs" },
      ],
    };
  },
};
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
