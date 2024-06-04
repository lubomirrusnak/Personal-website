<template>
    <div>
      <!-- Rounded switch -->
      <label class="switch">
        <input type="checkbox" @click="toggleDark" v-model="isDark">
        <span class="slider round"></span>
      </label>
  
      <div :style="{ backgroundColor: isDark  }">

        <p></p>
      </div>
    </div>
  </template>
  
  <script>
  import { useDark, useToggle } from '@vueuse/core';
  
  export default {
    data() {
      return {
        isDark: useDark({
          selector: 'body',
          attribute: 'color-scheme',
          valueDark: 'dark',
          valueLight: 'light',
        }),
      };
    },
    methods: {
      toggleDark() {
        useToggle(this.isDark);
      },
    },
  };
  </script>
  
  <style>
  .switch {
    position: fixed;
    display: inline-block;
    width: 50px;
    height: 20px;
  }
  
  /* Hide default HTML checkbox */
  .switch input {
    opacity: 0;
    width: 0;
    height: 0;
  }
  
  /* The slider */
  .slider {
    position: absolute;
    cursor: pointer;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background-color: #ccc;
    -webkit-transition: .4s;
    transition: .4s;
  }
  
  .slider:before {
    position: absolute;
    content: "";
    height: 20px;
    width: 26px;
    left: 2px;
    bottom: 0px;
    background-color: white;
    -webkit-transition: .4s;
    transition: .4s;
  }
  
  input:checked + .slider {
    background-color: #2196F3;
  }
  
  input:focus + .slider {
    box-shadow: 0 0 1px #2196F3;
  }
  
  input:checked + .slider:before {
    -webkit-transform: translateX(26px);
    -ms-transform: translateX(26px);
    transform: translateX(26px);
  }
  
  /* Rounded sliders */
  .slider.round {
    border-radius: 34px;
  }
  
  .slider.round:before {
    border-radius: 50%;
  }
  
  [color-scheme='dark'] {
    background: linear-gradient(90deg, rgb(0, 0, 7) 0%, rgb(5, 5, 63) 35%, rgb(78, 93, 136) 100%);
  }
  
  [color-scheme='light'] {
    background: linear-gradient(90deg, rgb(17, 6, 214) 0%, rgb(57, 90, 162) 35%, rgb(185, 192, 214) 100%);
  }
  </style>