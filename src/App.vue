<template>
  <div class="room">
    <div class="roomSkeleton">
      <Square width="500" height="500"
              rotatex="0" rotatey="0" rotatez="0"
              translatex="-125" translatey="0" translatez="-125"
              bg="linear-gradient(to right, #eee, #888)" thickness="20"></Square>
      <Square width="500" height="500"
              rotatex="180" rotatey="-90" rotatez="0"
              translatex="-125" translatey="0" translatez="-125"
              bg="linear-gradient(to right, #eee, #888)" thickness="20"></Square>
      <Square width="520" height="520"
              rotatex="90" rotatey="0" rotatez="0"
              translatex="-115" translatey="115" translatez="-250"
              bg="linear-gradient(to top right, #26110D, #120806)" thickness="20"></Square>
      <!--
      for floor :
        width & height =  wallWidth + thickness
        translateX & translateY = wallWidth / 4 - thickness / 2
      -->
    </div>
    <div class="roomItems">
      <div class="desk">
        <Square width="300" height="16"
                rotatex="0" rotatey="90" rotatez="0"
                translatex="-125" translatey="100" translatez="125"
                bg="linear-gradient(to bottom left, black, #222)" thickness="125"></Square>
        <Square width="16" height="150"
                rotatex="0" rotatey="0" rotatez="0"
                translatex="8" translatey="175" translatez="0"
                bg="linear-gradient(to top right, black, #222)" thickness="16"></Square>
        <Square width="16" height="150"
                rotatex="0" rotatey="0" rotatez="0"
                translatex="8" translatey="175" translatez="268"
                bg="linear-gradient(to top right, black, #222)" thickness="16"></Square>
      </div>
      <span class="wallText">WoxeOfficial</span>
      <div class="computer">
        <div class="keyboard">
          <Square width="80" height="4"
                  rotatex="0" rotatey="0" rotatez="0"
                  translatex="50" translatey="90" translatez="174"
                  bg="gray" thickness="90"></Square>

          <Square width="70" height="1"
                  rotatex="0" rotatey="0" rotatez="0"
                  translatex="50" translatey="88" translatez="169"
                  bg="darkgray" thickness="80"></Square>
        </div>

        <div class="screen">
          <Square width="80" height="4"
                  rotatex="0" rotatey="0" rotatez="0"
                  translatex="50" translatey="90" translatez="174"
                  bg="gray" thickness="90"></Square>

          <Square width="70" height="1"
                  rotatex="0" rotatey="0" rotatez="0"
                  translatex="50" translatey="88" translatez="169"
                  bg="#1D1D1DFF" thickness="80"></Square>
        </div>
      </div>
      <div class="wallLogo">

      </div>
    </div>

  </div>
</template>

<script>
import Square from "./components/Square"

export default {
  name: 'App',
  components: {
    Square,
  },
};
</script>

<style>

</style>
