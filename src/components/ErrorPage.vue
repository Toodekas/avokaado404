<template>
    <div class="error">
        <div class="content">
            <div class="logo404">
                <img alt="Vue logo" src="../assets/404Logo.svg">
            </div>
            <h1>Page not <u>found?</u></h1>
            <p>
            Seems like something is missing from avokaado.<br>
            We cannot find what you are looking for.
            </p>
            <h3>Installed CLI Plugins</h3>
            <ul>
                <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-babel" target="_blank" rel="noopener">babel</a></li>
                <li><a href="https://github.com/vuejs/vue-cli/tree/dev/packages/%40vue/cli-plugin-eslint" target="_blank" rel="noopener">eslint</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  name: 'ErrorPage',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-flex;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.error::before {
    display: block;
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    background: url('../assets/background-avokados-left.svg') left top no-repeat ;
    width: 30rem;
    height: 48rem;
}
.content {
    
}
.error::after {
    display: block;
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    background: url('../assets/background-avokaado-right.svg') right top no-repeat ;
    width: 30rem;
    height: 48rem;
}
</style>
