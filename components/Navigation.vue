<template>
  <div class="backgroundImage">
    <nav>
      <img class="logo" alt="Black Hills Gear Logo" src="/BHG-Logo_White.svg" />
      <div class="navButtons">
        <v-btn plain>Home</v-btn>
        <v-btn plain>Store</v-btn>
        <v-btn plain>About</v-btn>
        <v-btn plain>Contact</v-btn>
      </div>
    </nav>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@800&display=swap');

nav {
  font-family: 'Playfair Display', serif;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  height: 24vh;
  width: 100vw;
}

.navButtons {
  margin: 2.5em;
}

.backgroundImage {
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)),
    url('/custerstatepark.jpg');
  background-position: center;
  background-size: 100%;
  height: 24vh;
  width: 100vw;
}

.logoBanner {
  display: flex;
  align-items: center;
  height: fit-content;
  width: fit-content;
}

.logo {
  max-height: 16vh;
  margin: 2em;
}

.logoText {
  font-size: 2em;
  margin-right: 1em;
}
</style>
