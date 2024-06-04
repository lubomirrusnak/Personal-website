<template>
<div class="container">
    <div class="left">
      <h1>Education</h1>  
      <h2>Masters of Technology in Computer Science </h2>
      <h2>Bachelor of Technology in Inteligent Systems</h2>
      <h2>Secondary School of Electrical Engineering in Kosice</h2>

    </div>
    <div class="right">
      <h1>Skills</h1>
      <h2>Coding</h2>
      <ul>
      <li>Vue 3</li>
      <li>C#</li>
      <li>Python</li>
      <li>SQL</li>
      </ul>
      <h2>Proffesionall skills</h2>
      <ul>
        <li>Front end</li>
        <li>Backend</li>
        <li>Data Analysis</li>
    </ul>
    </div>
  </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
.container {
  display: flex;
  height:100vh; /* Nastaví výšku na celou obrazovku */
  width: 100vh;
}
.left, .right {
  flex: 1; /* Flexibilní box, každý zabere polovinu místa */
  
  color: wheat;
}
.prava{
border-radius: 0%;
border-style: solid;
border-color: coral;
}
h2 {
    border-radius: 0%;
    border-style: solid;
  border-color: coral;
}


</style>