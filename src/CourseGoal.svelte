<script>
  export let courseGoal;

  $: textColorRed = courseGoal.includes("!");
</script>

<style>
  .textRed {
    color: red;
  }
</style>

<h1 class:textRed={textColorRed}>{courseGoal}</h1>
