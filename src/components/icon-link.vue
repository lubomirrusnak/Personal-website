<template>



<div class="link">

  <fa class="linkedin" :icon="['fab', 'linkedin']"  style= "color: white;" @click="handleClick"  />



  <fa class="github" :icon ="['fab','github']" style="color: white;" @click="handleClickG"/>




  <fa class="instagram" :icon ="['fab','instagram']" style="color: white;" @click="handleClickI"/>

</div>
</template>

<script>
    export default {
        methods: {
    handleClick() {
      //window.location.href = 'https://www.linkedin.com/in/%C4%BEubom%C3%ADr-rusn%C3%A1k-6882ba211/';
      window.open('https://www.linkedin.com/in/%C4%BEubom%C3%ADr-rusn%C3%A1k-6882ba211/'); //This will open Google in a new window.

      // Your click event handling logic here
    },


    handleClickG() {
      window.open('https://github.com/projects');
      // Your click event handling logic here
    },

    handleClickI() {
      window.open('https://www.instagram.com/pifko_lr/');
      // Your click event handling logic here
    }
    },
}
</script>

<style scoped>


.linkedin{
 cursor:pointer;
margin-right: 1%;
padding: 10px; /* Optional: Adds some space around the icons */

}

.github{
  cursor:pointer;
  padding: 10px; /* Optional: Adds some space around the icons */

}
.instagram{
  cursor:pointer;
  padding: 10px; /* Optional: Adds some space around the icons */

}
.link{
  
  display: flex;
  align-items: center;
  font-size: 50px;
  margin-top: 20%;
  margin-left: -50%;
  position: relative;
  border-color: red;
  padding: 10px; /* Optional: Adds some space around the icons */

}

</style>