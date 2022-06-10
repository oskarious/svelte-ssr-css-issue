<script>
  import "../app.css";
</script>

<h1 class="a-css-class">This should be styled, but isn't during SSR</h1>
<h2 style="color: green; font-size: 72px">This, with inlined styles, looks correct</h2>
<slot />

<style global>
  @import '../app.css';
</style>