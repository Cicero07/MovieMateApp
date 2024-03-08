<template>
  <header>
    <router-link to="/">
        <h1><span>Movie</span>Mate</h1>
    </router-link>
  </header>
  <main>
    <router-view/>
  </main>
</template>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Fira Sans', sans-serif;

    &::selection{
      background: transparentize(#42b883,0.5);
    }
  }

  body{
    background-color: #35495e;
  }

  a{
    text-decoration: none;
  }

  header{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px 16px;
    background-color: #2c3d4e;
    box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.1);

    h1 {
      color: white;
      font-size: 28px;
    

      span{
      color: #42B883;
      }
    }
  }

  @media only screen and (min-width: 769px) {
  header {
    padding: 16px;
  }

  h1 {
    font-size: 32px;
  }

  .search-box {
    padding: 16px;
  }

  input[type="text"] {
    font-size: 20px;
    padding: 10px 16px;
  }

  input[type="submit"] {
    font-size: 20px;
    padding: 16px;
  }

  .movie-list {
    .movie {
      max-width: 50%;
      flex: 1 1 50%;
    }
  }
}
</style>
