<template>
  <div class="grid__col" :class="`grid__col--${this.size}`">
    <slot />
  </div>
</template>

<script>
export default {
  props: {
    size: {
      type: Number,
      default: 0
    }
  },
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
.grid {
  [class*='__col--'] {
    // applies gutters & styling to each column bar last.
    float: left;
    &:not(:last-child) {
      margin-right: $gutter-horizontal;
    }
  }

  &__col {
    background-color: $grid-col-color;
    color: $grid-col-font;
    &--1 {
      width: calc((100% / 12) - (#{$gutter-horizontal} * 11 / 12));
    }
    &--2 {
      width: calc((100% / 6) - (#{$gutter-horizontal} * 10 / 12));
    }
    &--3 {
      width: calc((100% / 4) - (#{$gutter-horizontal} * 9 / 12));
    }
    &--4 {
      width: calc((100% / 3) - (#{$gutter-horizontal} * 8 / 12));
    }
    &--5 {
      width: calc((100% / 2.4) - (#{$gutter-horizontal} * 7 / 12));
    }
    &--6 {
      width: calc((100% / 2) - (#{$gutter-horizontal} * 6 / 12));
    }
    &--7 {
      width: calc(
        (100% / 1.714285714285714) - (#{$gutter-horizontal} * 5 / 12)
      );
    }
    &--8 {
      width: calc((100% / 1.5) - (#{$gutter-horizontal} * 4 / 12));
    }
    &--9 {
      width: calc(
        (100% / 1.333333333333333) - (#{$gutter-horizontal} * 3 / 12)
      );
    }
    &--10 {
      width: calc((100% / 1.2) - (#{$gutter-horizontal} * 2 / 12));
    }
    &--11 {
      width: calc(
        (100% / 1.090909090909091) - (#{$gutter-horizontal} * 1 / 12)
      );
    }
    &--12 {
      width: 100%;
    }
  }
}
</style>
