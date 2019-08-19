<template>
  <div class="grid">
    <slot />
  </div>
</template>

<script></script>

<style lang="scss" scoped>
.grid {
  display: block;
  margin: 0 auto;
  max-width: $grid-width;
  text-align: center;
  @include clearfix;

  &:not(:last-child) {
    margin-bottom: $gutter-vertical;
  }
}
</style>
