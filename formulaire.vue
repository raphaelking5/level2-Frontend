<template>
  <main id="kkkkk">
    <span v-if="name">Votre nom : {{ name }}</span>
    <div>
      <label for="name">Votre nom </label>
      <input type="text" v-model="name" id="name">

       <input v-model="message" placeholder="modifiez moi">
        <p> Le message est : {{ message }} </p>
        
      <div>
        <label for="age">Votre age</label>
        <select id="age" v-model="age">
          <option value="5">moins de 5 ans </option>
          <option value="20">moins de 20 ans </option>
          <option value="50">moins de 50 ans </option>
          <option value="105">moins de 105 ans </option>
        </select>
      </div>
      <span v-if="age">Vous avez moins de {{ age }} ans</span>
      <div>
        vous aimez les pommes ? <br />
        <div>
        <label for="yes">oui</label>
        <input type="radio" id="yes" value="true" v-model="apple" />
      </div>
      <div>
        <label for="no">non</label>
        <input type="radio" id="yes" value="true" v-model="apple" />
      </div> 
      </div>
      <span v-if="apple">Vous aimez les pommes</span>
      <span v-else> vous n'aimez pas les pommes</span>
      </main>
      
      
  <input v-model="maData" />
</template>


<script>
const rootComponent = {
    data() {
        return {
            maData:'Valeur par défaut'
        }
    }
}
const Formulaire = {
  data() {
    return {
      name : '',
      age :0,
      apple : false
    }
  },
}
const app = vue.createApp(Formulaire).mount ('#app')

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>