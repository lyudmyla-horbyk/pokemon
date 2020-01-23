<template>
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
</template>
<style scoped lang="css">
.pokemon-card .pokemon-card__img {
  width: 100%;
  display: block;
}
.pokemon-card {
  border: 1px solid black;
  padding: 10px;
}
.pokemon-card .pokemon-card__title {
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
.tag {
  padding: 8px 10px 8px 10px;
  cursor: pointer;
  border-radius: 5px;
  font-size: 20px;
  border: none;
  transition-duration: 0.4s;
}
@media (min-width: 400px) {
  .tag--green {
    padding: 10px 30px 10px 30px;
  }
  .tag--violet {
    padding: 10px 30px 10px 30px;
  }
}
</style>
