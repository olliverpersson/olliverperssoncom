<template>
  <div>
    <Nuxt />
  </div>
</template>

<style>
html {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

/* 
Layout CSS Library
Created by Olliver Persson
github.com/olliverpersson/layout-library
*/

div.full,
div.split div {

    width: 100%;
    padding: 20px;
    overflow: hidden;
}

div.img img {

    width: 100%;
    max-height: 500px;
    object-fit: cover;

}

div.img, div.split div.img {

    padding: 0px;

}

div.dialog {

    position: fixed;
    width: 100vw;
    height: 100vh;
    top: 0px;
    left: 0px;
    background: rgba(75, 75, 75, 0.5);
    display: flex;
    justify-content: center;
    align-items: center;

}

@media screen and (min-width: 850px) {

    div.full,
    div.split div {

        width: auto;
        padding: 30px;
    }

    div.split {

        display: flex;
        display: -webkit-flex;
    }
    
    div.split-reverse {

        display: flex;
        display: -webkit-flex;
        flex-direction: row-reverse;
    }

    div.split div {

        flex-grow: 1;
    }

    div.split div.half {

        flex-basis: 50%;
    }

    div.split div.third {

        flex-basis: 33%;
        padding: 20px;

    }

    div.split div.fourth {

        flex-basis: 25%;
    }

    div.split div.fifth {

        flex-basis: 20%;
    }
    
    .img, div.split .img, div.third.img {

        padding: 0px;

    }

}

@media screen and (min-width: 900px) {

    div.full,
    div.split div {

        padding: 50px 100px 50px 100px;
        
    }

    .img {

        padding: 0px;

    }

}

@media screen and (min-width: 1500px) {
    
    div.full, div.split {
        
        width: 1100px;
        margin: 0px auto;
        
    }
    
}
</style>
