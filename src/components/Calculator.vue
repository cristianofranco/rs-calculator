<template>
  <div class="h-[566px] w-[356px] p-8 bg-[#2D2A37] calculator-shadow flex rounded-[48px]">
    <div class="w-[288px] h-[86px] mt-3 flex-col justify-end">
      <input class="w-full h-7 text-right text-lg px-5 bg-transparent border-none
       text-[#6B6B6B]" type="text">
      <div class="flex justify-between px-5">
        <img src="/equals.svg" alt="equals sign">
        <p class="text-4xl text-[white]">2</p>
      </div>
      <Buttons />
    </div>
  </div>
</template>

<script>
import Buttons from './Buttons.vue'
export default {
  components: {
    Buttons
  }
}
</script>
