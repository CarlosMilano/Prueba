<script setup>
import Menu from './components/Menu.vue';
import Chat from './components/Chat.vue';
import Contact from './components/Contact.vue';
import ChatMenu from './components/ChatMenu.vue';
import Abierto from './components/Abierto.vue';
import Message from './components/Message.vue';
</script>

<template>
    <div id="App" class="home">
        <section class="menu">
          <Menu/>
          <h1>Chats</h1>
            <Chat/> 
            <h1>Contacts</h1>
            <Contact/>
        </section>
        <section class="chat-area">
            <ChatMenu/>
            <Abierto/>
            <Message/>
        </section>
    </div>
</template>

<style scoped>

.home{
    display: grid;
    grid-template-columns: 350px 1fr;
    grid-template-areas: "menu chat";

}
.menu{
    width: 320px;
    height: 100vh;
    margin: 0;
    display: flex;
    flex-direction: column;
    padding: 15px;
    grid-area: menu;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.chat-area{
    grid-area: chat;
    position: relative;
}

h1{
    font-family: sans-serif;
    color: blueviolet;
    font-weight: 400;
    padding: 10px;
}
</style>
