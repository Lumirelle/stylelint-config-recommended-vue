<style lang="scss">
a {
    color: v-bind(color);
    padding-right: math.div(4, 2);
}

// SCSS
.b {
    // stylelint-disable-next-line scss/at-if-no-null
    @if $x == null {
        color: red;
    }
}
@mixin my-mixin {
  color: blue
}

.c {
  @include my-mixin
}

$animation-duration: 300ms;
$animation-function: ease-in-out;
.d {
  transition: all $animation-duration $animation-function;
}

// Vue
:global(.foo),
::v-deep(.foo),
::v-slotted(.foo),
::v-global(.foo),
:deep(.foo),
:slotted(.foo) {
    color: red;
}

</style>