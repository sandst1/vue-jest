<template>
  <div :class="$style.testPcss"></div>
</template>

<style module lang="postcss">
  @import "./styles/transitions";

  .testPcss {
    background-color: purple;
  }
</style>

<style module lang="pcss">
  /* This syntax is for postcss-custom-properties */
  --primary-color: green;

  /* This syntax is for postcss-nesting, but invalid as Pure CSS */
  body {
    @media screen {
      background-color: grey;
    }
  }
</style>
