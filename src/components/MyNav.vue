<template>
  <nav class="my-nav">
    <div class="logo">
      <img src="@/assets/nav-logo.png" alt="" />
    </div>
    <div class="links">
      <ul>
        <li v-for="link in links" :key="link">{{ link }}</li>
      </ul>
    </div>
    <div class="btns">
      <button>LOGIN</button>
      <button>SIGN UP</button>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      logo: "My Logo",
      links: ["Link one", "Link Two", "Link Three", "Link Four"],
    };
  },
};
</script>
