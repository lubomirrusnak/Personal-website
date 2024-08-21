<template>
<div class="container">
    <div class="left">
      <h1>Education</h1>  
        <h2 class="Education">Masters of Technology in Computer Science </h2>
        <h2 class="Education">Bachelor of Technology in Inteligent Systems</h2>
        <h2 class="Education">Secondary School of Electrical Engineering in Kosice</h2>
      

      
    </div>
    <div class="right">
      <h1>Skills</h1>
      <div class="Coding-section">
      <h2>Coding</h2>
      <dl> 
          <dd>Vue 3</dd> 
          <dd>C#</dd>
          <dd>Python</dd>
          <dd>SQL</dd>
      </dl>
    </div>
    <div class="Coding-section">
      <h2>Proffesionall skills</h2>
      <dl> 
          <dd>Frontend</dd> 
          <dd>Backend</dd>
          <dd>Data Analysis</dd>
          <dd>Machine Learning</dd>
      </dl>
    </div>
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
h1{
  text-align: left;

}


.left, .right {
  flex: 1; /* Flexibilní box, každý zabere polovinu místa */
  color: wheat;

  
}
.prava{
margin-top: 40%;
border-radius: 0%;
border-style: solid;
border-color: coral;

}


.Coding-section{
  border-radius: 0%;
  border-style: solid;
  border-color: rgb(175, 194, 234);
  max-width: 400px; /* Maximálna šírka pre zúženie */  
  margin-bottom: 12px;
  text-align: left;
  padding-left: 20px;
  padding-top: 10px;
  border-radius: 5%;

}

.Education{
  border-radius: 5%;
  border-style: solid;
  border-color: rgb(175, 194, 234);
  max-width: 340px; /* Maximálna šírka pre zúženie */  
  margin-bottom: 12px;
  margin-bottom: 15px;
}

dd {
  margin-bottom: 12px; /* Pridanie väčšej medzery medzi riadkami */
}



</style>