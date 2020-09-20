<template>
  
  <div class="container">
    
    <header>

      <h1>{{ page.title }}</h1>
      <p>{{ page.description }}</p>

    </header>

    <section>

      <div class="full">

        <nuxt-content :document="page" />

      </div>
      
      <div class="split" style="background: #023059; color: #023059">

        <div class="half">
          
          <p>Helloworld</p>
        
        </div>

        <div class="half">

          <p>Other half </p>

        </div>

      </div>

    </section>

  </div>

</template>

<script>
import Navigation from '@/components/Navigation'

export default {

  components: { Navigation },
  data() {

    return {

      page: {}

    }

  },
  async asyncData({ $content }) {

    let page = await $content('homescreen').fetch();

    return { page }

  }

}
</script>

<style scoped>

  .container {

    overflow: hidden;

  }

  header {

    background: #fff url('/train-night-blue.jpg') no-repeat center/cover;
    height: 100vh;
    width: 100vw;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

  }

  header h1 {

    background-color: white;
    color: black;
    font-size: 5rem; 
    font-weight: bold;
    padding: 20px;
    mix-blend-mode: screen;
    animation-name: intro;
    animation-duration: 5s;

  }

  header p {

    margin: 10px;
    padding: 15px;
    color: #011C40;;
    background: white;
    font-weight: bold;
    animation-name: intro;
    animation-duration: 5s;

  }

  section {

    background: #D5E5F2;
    color: #023059;
    font-weight: bold;

  }

  @keyframes intro {

    0% {

      transform: scale(0);

    }

    100% {

      transform: scale(1);

    }

  }

</style>
