<template>
    <!-- Le template définit la structure HTML du composant -->
    <div>
        <h1>Récepteur</h1>
        <RadioComponent @coin="updateMessage"/>
        <!-- Inclusion du composant "RadioComponent" et écoute de l'événement personnalisé "coin" -->
        {{ message }}
        <!-- Affichage de la variable "message" -->
    </div>
</template>

<script>
import RadioComponent from "./Radio"  // Import du composant "RadioComponent"

export default {
    name: "ReceiverComponent", // Nom du composant
    components: {
        RadioComponent, // Enregistrement du composant "RadioComponent" pour pouvoir l'utiliser
    },
    data: () => ({
        message: "Pas de message", // Initialisation de la variable "message"
    }),
    methods: {
        updateMessage(payload) {
            // Une méthode qui reçoit le payload de l'événement "coin"
            this.message = payload.message; // Mise à jour de la variable "message" avec le message reçu
        }
    }
}
</script>
