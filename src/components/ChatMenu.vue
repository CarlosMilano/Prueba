<script >
export default {
    data() {
        return {
            name: "Carlos Milano",
            message: "Frontend Developer",
        };
    }
};
</script>

<template>
    <div  class="chat-menu">
        <article class="info">
            <img src="/images/prueba.png" alt="Imagen prueba">
            <article class="more-info">
                <h5>{{ name }}</h5>
                <p>{{ message }}</p>
            </article> 
        </article>
        
    </div>
</template>


<style scoped>
.chat-menu{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px;
    border-bottom: 2px solid rgb(181, 181, 181);
}
.chat-menu img{
    height: 60px;
    width: 60px;
    border-radius: 100%;
}

.info{
    display: flex;
    align-items: center;
    gap: 15px;
}
* {
    margin: 0;
    padding: 0;
}</style>
