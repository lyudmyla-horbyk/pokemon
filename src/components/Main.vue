<template>
  <body>
    <header class="header">
      <h1 class="header__title">Pokedex</h1>
    </header>
    <main class="main">
      <div class="pokemons-list">
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Bulbazavr.png" />
          <h2 class="pokemon-card__title">Bulbazavr</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--green">
              Grass
            </div>
            <div class="tag tag--violet">
              Poison
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Charmander.png" />
          <h2 class="pokemon-card__title">Charmander</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--red">
              Fire
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Bulbazavr.png" />
          <h2 class="pokemon-card__title">Bulbazavr</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--green">
              Grass
            </div>
            <div class="tag tag--violet">
              Poison
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Charmander.png" />
          <h2 class="pokemon-card__title">Charmander</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--red">
              Fire
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Bulbazavr.png" />
          <h2 class="pokemon-card__title">Bulbazavr</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--green">
              Grass
            </div>
            <div class="tag tag--violet">
              Poison
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Charmander.png" />
          <h2 class="pokemon-card__title">Charmander</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--red">
              Fire
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Bulbazavr.png" />
          <h2 class="pokemon-card__title">Bulbazavr</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--green">
              Grass
            </div>
            <div class="tag tag--violet">
              Poison
            </div>
          </div>
        </article>
        <article class="pokemon-card">
          <img class="pokemon-card__img" src="../assets/img/Charmander.png" />
          <h2 class="pokemon-card__title">Charmander</h2>
          <div class="pokemon-card__tags">
            <div class="tag tag--red">
              Fire
            </div>
          </div>
        </article>
        <div class="load-more-wrapper">
          <button class="button load-more-wrapper__button">
            Load More
          </button>
        </div>
      </div>
      <div class="pokemon">
        <div class="sidebar">
          <img class="sidebar__img" src="../assets/img/Charmander.png" />
          <h2 class="sidebar__title">Charmander #004</h2>
          <div class="sidebar__table-wrapper">
            <table>
              <tr>
                <td>
                  Type
                </td>
                <td>Fire</td>
              </tr>
              <tr>
                <td>Attact</td>
                <td>52</td>
              </tr>
              <tr>
                <td>Deffens</td>
                <td>43</td>
              </tr>
              <tr>
                <td>HP</td>
                <td>39</td>
              </tr>
              <tr>
                <td>SP Attatct</td>
                <td>60</td>
              </tr>
              <tr>
                <td>SP Deffens</td>
                <td>50</td>
              </tr>
              <tr>
                <td>Speed</td>
                <td>65</td>
              </tr>
              <tr>
                <td>Weight</td>
                <td>85</td>
              </tr>
              <tr>
                <td>Total moves</td>
                <td>89</td>
              </tr>
            </table>
          </div>
        </div>
      </div>
    </main>
    <footer class="footer"></footer>
  </body>
</template>

<style lang="css">
/* general */

header,
main,
footer,
h1,
h2,
h3,
h4,
h5,
h6,
p {
  margin: 0;
  padding: 0;
}

body {
  max-width: 1200px;
  margin: auto;
  font-family: "Exo 2", sans-serif;
  padding: 7px;
}
* {
  box-sizing: border-box;
}

/* header */

.header {
  display: flex;
  justify-content: center;
  align-items: center;
}

.header__title {
  border: 1px solid black;
  font-size: 50px;
  margin-bottom: 15px;
  padding: 0 5px 0 5px;
}

/* button */

.tag,
.button {
  padding: 8px 10px 8px 10px;
  cursor: pointer;
  border-radius: 5px;
  font-size: 20px;
  border: none;
  transition-duration: 0.4s;
}

/* main */

@media (min-width: 540px) {
  .pokemons-list {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-gap: 5px;
  }
  .header__title {
    padding: 8px 80px 8px 80px;
  }
}
@media (min-width: 900px) {
  .pokemons-list {
    grid-template-columns: 1fr 1fr 1fr;
  }
}
@media (min-width: 1100px) {
  main {
    display: grid;
    grid-template-columns:
      50%
      50%;
  }
  .pokemons-list {
    grid-template-columns: 1fr 1fr;
  }
}

.pokemons-list .pokemon-card__img {
  width: 100%;
  display: block;
}
.pokemons-list .pokemon-card {
  border: 1px solid black;
  padding: 10px;
}
.pokemons-list .pokemon-card__title {
  text-align: center;
  margin-bottom: 20px;
  margin-top: 20px;
}

.pokemon-card .pokemon-card__tags {
  display: flex;
  justify-content: space-around;
}
.tag.tag--green {
  background-color: #99ffbb;
}
.tag.tag--green:hover {
  background-color: #00e600;
  color: white;
}
.tag.tag--red {
  background-color: #ff471a;
}
.tag.tag--red:hover {
  color: white;
  background-color: #e62e00;
}
.tag.tag--violet {
  background-color: #d9b3ff;
}
.tag.tag--violet:hover {
  color: white;
  background-color: #b366ff;
}
@media (min-width: 400px) {
  .tag--green {
    padding: 10px 30px 10px 30px;
  }
  .tag--violet {
    padding: 10px 30px 10px 30px;
  }
}
.load-more-wrapper {
  display: grid;
  grid-column: 1/3;
}
.load-more-wrapper .load-more-wrapper__button {
  background-color: #0099ff;
  color: white;
  width: 100%;
  margin-top: 15px;
}

.load-more-wrapper .load-more-wrapper__button:hover {
  background-color: #007acc;
}

/* sidebar */
.pokemon {
  display: flex;
  justify-content: center;
  align-items: flex-start;
}
.sidebar {
  border: 1px solid black;
  padding: 10px;
}
.sidebar .sidebar__title {
  text-align: center;
  margin-bottom: 20px;
  margin-top: 20px;
}

.sidebar .sidebar__table-wrapper {
  display: flex;
  justify-content: center;
}
.sidebar .sidebar__img {
  height: 259px;
}
</style>
