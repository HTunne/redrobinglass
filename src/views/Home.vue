<template>
  <div class="home">
    <img alt="Red Robin Glass logo" src="../assets/robin_opt.svg" />
    <h1>Red Robin Glass</h1>
    <div id='homelinks'>
      <nav-button title='About' route='/about' />
      <nav-button title='Gallery' route='/gallery' />
      <nav-button title='Contact' route='/contact' emphasis=true />
    </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavButton from "@/components/NavButton.vue";

export default {
  name: "Home",
  components: {
    NavButton
  }
};
</script>


<style scoped>
img{
    opacity: 0.6;
    height: 9em;
    margin: 30px auto 0 auto;
}

h1 {
    margin-top: 1rem;
    color: #a90d07;
    font-family: 'Amatic SC';
    font-size: 4em;
}

#homelinks {
    display: flex;
    flex-direction: column;
    align-items: center;
}

#about {
    font-weight: 100;
}
</style>
