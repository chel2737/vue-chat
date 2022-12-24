<template>
<Container>
<ChatWindow>
<ChatMessage>
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
};
</script>
<style>
body {
  margin: 0;
  background-color: #f9f9fa;
}
</style>
