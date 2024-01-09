<script >
export default {
    data() {
        return {
            message1: "Este es un mensaje que mande a alguien",
            message2: "Este es un mensaje que me mando alguien",
        };
    }
};
</script>

<template>
    <div class="chat-abierto">
        <article class="message-r">
                <p class="message-description-send">{{ message1 }}</p>
                <img src="/images/prueba.png" alt="Imagen prueba">
            </article>
        <article class="message">
            <img src="/images/prueba.png" alt="Imagen prueba">
                <p class="message-description-r">{{ message2 }}</p>
        </article>
        <article class="message-r">
                    <p class="message-description-send">{{ message1 }}</p>
                    <img src="/images/prueba.png" alt="Imagen prueba">
                </article>
            <article class="message">
                <img src="/images/prueba.png" alt="Imagen prueba">
                    <p class="message-description-r">{{ message2 }}</p>
            </article>
            <article class="message-r">
                        <p class="message-description-send">{{ message1 }}</p>
                        <img src="/images/prueba.png" alt="Imagen prueba">
                    </article>
                <article class="message">
                    <img src="/images/prueba.png" alt="Imagen prueba">
                        <p class="message-description-r">{{ message2 }}</p>
                </article>
    </div>
</template>


<style scoped>

.chat-abierto{
    padding: 25px;
}

.message{
    display: flex;
    align-items: center;
    gap: 15px;
}

.message img{
    height: 60px;
    width: 60px;
    border-radius: 100%;
}

.message-r{
    display: flex;
    align-items: center;
    gap: 15px;
    justify-content: end;
}

.message-r img{
    height: 60px;
    width: 60px;
    border-radius: 100%;
}

.message-description-send{
    padding: 10px;
    background-color: blueviolet;
    color: white;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.message-description-r{
    padding: 10px;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

* {
    margin: 0;
    padding: 0;
}</style>
