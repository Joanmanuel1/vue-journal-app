<template>
  <div class="entry-container mb-3 pointer p-2" @click="$router.push({name:'entry', params:{id: 10}})">
    <div class="entry-title d-flex">
      <span class="text-succes fs-5 fw-bold">02</span>
      <span class="mx-1 fs-5"> Septiembre</span>
      <span class="mx-2 fw-light">2022, Viernes</span>
    </div>

    <div class="entry-description">
      Cillum fugiat Lorem ipsum consectetur laboris. Tempor laborum aliquip
      laboris est sunt. Amet sint sint quis officia mollit culpa aute dolore
      duis aute qui fugiat commodo.
    </div>
  </div>
</template>

<script>
export default {

};
</script>

<style lang="scss" scoped>
.entry-container {
  border-bottom: 1px solid darkgreen;
  transition: 0.2s all ease-in;

  &:hover {
    background-color: lighten($color: grey, $amount: 45);
    transition: 0.2s all ease-in;
  }

  .entry-description{
    font-size:12px;
  }
}

</style>