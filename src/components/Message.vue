<script >

</script>

<template>
    <div class="send-message">
             <input class="box" type="text" placeholder="Type your message..">
            <button>Send</button>
    </div>
</template>


<style scoped>
.send-message {
    width: 90%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    position: absolute;
    bottom: 40px;
    right: 40px;
}

.box{
    width: 100%;
    height: 40px;
    display: flex;
    align-items: center;
    border: none;
    padding: 7px;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}
.send-message button{
    padding: 10px 22px ;
    background-color: blueviolet;
    border: none;
    border-radius: 5px;
    color: white;
    position: absolute;
    right: 10px;
}

* {
    margin: 0;
    padding: 0;
}</style>
