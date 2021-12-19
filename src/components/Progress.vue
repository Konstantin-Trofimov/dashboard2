<template>
  <div class="progress">
    <p class="progress__text">{{ progress }}</p>
    <svg
        width="5.208vw"
        height="0.625vw"
        viewBox="0 0 100 12" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M95.5 0H99.5L88.5 12H84.5L95.5 0Z" fill="#F79A2D"/>
      <path d="M59.5 0H63.5L52.5 12H48.5L59.5 0Z" fill="#F79A2D"/>
      <path d="M77.5 0H81.5L70.5 12H66.5L77.5 0Z" fill="#F79A2D"/>
      <path d="M41.5 0H45.5L34.5 12H30.5L41.5 0Z" fill="#F79A2D"/>
      <path d="M11.5 0H15.5L4.5 12H0.5L11.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
      <path d="M89.5 0H93.5L82.5 12H78.5L89.5 0Z" fill="#F79A2D"/>
      <path d="M53.5 0H57.5L46.5 12H42.5L53.5 0Z" fill="#F79A2D"/>
      <path d="M23.5 0H27.5L16.5 12H12.5L23.5 0Z" fill="#F79A2D"/>
      <path d="M71.5 0H75.5L64.5 12H60.5L71.5 0Z" fill="#F79A2D"/>
      <path d="M35.5 0H39.5L28.5 12H24.5L35.5 0Z" fill="#F79A2D"/>
      <path d="M83.5 0H87.5L76.5 12H72.5L83.5 0Z" fill="#F79A2D"/>
      <path d="M47.5 0H51.5L40.5 12H36.5L47.5 0Z" fill="#F79A2D"/>
      <path d="M17.5 0H21.5L10.5 12H6.5L17.5 0Z" fill="#F79A2D" />
      <path d="M65.5 0H69.5L58.5 12H54.5L65.5 0Z" fill="#F79A2D"/>
      <path d="M29.5 0H33.5L22.5 12H18.5L29.5 0Z" fill="#F79A2D"/>
    </svg>

  </div>
</template>

<script>
export default {
  name: "Progress",
  props: ["progress"],
};
</script>

<style lang="scss">
.progress {
  position: absolute;
  z-index: 1;
}

.progress__text {
  font-weight: 700;
  font-size: 0.521vw;
  line-height: 1.042vw;
  color: #fb9b2b;
  padding-right: 0.5vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 0.75vw;
    padding: 0 0.3vw;
  }
}
</style>
