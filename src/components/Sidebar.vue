<template>
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
</template>
<style scoped lang="css">
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
