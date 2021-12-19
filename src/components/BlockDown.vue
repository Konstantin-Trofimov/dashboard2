<template>
  <div class="block-down"  v-on:click="stud_click">
    <svg class="block-down__icon d-md-none">
      <use href="@/assets/img/sprite.svg#block-down-icon"></use>
    </svg>

    <svg class="block-down__icon d-lg-none" width="29vw" height="17vw" viewBox="0 0 290 171" fill="none" xmlns="http://www.w3.org/2000/svg">
      <path d="M16.5 0H273.5L290 16.5V155.5L274.5 171H15.5L0 155.5V16.5L16.5 0Z" fill="#112054" fill-opacity="0.7"/>
      <path d="M1 16.9142L16.9142 1H273.086L289 16.9142V155.086L274.086 170H15.9142L1 155.086V16.9142Z" stroke="#217AFF" stroke-opacity="0.9" stroke-width="2"/>
    </svg>

    



    <div class="block-down__items">
      <div class="block-down__item first--item d-md-none">
        <p class="block-down__title">
          Трудоустройство <br />
          выпускников
        </p>

        <div class="block__down-wrap">
          <svg
              class="block-down__circle" width="4.167vw" height="4.167vw"
              viewBox="0 0 85 85" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="42.5" cy="42.5" r="37.5" stroke="#0E2D7B" stroke-width="6" stroke-dasharray="2 2"/>
            <path d="M42.6254 5.00014C51.8936 5.03114 60.8219 8.49319 67.6881 14.7185C74.5543 20.9437 78.872 29.4911 79.8082 38.7119C80.7444 47.9326 78.2329 57.1734 72.758 64.6517C67.2832 72.13 59.233 77.316 50.1602 79.2092C41.0875 81.1024 31.6351 79.5688 23.6263 74.9042C15.6176 70.2395 9.61996 62.7743 6.79039 53.9487C3.96082 45.123 4.49978 35.5622 8.30331 27.1104C12.1068 18.6587 18.9055 11.9149 27.3877 8.17984" stroke="#FB9B2B" stroke-width="9" stroke-dasharray="2 2"/>
            <circle cx="42.5" cy="42.5" r="28.5" stroke="#FB9B2B"/>
          </svg>

          <p class="block__down-val">91%</p>
        </div>

        <p class="block__down-label">QS WUR</p>
      </div>

      <div class="block-down__item second--item">
        <p class="block-down__title">Нагрузка преподавателей</p>

        <p class="block__down-label">Плановая <span>950676 <br class="d-md-none"> часов</span></p>

        <ProgressThird />

        <p class="block-down__percent">23.2%</p>
        <p class="block__down-label">Фактическая</p>
      </div>

      <div class="block-down__item third--item d-md-none">
        
        <img class="legend-data" src="../assets/img/down-block-diagramm.svg" alt="">

        <div class="block-graph__items">
          <div class="block-graph__item">
            <div class="block-graph__inf">
              <svg class="block-graph__icon" width="0.833vw" height="0.833vw">
                <use href="@/assets/img/sprite.svg#block-graph-icon1"></use>
              </svg>
              <span>Бакалавры</span>
            </div>
          </div>

          <div class="block-graph__item">
            <div class="block-graph__inf">
              <svg class="block-graph__icon" width="0.833vw" height="0.833vw">
                <use href="@/assets/img/sprite.svg#block-graph-icon2"></use>
              </svg>
              <span>Специалисты</span>
            </div>
          </div>

          <div class="block-graph__item">
            <div class="block-graph__inf">
              <svg class="block-graph__icon" width="0.833vw" height="0.833vw">
                <use href="@/assets/img/sprite.svg#block-graph-icon3"></use>
              </svg>
              <span>Магистры</span>
            </div>
          </div>
        </div>
      </div>

      <div class="block-down__item fourth--item">
        <div class="block-down__lists">
          <div class="block-down__list">
            <span>Очное</span>
            <div class="progress-fourth-line" style="width: 58%" data-text="30 770"></div>
            <!-- <ProgressFourth /> -->
          </div>

          <div class="block-down__list">
            <span>Очно-заочное</span>

            <div class="progress-fourth-line" style="width: 12%" data-text="5 505"></div>
            <!-- <ProgressFourth /> -->
          </div>

          <div class="block-down__list">
            <span>Заочное</span>

            <div class="progress-fourth-line" style="width: 23%" data-text="6 962"></div>
            <!-- <ProgressFourth /> -->
          </div>
        </div>

        <div class="block-down__lists">
          <div class="block-down__list">
            <span>Бюджет</span>

            <div class="progress-fourth-line" style="width: 16%" data-text="9 818"></div>
            <!-- <ProgressFourth /> -->
          </div>

          <div class="block-down__list">
            <span>Внебюджет</span>

            <div class="progress-fourth-line" style="width: 55%" data-text="33 419"></div>
            <!-- <ProgressFourth /> -->
          </div>
        </div>
      </div>

    </div>

    <div class="progress progress--right1 d-md-none">
      <p class="progress__text">01.12.2021</p>
      <svg
          width="5.208vw"
          height="0.625vw"
          viewBox="0 0 99 12" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M95 0H99L88 12H84L95 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M59 0H63L52 12H48L59 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M77 0H81L70 12H66L77 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M41 0H45L34 12H30L41 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M11 0H15L4 12H0L11 0Z" fill="#F79A2D" />
        <path d="M89 0H93L82 12H78L89 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M53 0H57L46 12H42L53 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M23 0H27L16 12H12L23 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M71 0H75L64 12H60L71 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M35 0H39L28 12H24L35 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M83 0H87L76 12H72L83 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M47 0H51L40 12H36L47 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M17 0H21L10 12H6L17 0Z" fill="#F79A2D"  fill-opacity="0.2"/>
        <path d="M65 0H69L58 12H54L65 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        <path d="M29 0H33L22 12H18L29 0Z" fill="#F79A2D" fill-opacity="0.2"/>
      </svg>
    </div>

    <div class="progress progress--left1 d-lg-none">
      <p class="progress__text">01.12.2021</p>
      <svg
          width="5.208vw"
          height="0.625vw"
          viewBox="0 0 100 12"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
          class="progress__icon"
      >
        <path d="M4.5 0H0.5L11.5 12H15.5L4.5 0Z" fill="#FB9B2B"  />
        <path
            d="M40.5 0H36.5L47.5 12H51.5L40.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M22.5 0H18.5L29.5 12H33.5L22.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M58.5 0H54.5L65.5 12H69.5L58.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M88.5 0H84.5L95.5 12H99.5L88.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M10.5 0H6.5L17.5 12H21.5L10.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M46.5 0H42.5L53.5 12H57.5L46.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M76.5 0H72.5L83.5 12H87.5L76.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M28.5 0H24.5L35.5 12H39.5L28.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M64.5 0H60.5L71.5 12H75.5L64.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M16.5 0H12.5L23.5 12H27.5L16.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M52.5 0H48.5L59.5 12H63.5L52.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M82.5 0H78.5L89.5 12H93.5L82.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M34.5 0H30.5L41.5 12H45.5L34.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
        <path
            d="M70.5 0H66.5L77.5 12H81.5L70.5 0Z"
            fill="#FB9B2B"
            fill-opacity="0.2"
        />
      </svg>
    </div>

    <div class="progress progress--right1 d-lg-none">
      <p class="progress__text">92% год</p>
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

  </div>
</template>

<script>
import ProgressFourth from './ProgressFourth.vue'
import ProgressThird from './ProgressThird'
export default {
  components: {
    ProgressThird,
    ProgressFourth,
  },
  methods: {
    stud_click: function() {
      this.connection.send('stud_click')
    },
  },
  created() {
    const ws_url = 'ws://195.211.102.43:8999'
    this.connection = new WebSocket(ws_url)

    this.connection.onerror = error => {
      console.log(error)
    }
  },
}
</script>

<style lang="scss" scoped>

.progress-fourth-line {
  background-color: #217aff;
  height: 0.208vw;
  position: relative;
  display: flex;
  justify-content: flex-start;
  padding-left: 0.05vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    height: 0.4vw;
  }

  &:after {
    content: '';
    position: absolute;
    right: -0.3vw;
    top: 50%;
    width: 0.521vw;
    height: 0.521vw;
    transform: translateY(-50%);
    background: url('../assets/img/triangle.svg') no-repeat center/contain;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      height: 0;
      width: 0;
      background: none;
    }
  }

  &:before {
    content: attr(data-text);
    font-size: 0.521vw;
    position: relative;
    top: -0.8vw;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      font-size: 0.63vw;
      top: -1.7vw;
    }
  }
}

.block-down {
  cursor: pointer;
}

.block-down__graph {
  width: 9.635vw;
  height: 5.313vw;
}

.block-down__lists {
  width: 11.5vw;
  padding-bottom: 0.469vw;
  margin-bottom: 0.4vw;
  position: relative;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    padding-right: 2vw;
    padding-top: 0.6vw;
    width: 16vw;
  }

  &:first-of-type:after {
    content: '';
    position: absolute;
    bottom: 0;
    left: 1.042vw;
    right: 0;
    border-bottom: 1px dashed rgba(33, 122, 255, 0.7);
    @media (min-width: 768px) and (max-width: 1199.98px) {
      right: 2vw;
      left: 0.5vw;
    }
  }
}

.block-down__list {
  display: flex;
  align-items: center;
  line-height: 1vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    line-height: 2.5vw;
  }

  span {
    font-size: 0.677vw;
    flex: 0 0 auto;
    width: 4.167vw;
    text-align: right;
    margin-right: 0.208vw;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      font-size: 1vw;
      width: 5.2vw;
      margin-top: -0.4vw;
    }
  }
}

.block-graph {
  position: absolute;
  top: 1.2vw;
  left: 0.3vw;
}

.block-graph__items {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  max-width: 11.5vw;
  transform: translate(-0.8vw, 0.1vw);
}

.block-graph__item {
  padding: 0 0.417vw;
}

.block-graph__inf {
  display: flex;
  align-items: center;
  font-size: 0.677vw;
  line-height: 0.833vw;
  letter-spacing: 0.03em;
}

.block-graph__icon {
  margin-right: 0.521vw;
  flex: 0 0 auto;
}

.block-down {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 41.198vw;
  height: 8.542vw;
  z-index: 1;
  bottom: 2vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    width: 29vw;
    height: 17vw;
    bottom: auto;
    position: relative;
    left: auto;
    transform: none;
  }
}

.block-down__percent {
  font-size: 1.146vw;
  line-height: 1.042vw;
  color: #217aff;
  margin-bottom: 0.104vw;
  padding-top: 0.2vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1.5vw;
    line-height: 2.5vw;
    padding-top: 0;
  }
}

.block__down-label {
  letter-spacing: 0.1em;
  text-transform: uppercase;
  //font-size: 0.469vw;
  font-size: 0.7vw;
  line-height: 0.829vw;
  //line-height: 0.729vw;
  color: #627dae;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 0.9vw;
    margin-bottom: 0.5vw;
  }

  span {
    font-size: 0.677vw;
    line-height: 0.833vw;
    letter-spacing: 0.03em;
    text-transform: none;
    color: #fff;
    position: absolute;
    padding-left: 3px;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      font-size: 0.9vw;
      position: relative;
      padding-left: 0;
    }
  }
}

.block__down-wrap {
  position: relative;
}

.block__down-val {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 1.146vw;
  line-height: 1.042vw;
  color: #f79a2d;

  &:after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    width: 2.969vw;
    height: 2.969vw;
    transform: translate(-50%, -50%);
    border: 1px solid #fb9b2b;
    border-radius: 50%;
  }
}

.block-down__icon {
  width: 41.198vw;
  height: 8.542vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    height: 17vw;
    width: 29vw;
  }
}

.block-down__title {
  font-size: 0.677vw;
  line-height: 0.833vw;
  text-align: center;
  letter-spacing: 0.03em;
  margin-bottom: 0.321vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1.5vw;
    line-height: 2vw;
    text-align: left;
  }
}

.block-down__items {
  position: absolute;
  top: 0;
  left: 0;
  display: flex;

}

.block-down__item {
  display: flex;
  flex-direction: column;
  position: relative;
}

.first--item {
  padding-left: 1.5vw;
  padding-top: 0.8vw;
  padding-right: 0.938vw;

  &:before {
    content: '';
    position: absolute;
    top: 1.6vw;
    bottom: 0.8vw;
    right: 0;
    border: 1px dashed rgba(33, 122, 255, 0.7);
  }
}

.second--item {
  padding-top: 1.3vw;
  padding-left: 0.781vw;
  margin-right: 1.4vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    padding-left: 1.5vw;
  }
}

.third--item {
  padding-top: 1.1vw;
}

.block-down__circle {
  margin-left: auto;
  margin-right: auto;
}

.fourth--item {
  padding-top: 1vw;
}

.legend-data {
  height: 5.5vw;
  width: 12vw;
  
}
</style>
