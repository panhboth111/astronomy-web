<template>
  <v-app-bar app dark flat fixed clipped-right>
    <v-toolbar-title class="display-1 font-weight-light"
      ><span>ASTRO</span><span class="purple--text">KIT</span></v-toolbar-title
    >

    <v-spacer></v-spacer>
    <div class="hidden-sm-and-down mr-10">
      <router-link
        v-for="(item, i) in items"
        :key="i"
        :to="item.router"
        style="text-decoration:none"
        class="black--text"
      >
        <v-btn class="subtitle font-weight-light">{{ item.title }}</v-btn>
      </router-link>
    </div>
    <v-app-bar-nav-icon
      @click="drawerToggle"
      class="hidden-md-and-up"
    ></v-app-bar-nav-icon>
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: "About", router: "/about" },
      { title: "Documents", router: "/documents" },
      { title: "Contact", router: "/contact" }
    ]
  })
};
</script>

<style></style>
