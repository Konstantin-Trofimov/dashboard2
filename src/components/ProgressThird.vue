<template>
  <svg class="plan-svg"
      width="3.5vw" height="1.388vw"
      viewBox="0 0 63 20" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M63 10L-1.01328e-06 10" stroke="#0E2D7B" stroke-width="20" stroke-dasharray="3 2"/>
    <svg x="-1.5">
      <path d="M14 10H1.90743e-07" stroke="#217AFF" stroke-width="20" stroke-dasharray="3 2"/>
    </svg>
  </svg>
    


</template>

<script>
export default {
  name: 'ProgressThird',
}
</script>

<style lang="scss" scoped>
.line-third {
  width: 6.385vw;
  height: 1.042vw;
  margin-top: 0.156vw;
  margin-bottom: 0.313vw;
}
.plan-svg{
  @media (min-width: 768px) and (max-width: 1199.98px) {
    height: 4vw;
    width: 10vw;
  }
}
</style>
