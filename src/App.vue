<template>
  <img class="step-2" alt="Vue logo" src="./assets/logo.png">
  <HelloWorld class="hello" msg="Welcome to Your Vue.js App"/>
  <vue-guided-tour :steps="steps" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data() {
    return {
      steps: [
        {
          target: '.step-1',
          slot: 'step-1',
          title: 'Testando o Tour',
          content: 'Apenas um teste da lib que o Jeudi mandou no grupo. Nunca tinha usasdo, porém parece bem bacana!',
          popover: {
            placement: 'start',
            position: 'right',
            id: 'hello-world',
          },
        },
        {
          target: '.step-2',
          title: 'Logo do Vue',
          content: 'Aqui é a logo do Vue!',
          popover: {
            placement: 'end',
            position: 'right',
          },
        },
        {
          target: '.step-3',
          title: 'Bem-vindo ao Vue.js App',
          content: 'Bem-vindo ao Vue.js App',
          popover: {
            placement: 'center',
            position: 'left',
          },
        },
        {
          target: '.step-4',
          title: 'Plugins Instalados',
          content: 'Plugins Instalados',
          popover: {
            placement: 'center',
            position: 'right',
          },
        },
        {
          target: '.step-5',
          title: 'Links Importantes',
          content: 'Links Importantes',
          popover: {
            placement: 'center',
            position: 'bottom',
          },
        },
        {
          target: '.step-6',
          title: 'Todo Ecossistema',
          content: 'Todo Ecossistema',
          popover: {
            placement: 'center',
            position: 'top',
          },
        },
        {
          target: '.step-7',
          title: 'Muito Bem-vindo!',
          content: 'Caso hajam mais dúvidas, visite nosso FAC.',
          popover: {
            placement: 'start',
            position: 'center',
            id: 'finish',
          },
        },
      ],
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.hello {
  width: 500px;
}
</style>
