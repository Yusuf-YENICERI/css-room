<template>
  <div
      class="square"
      :style="`--width: ${width}px; --height: ${height}px; --bg: ${bg}; --rotateX: ${rotatex}deg; --rotateY: ${rotatey}deg; --rotateZ: ${rotatez}deg; --translateX: ${translatex}px; --translateY: ${translatey}px; --translateZ: ${translatez}px`"
  >
    <div class="front side"></div>
    <div :style="`--thickness: ${-thickness}px;`"
         class="back side"></div>
    <div class="left side" :style="`--thickness: ${thickness}px; --width: ${-width / 2 + 1}px;`"></div>
    <div class="right side" :style="`--thickness: ${thickness}px; --width: ${-width / 2 + 1}px;`"></div>
    <div class="top side" :style="`--thickness: ${thickness}px; --width: ${width}px; --translate: ${height / 2}px`"></div>
    <div class="bottom side" :style="`--thickness: ${thickness}px; --width: ${width}px; --translate: ${height / 2}px`"></div>

    <!-- 1px for remove little space between sides -->
  </div>
</template>

<script>
export default {
  name: 'Square',
  props: ['rotatex', 'rotatey', 'rotatez', 'translatex', 'translatey', 'translatez', 'width', 'height', "bg", "thickness"],
};
</script>
