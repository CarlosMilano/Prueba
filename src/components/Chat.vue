<script >
export default {
    data() {
        return {
            chats:[
                {
                    name: "Carlos Milano",
                    message: "Buen dia como estas",
                    date: "8 Ene",
                },
                {
                    name: "Carlos Milano",
                    message: "Buen dia como estas",
                    date: "8 Ene",
                }
            ]
        };
    }
};
</script>

<template>
      <div v-for="(chat, index) in chats" :key="index" class="chat">
        <img src="/images/prueba.png" alt="Imagen prueba">
        <article>
            <h5>{{ chat.name }}</h5>
            <p >{{ chat.message }}</p>
        </article>
        <p class="date">{{ chat.date }}</p>
    </div>  
</template>


<style scoped>
.chat{
    display: flex;
    align-items: center ;
    gap: 15px;
    padding: 10px;
    position: relative;
    transition: background-color 0.3s;
    border-radius: 15px;
    margin: 8px;
}

.chat:hover {
  background-color: rgba(193, 99, 255, 0.7);
}
.chat img{
    height: 50px;
    width: 50px;
    border-radius: 100%;
}
.date{
    position: absolute;
    top: 14px;
    right: 8px;
}
.chat p{
    font-size: 15px;
}
* {
    margin: 0;
    padding: 0;
}</style>
