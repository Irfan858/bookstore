<script>
export default {
  data() {
    return {
      name: "Irfan",
    };
  },
  methods: {
    greet(name) {
      alert(`Hi ${name}, Welcome to Vue`);
    },
  },
};
</script>

<template>
  <div class="container d-flex flex-column justify-content-center text-center">
    <div>
      <a href="https://vitejs.dev" target="_blank">
        <img src="/vite.svg" class="logo" alt="Vite logo" />
      </a>
      <a href="https://vuejs.org/" target="_blank">
        <img src="../assets/vue.svg" class="logo vue" alt="Vue logo" />
      </a>
    </div>
    <div>
      <h1>Hello Vue</h1>
      <p>Learning Vue At Camp404</p>
    </div>
    <div>
      <input
        type="text"
        v-model="name"
        placeholder="Input Your Name"
        class="form-control"
      />
      <p>Your Name : {{ name }}</p>
      <button @click="greet(name)" class="btn btn-success">Say Hi</button>
    </div>
  </div>
</template>
<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
