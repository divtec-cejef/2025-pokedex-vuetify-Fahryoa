<script setup lang="ts">
  const listeQuestion = [
    {
      question: 'Qu\'est-ce qu\'un Pokédex ?',
      answer: 'Un Pokédex est un dispositif électronique qui répertorie et fournit des informations sur les différentes espèces de Pokémon. Notre application est une version numérique de cet outil.',
    },
    {
      question: 'Comment puis-je ajouter un Pokémon à mes favoris ?',
      answer: 'Pour ajouter un Pokémon à vos favoris, cliquez simplement sur l\'icône en forme de cœur sur la carte du Pokémon. L\'icône deviendra rouge pour indiquer que le Pokémon est maintenant dans vos favoris.',
    },
    {
      question: 'Pourquoi certains Pokémon ont-ils plusieurs types ?',
      answer: 'Certains Pokémon possèdent des caractéristiques de plusieurs types, ce qui se reflète dans leurs capacités et leurs faiblesses. Par exemple, Charizard est à la fois de type Feu et Vol.',
    },
    {
      question: 'Comment fonctionne la recherche de Pokémon ?',
      answer: 'Vous pouvez rechercher des Pokémon en tapant leur nom dans la barre de recherche. La liste se mettra à jour automatiquement pour afficher les Pokémon dont le nom correspond à votre recherche.',
    },
    {
      question: 'Que signifient les différentes statistiques des Pokémon ?',
      answer: 'Les statistiques comme HP, Attaque, Défense et Vitesse représentent les capacités de base d\'un Pokémon. HP représente les points de vie, Attaque la puissance offensive, Défense la résistance aux attaques, et Vitesse détermine l\'ordre d\'action en combat.',
    },
    {
      question: 'L\'application est-elle mise à jour régulièrement avec de nouveaux Pokémon ?',
      answer: 'Oui, nous nous efforçons de maintenir notre base de données à jour avec les derniers Pokémon découverts. Cependant, la fréquence des mises à jour peut varier en fonction des nouvelles sorties de jeux et d\'informations officielles.',
    },
  ]
</script>

<template>
  <h1>Foire Aux Questions (FAQ)</h1>
  <div>
    <v-expansion-panels>
      <v-expansion-panel v-for="(questions, index) in listeQuestion" :key="index">
        <v-expansion-panel-title>{{ questions.question }}</v-expansion-panel-title>
        <v-expansion-panel-text>{{ questions.answer }}</v-expansion-panel-text>
      </v-expansion-panel>
    </v-expansion-panels>
  </div>
</template>

<style scoped>
div {
  max-width: 1160px;
  margin: auto;
}
h1 {
  text-align: center;
  padding-top: 16px;
  padding-bottom: 24px;
}
</style>
