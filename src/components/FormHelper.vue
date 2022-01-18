<template lang="pug">
  .Container
    h1 Please fill out below from
    form
      .From__header
        slot(name="form-header")
      .From__fields
        slot(name="form-fields")
      .Form__controller
        slot(name="form-controller")

</template>
<style scoped>
/* 여기에 적절한 스타일을 넣으면 재사용할 수 있음 */
</style>
