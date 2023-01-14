<template>
<Container>
<ChatWindow>
<ChatMessage username="Stiv ">
</ChatMessage>
</ChatWindow>
</Container>
</template>
<script>
import Container from "./components/MyContainer.vue";
import ChatMessage from "./components/ChatMessage.vue";
import ChatWindow from "./components/ChatWindow.vue";

export default {
  name: "App",
  components: {
    Container,
    ChatMessage,
    ChatWindow,
  },
  methods: {
    getList() {
      this.axios.get('https://61bcd385d8542f0017824a2a.mockapi.io/messages').then(response => (console.log(response.data)))
    }
  }
};
</script>
<style>
body {
  margin: 0;
  background-color: #f9f9fa;
}
</style>
