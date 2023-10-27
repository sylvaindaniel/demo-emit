<template>
    <div class="radio">
        <h2>Radio</h2>
        <button @click="sendMessage">Envoyer un message</button>
    </div>
</template>

<script>
export default {
    name: "RadioComponent", // Nom du composant
    methods: {
        sendMessage() {
            // la fonction $emit est appelée lorsque le bouton est cliqué, 
            //elle prend en paramètre le nom de l'evenement et un payload (l'objet message avec le contenu du message)
            this.$emit('coin', {
                message: 'Message à moi'
            });
        }
    }
}
</script>

<style scoped lang="scss">
.radio {
    margin-bottom: 15px;
}
</style>
