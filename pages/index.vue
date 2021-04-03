<template>
  <div class="container">
    <div>
      <h1 class="title">
        这是一个nuxt.js
      </h1>
      <div class="links">
        <!-- 相当于刷新页面 -->
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
          style="width: 200px;"
        >
          Documentation
        </a>
        <nuxt-link to="/student" class="button--green" style="width: 200px;height: 100px; line-height: 80px;"  >跳转学生默认页面</nuxt-link>
        <button class="button--green" style="width: 200px;height: 200px;" @click="jump">这是一个学生id页面</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  methods: {
    jump() {
      this.$router.push({path: "/student/1"})
    }
  }

}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
  -o-table-baseline: inherit;
}
</style>
