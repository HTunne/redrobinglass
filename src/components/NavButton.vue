<template>
    <div id="nav-button" :class="{ emph: emphasis }">
        <div>
            <router-link v-bind:to=route>{{ title }}</router-link>
        </div>
    </div>
</template>

<script>
export default {
    name: "nav-button",
    props: {
        title: String,
        route: String,
        emphasis: Boolean,
    }
}
</script>

<style scoped>
a:link {
  text-decoration: none;
}

a:visited {
  text-decoration: none;
}

a:hover {
  text-decoration: none;
}

a:active {
  text-decoration: none;
}

#nav-button {
    margin: 0.5rem;
    padding:  0.5rem;
    width: 10rem;
    border-radius: 0.25rem;
    border: 1px solid black;
}

#nav-button a {
  font-weight: bold;
  color: #2c3e50;
}

#nav-button a.router-link-exact-active {
  color: #42b983;
}

.emph {
    background: green;
    border: 1px solid green;
}


</style>
