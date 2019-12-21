<template>
  <div id="app">
    <h1>Calculator <span>by Danilo Costa</span></h1>
    <Calculator />
  </div>
</template>

<script>
import Calculator from "./main/Calculator"
export default {
  name: 'app',
  components: { Calculator }
}
</script>

<style>
    * { font-family: 'Roboto Mono'; margin: 0; padding: 0 }
    h1 { margin-bottom: 2rem; text-shadow: rgba(0,0,0,.5) 1px 1px 2px }
    h1 span { display: block; font-weight: lighter; font-size: 1rem; color: #ffffffcc }
    #app {
        display: flex;
        flex-direction: column;
        height: 100vh;
        justify-content: center;
        align-items: center;
        text-align: center;
        color: #fff;
        background-color: #0093E9;
        background-image: linear-gradient(160deg, #0093E9 0%, #80D0C7 100%);
    }
</style>
