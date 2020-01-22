<template>
  <header class="header">
    <h1 class="header__title">Pokedex</h1>
  </header>
</template>
<style scoped lang="css">
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
@media (min-width: 540px) {
  .header__title {
    padding: 8px 80px 8px 80px;
  }
}
</style>
