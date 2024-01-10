<script>
export default {
    data() {
        return {
            messages: [],
            newMessage: ''
        };
    },
    methods: {
        sendMessage() {
            if (this.newMessage.trim() !== '') {
                this.messages.push(this.newMessage);
                this.newMessage = '';
            }
        }
    }
};
</script>

<template>
    <div class="area">
            <div class="message-area" v-for="(message, index) in messages" :key="index">
                    <p class="message">{{ message }}</p>
                    <img src="/images/prueba.png" alt="Imagen prueba">
            </div>
        <div class="text-area">
            <input class="text-box" v-model="newMessage" placeholder="Type your message..." />
            <button @click="sendMessage">Send</button>
        </div>
    </div>
</template>

<style scoped>

.message-area {
    display: flex;
    right: 10px;
    margin: 10px;
    flex-direction: row;
    align-items: center;
    justify-content: flex-end;
}

.message {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    border-radius: 5px;
    padding: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    background-color: blueviolet;
    color: white;
}

.message-area img {
    height: 60px;
    width: 60px;
    border-radius: 100%;
    margin-left: 10px;
}
.text-area {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;
    height: 40px;
    position: absolute;
    bottom: 10px;
    right: 30px;
}
.area {
    display: flex;
    flex-direction: column;
    position: relative;
    height: 100%;
    width: 100%;
}
.text-box {
    width: 100%;
    height: 100%;
    border-radius: 5px;
    padding: 5px;
    border: none;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

button {
    position: absolute;
    border-radius: 5px;
    border: none;
    background-color: blueviolet;
    color: white;
    font-weight: 600;
    cursor: pointer;
    padding: 8px 13px;
    right: 10px;
}

* {
    margin: 0;
    padding: 0;
}
</style>
