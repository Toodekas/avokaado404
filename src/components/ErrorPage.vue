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
            <ul class="btns">
                <li>
                    <div class="back-btn">
                        <a @click="history.back()" type="button" class="btn btn-primary btn-radius" >Previous page</a>
                    </div>
                </li>
                <li><a href="https://avokaado.io/" class="btn btn-secondary btn-radius">Go home</a></li>
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

<style scoped>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-flex;
  margin: 0 10px;
}

p {
    font-size: 1.125rem;
    line-height:1.875rem;
    letter-spacing: 0.027rem;
    color:#647278;
}
u {
    text-decoration: underline;
    -webkit-text-decoration-color: #2EBD59; /* safari still uses vendor prefix */
    text-decoration-color: #2EBD59;
    bottom: -0.4rem;
    text-underline-offset: 0.4rem;
}

.error {
    z-index: 2;
    display:flex;
    flex-direction: column;
    position: relative;
}
.error::before {
    z-index: 1;
    display: block;
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    background: url('../assets/background-avokados-left.svg') left top no-repeat ;
    width: 30rem;
    height: 48rem;
}
.error::after {
    z-index: 1;
    display: block;
    content: "";
    position: absolute;
    top: 0;
    right: 0;
    background: url('../assets/background-avokaado-right.svg') right top no-repeat ;
    width: 30rem;
    height: 48rem;
}
.content {
    margin-top: 6rem;
}
.btn {
    border-color: #2EBD59;
    padding-left:2.25rem;
    padding-right:2.25rem;
    width:12rem;
}
.btn-primary {
    background-color:#2EBD59;
}
.btn-primary:hover {
    background-color:#1d7437;
    border-color: #1d7437;
}
.btn-secondary {
    background-color: #ffffff;
    color:#000000;
}
.btn-secondary:hover {
    background-color: #2EBD59;
    color:#ffffff;
    border-color: #2EBD59;
}

.btn-radius {
    border-radius: 2.6rem;
}

.btns{
    flex-direction: column;
}

@media only screen and (max-width: 1100px){
    .error::before{
        background: none;
    }
    .error::after{
        background: none;
    }
}
@media only screen and (max-width: 420px){
    .btn-secondary {
        margin-top:0.8rem;
    }
}
</style>
