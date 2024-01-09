<script >
export default {
    data() {
        return {
            contactos:[{
                name: "Carlos Milano",
                description: "Alguna descripcion del contacto"
            },
            {
                name: "Carlos Milano",
                description: "Alguna descripcion del contacto"
            },
            {
                name: "Carlos Milano",
                description: "Alguna descripcion del contacto"
            },
            {
                name: "Carlos Milano",
                description: "Alguna descripcion del contacto"
            },
            {
                name: "Carlos Milano",
                description: "Alguna descripcion del contacto"
            },
        ]
        }
    }
};
</script>

<template>
    <div v-for="(contacto, index) in contactos" :key="index" class="chat">
        <img src="/images/prueba.png" alt="Imagen prueba">
        <article>
            <h5>{{ contacto.name }}</h5>
            <p>{{ contacto.description }}</p>
        </article>
    </div>
</template>


<style scoped>
.chat {
    display: flex;
    align-items: center;
    gap: 15px;
    padding: 10px;
    transition: background-color 0.3s;
    border-radius: 15px;
    margin: 8px
}
.chat:hover {
  background-color: rgba(193, 99, 255, 0.7);
}
.chat img {
    height: 50px;
    width: 50px;
    border-radius: 100%;
}

.chat p {
    font-size: 15px;
}

* {
    margin: 0;
    padding: 0;
}
</style>
