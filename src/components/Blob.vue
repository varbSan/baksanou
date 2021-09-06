<template>
  <div class="blob">
    <img
      class="profile-picture"
      src="../assets/profile-picture.png"
      alt="Profile Picture"
    />
    <svg
      id="visual"
      viewBox="0 0 900 900"
      width="100%"
      height="100%"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      version="1.1"
    >
      <rect x="0" y="0" width="100%" height="100%" fill="#006b5e"></rect>
      <g transform="translate(484.5332216626009 460.3007594262465)">
        <path
          d="M120 -220.5C161 -184.2 203.5 -163.1 229.7 -128.9C256 -94.7 266 -47.3 264.8 -0.7C263.7 46 251.3 92 231.4 137.2C211.5 182.4 184 226.7 144.2 244.2C104.3 261.7 52.2 252.4 -4.4 260C-61 267.7 -122 292.3 -179 284.7C-236 277.1 -289.1 237.3 -304.4 184.5C-319.7 131.7 -297.4 65.8 -305.3 -4.6C-313.2 -75 -351.5 -150 -324.4 -182.5C-297.3 -215 -204.9 -204.9 -140 -227.4C-75 -249.9 -37.5 -305 1 -306.7C39.5 -308.4 79 -256.8 120 -220.5"
          fill="#669b90"
          id="blob1"
        ></path>
      </g>
      <g 
        transform="translate(489.03020771318756 400.24503911219267)"
        style="visibility: hidden" 
      ><path
          d="M121.8 -195.4C168.5 -183.9 224.6 -173 247 -140.5C269.4 -108 258.2 -54 271 7.4C283.9 68.8 320.8 137.7 305.1 181.8C289.4 226 221.2 245.5 161.6 286.1C102 326.7 51 388.3 -4.7 396.6C-60.5 404.8 -121 359.6 -185.7 321.9C-250.3 284.2 -319.2 254.1 -354.9 201.7C-390.7 149.3 -393.3 74.7 -378.5 8.6C-363.6 -57.5 -331.2 -115 -298.3 -172.3C-265.4 -229.6 -231.9 -286.7 -182.1 -296.5C-132.3 -306.2 -66.2 -268.6 -14.3 -243.8C37.5 -219 75 -206.9 121.8 -195.4"
          fill="#669b90"
          id="blob2"
        ></path>
      </g>
    </svg>
  </div>
</template>

<script setup>
import { onMounted } from '@vue/runtime-core'
import KUTE from 'kute.js'

onMounted(() => {
  const tween = KUTE.fromTo(
    '#blob1',
    { path: '#blob1' },
    { path: '#blob2' },
    { repeat: 999, duration: 3000, yoyo: true }
  )

  tween.start()
})
</script>

<style lang="scss" scoped>
.blob {
  position: relative;
  min-width: 90%;
  max-width: 100%;
}

.profile-picture {
  width: 50%;
  border-radius: 50%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
</style>
