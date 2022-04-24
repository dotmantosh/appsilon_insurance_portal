<template>
  <div class="header">
    <ul class="header__list">
      <li class="header__list--item">Overview</li>
      <li class="header__list--item">Policy</li>
      <li class="header__list--item selected">Reports</li>
    </ul>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="scss">
.header{
  background-color: #fff;
  border-top-right-radius: 20px;
  width: 100%;
  height: 8.7rem;
  box-shadow:3px 5px 15px rgba($color: #000000, $alpha: 0.1);
  &__list{
    display: flex;
    align-items: center;
    margin-left: 5.5rem;
    height: 100%;
    list-style: none;
    padding: 0;

    &--item{
      margin-right: 3.5rem;
      font-size: 1.5rem;
      line-height: 21px;
      cursor: pointer;
    }
    .selected{
      color: var(--app-purple-1);
      font-weight: 600;
    }
  }
}


</style>
  