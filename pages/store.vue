<script>
export default {
  name: 'App',
}
</script>
<template>
  <!--START SERVICES-->
  <section class="section pt-5" id="services">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 offset-lg-2">
          <h1 class="section-title text-center">Products</h1>
          <div class="ec-cart-widget"></div>
          <div id="app">
            <Ecwid :storeId="11279422" />
          </div>

          <div class="section-title-border margin-t-20"></div>
        </div>
      </div>
    </div>
  </section>
  <!--START SERVICES-->
</template>
