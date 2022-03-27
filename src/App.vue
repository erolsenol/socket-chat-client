<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="align-center"></div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main>
      <HelloWorld v-if="false" />
      <ChatPanel />
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from "./components/HelloWorld";
import ChatPanel from "@/components/ChatPanel.vue";

export default {
  name: "App",

  components: {
    HelloWorld,
    ChatPanel,
  },

  data: () => ({
    //
  }),
};
</script>
