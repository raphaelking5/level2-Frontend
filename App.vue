<template>

<h1> form1 </h1>
  <main id="kkkkk">
     <p>
    <label for="name">Name</label>
    <input
      id="name"
      v-model="name"
      type="text"
      name="name"
    >
  </p>

  <p>
    <label for="age">Age</label>
    <input
      id="age"
      v-model="age"
      type="number"
      name="age"
      min="0"
    >
  </p>

  <p>
    <label for="movie">Favorite Movie</label>
    <select
      id="movie"
      v-model="movie"
      name="movie"
    >
      <option>Star Wars</option>
      <option>Vanilla Sky</option>
      <option>Atomic Blonde</option>
    </select>
  </p>
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
      </main>

       <p>
    <input
      type="submit"
      value="validez"
    >
  </p>

  <div id="toto">
     <p>
    <label for="name">Name</label>
    <input
      id="name"
      v-model="name"
      type="text"
      name="name"
    >
  </p>
  <span v-if="nom">Vous avez  {{ nom }} ans</span>

  <p>
    <label for="age">Age</label>
    <input
      id="age"
      v-model="age"
      type="number"
      name="age"
      min="0"
    >
  </p>

  <p>
    <label for="movie">Favorite Movie</label>
    <select
      id="movie"
      v-model="movie"
      name="movie"
    >
      <option>Star Wars</option>
      <option>Vanilla Sky</option>
      <option>Atomic Blonde</option>
    </select>
  </p>
      <div>
        <label for="age">Votre age</label>
        <select id="age" v-model="age">
          <option value="5">moins de 5 ans </option>
          <option value="20">moins de 20 ans </option>
          <option value="50">moins de 50 ans </option>
          <option value="105">moins de 105 ans </option>
        </select>
      </div>
      <span v-if="age">Vous avez  {{ age }} ans</span>
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
      </div>

       <p>
    <input
      type="submit"
      value="validez"
    >
  </p>
</template>
<script>
export default {
  name:"app",
  data(){
    return{
      errors: [],
name: "",
age: "",
movie: "",
  newHeading(){
    document.form1= this.form1;
  }
    }
  }
}
</script>

<style>
#kkkkk {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: aqua;
  color: coral;
}

#toto {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: rebeccapurple;
  color: red;
}
</style>



