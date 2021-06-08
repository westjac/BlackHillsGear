<template>
  <nav>
    <div class="logoBanner">
      <img class="logo" alt="Black Hills Gear Logo" src="/logoBadge.png" />
      <h1 class="logoText">Black Hills Gear</h1>
    </div>
    <div class="navButtons">
      <v-btn plain>Home</v-btn>
      <v-btn plain>Store</v-btn>
      <v-btn plain>About</v-btn>
      <v-btn plain>Contact</v-btn>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@800&display=swap');

nav {
  font-family: 'Playfair Display', serif;
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('/custerstatepark.jpg');
  background-position: center;
  background-size: 100%;
  display: flex;
  justify-content: space-between;
  height: 32vh;
  width: 100vw;
}

.navButtons {
  margin: 2.5em;
}

.logoBanner {
  display: flex;
  align-items: center;
  height: fit-content;
  width: fit-content;
}

.logo {
  max-height: 6vh;
  margin: 2em;
}

.logoText {
  font-size: 2em;
  margin-right: 1em;
}
</style>
