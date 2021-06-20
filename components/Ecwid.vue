<template>
  <div :id="`my-store-${storeId}`"></div>
</template>
<script>
function injectEcwidScript(storeId) {
  const ecwidScript = document.createElement('script')
  ecwidScript.setAttribute('type', 'text/javascript')
  ecwidScript.setAttribute('charset', 'utf-8')
  ecwidScript.setAttribute('data-cfasync', 'false')
  ecwidScript.setAttribute(
    'src',
    `https://app.ecwid.com/script.js?${storeId}&data_platform=code&data_date=2020-02-17`
  )
  ecwidScript.onload = injectEcwidProductBrowser(storeId)
  document.head.appendChild(ecwidScript)
}
function injectEcwidProductBrowser(storeId) {
  return function () {
    const ecwidBrowserScript = document.createElement('script')
    ecwidBrowserScript.setAttribute('type', 'text/javascript')
    ecwidBrowserScript.setAttribute('charset', 'utf-8')
    ecwidBrowserScript.text = `xProductBrowser("categoriesPerRow=3","views=grid(20,3) list(60) table(60)","categoryView=grid","searchView=list","id=my-store-${storeId}");`
    document.head.appendChild(ecwidBrowserScript)
  }
}
export default {
  name: 'Ecwid',
  props: {
    storeId: {
      type: Number,
      default: 1003,
    },
  },
  mounted() {
    injectEcwidScript(this.storeId)
  },
}
</script>
<style></style>
