<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Amatic+SC:wght@400;700&family=Montserrat:wght@100;200;300;400&display=swap');
:root {
    --background-color: #ffffef;
    --robin-red: #2c3e50;
}

body {
  background-color: var(--background-color);
}

#app {
  font-family: Montserrat, sans-serif;
  font-weight: thin;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--robin-red);
}

h1 {
    margin-top: 1rem;
    color: #a90d07;
    font-family: 'Amatic SC';
    font-size: 4em;
}
</style>
