<template>
  <main class="main">
    <div class="pokemons-list">
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <PokemonCard />
      <div class="load-more-wrapper">
        <button class="button load-more-wrapper__button">
          Load More
        </button>
      </div>
    </div>
    <div class="pokemon">
      <Sidebar />
    </div>
  </main>
</template>

<script>
import PokemonCard from "./PokemonCard";
import Sidebar from "./Sidebar";
export default {
  components: {
    PokemonCard,
    Sidebar
  }
};
</script>
<style lang="css">
/* button */

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

.pokemon {
  display: flex;
  justify-content: center;
  align-items: flex-start;
}
</style>
