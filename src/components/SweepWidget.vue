<template>
  <div id="62489-mxgut9zf" class="sw_container" ref="sweepWidget"></div>
</template>

<script>
export default {
  name: "SweepWidget",
  mounted() {
    const script = document.createElement("script");
    script.setAttribute("src", "https://sweepwidget.com/w/j/w_init.js");
    script.setAttribute("type", "text/javascript");
    this.$refs.sweepWidget.appendChild(script);
  },
};
</script>

<style></style>
