<template>
  <div class="finance-tablet">

    <div class="finance-tablet-left d-lg-none">
      <svg  width="8.5vw" height="17vw" viewBox="0 0 81 171" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M16 0H81V16.5V155.5V171H16L0 155.5V16.5L16 0Z" fill="#112054" fill-opacity="0.7"/>
        <path d="M1 16.9052L16.4233 1H80V16.5V155.5V170H16.405L1 155.076V16.9052Z" stroke="#217AFF" stroke-opacity="0.9" stroke-width="2"/>
      </svg>

      <div class="cirlce-block__contains">
        <div class="cirlce-block__wrap">
          <span class="circle-block__value">
            3,77
            <svg class="circle-block__icon circle-block__icon__down" width="0.781vw" height="0.781vw">
              <use href="../assets/img/sprite.svg#icon2"></use>
            </svg>
          </span>

        </div>
        <p class="circle-block__text">Денежные <br />Средства, млрд.</p>
      </div>

      <div class="cirlce-block__contains">
        <div class="cirlce-block__wrap">
          <span class="circle-block__value">
            5,75
            <!-- <svg class="circle-block__icon circle-block__icon__down" width="0.781vw" height="0.781vw">
              <use href="../assets/img/sprite.svg#icon2"></use>
            </svg> -->
            <svg style="top: 0.5vw" class="circle-block__icon arrow-cash circle-block__icon__top" width="0.781vw" height="0.781vw">
                <use href="../assets/img/sprite.svg#icon1"></use>
              </svg>
          </span>

        </div>
        <p class="circle-block__text">Касса, млн.</p>
      </div>
    </div>

    <div class="finance-block" id="fin_click" v-on:click="fin_click">
      <svg class="finance-block__bg d-md-none" width="22.865vw" height="22.135vw">
        <use href="@/assets/img/sprite.svg#finance-container"></use>
      </svg>

      <svg class="finance-block__bg d-lg-none" width="52.2vw" height="17vw" viewBox="0 0 522 171" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 0H507.88L522 16.5V155.5L508.736 171H13.2639H0V16.5V0Z" fill="#112054" fill-opacity="0.7"/>
        <path d="M1 1H507.42L521 16.8694V155.131L508.276 170H13.2639H1V16.5V1Z" stroke="#217AFF" stroke-opacity="0.9" stroke-width="2"/>
      </svg>

      <div class="finance-block__top">
        <p class="finance-block__title">Финансы</p>

        <div class="finance-block__text">
          <p>7 062 872 552 руб.</p>
          <span>Основные средства на балансе</span>
        </div>
      </div>

      <div class="finance-block__bottom">
        <img
            class="finance-block__graph d-md-none"
            src="@/assets/img/graph_finance.svg"
            alt=""
        />

        <div class="finance-block__row">
          <div class="finance-block__circle">
            <div class="circle-wrap">
              <svg class="d-md-none"
                  width="6.563vw"
                  height="6.510vw"
                  viewBox="0 0 126 125"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
              >
                <path
                    d="M62.8976 5C53.4417 5 44.1317 7.33203 35.7923 11.7895C27.4529 16.247 20.3415 22.6924 15.0881 30.5547C9.83465 38.417 6.6013 47.4536 5.67446 56.864C4.74762 66.2744 6.15588 75.7682 9.77451 84.5043C13.3931 93.2404 19.1104 100.949 26.42 106.948C33.7295 112.947 42.4056 117.05 51.6799 118.895C60.9541 120.74 70.5402 120.269 79.5889 117.524C88.6377 114.779 96.8699 109.845 103.556 103.159L91.3348 90.9372C86.6582 95.6137 80.9006 99.0648 74.5717 100.985C68.2429 102.904 61.5383 103.234 55.0518 101.944C48.5652 100.653 42.497 97.7832 37.3846 93.5876C32.2723 89.392 28.2735 84.0003 25.7426 77.8901C23.2117 71.7799 22.2267 65.1399 22.875 58.5581C23.5232 51.9764 25.7847 45.656 29.459 40.157C33.1333 34.658 38.1071 30.15 43.9398 27.0324C49.7724 23.9148 56.284 22.2837 62.8976 22.2837V5Z"
                    fill="#217AFF"
                />
                <path
                    d="M107.092 106.694C115.833 97.9534 121.785 86.817 124.197 74.6931C126.608 62.5693 125.371 50.0027 120.64 38.5823C115.91 27.1619 107.899 17.4007 97.6207 10.5331C87.3427 3.66556 75.2589 -1.47407e-07 62.8976 0V19.8203C71.3388 19.8203 79.5905 22.3234 86.6091 27.0131C93.6278 31.7028 99.0981 38.3685 102.328 46.1672C105.559 53.9659 106.404 62.5473 104.757 70.8264C103.11 79.1054 99.0455 86.7102 93.0767 92.6791L107.092 106.694Z"
                    fill="#2BD6FB"
                />
                <rect
                    x="104.571"
                    y="23.571"
                    width="7"
                    height="7"
                    transform="rotate(-90 104.571 23.571)"
                    fill="white"
                    stroke="#2BD6FB"
                    stroke-width="3"
                />
                <rect
                    x="18.787"
                    y="105.785"
                    width="7"
                    height="7"
                    transform="rotate(-88.7585 18.787 105.785)"
                    fill="white"
                    stroke="#2E81FE"
                    stroke-width="3"
                />
              </svg>

              <svg class="d-lg-none"
                   width="8vw"
                   height="8vw"
                   viewBox="0 0 94 94" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="47.5" cy="46.5" r="34" stroke="#217AFF"/>
                <path d="M80.234 80.234C86.8071 73.6609 91.2834 65.2864 93.0969 56.1692C94.9104 47.0521 93.9797 37.602 90.4223 29.0139C86.865 20.4258 80.8409 13.0854 73.1118 7.92093C65.3827 2.7565 56.2957 -1.1085e-07 47 0V7.05C54.9014 7.05 62.6253 9.39303 69.195 13.7828C75.7648 18.1726 80.8853 24.4119 83.909 31.7118C86.9327 39.0117 87.7239 47.0443 86.1824 54.7939C84.6409 62.5434 80.836 69.6618 75.2489 75.2489L80.234 80.234Z" fill="#2BD6FB"/>
                <path d="M47.5 0C39.853 9.11892e-08 32.3241 1.8859 25.5801 5.49066C18.836 9.09542 13.0851 14.3078 8.83666 20.666C4.58823 27.0242 1.97344 34.3321 1.22391 41.9422C0.474373 49.5523 1.61323 57.2299 4.5396 64.2948C7.46597 71.3596 12.0895 77.5938 18.0007 82.445C23.9119 87.2962 30.9283 90.6147 38.4283 92.1065C45.9283 93.5984 53.6805 93.2175 60.9982 90.9977C68.3159 88.7779 74.9732 84.7877 80.3805 79.3805L75.4484 74.4484C70.8522 79.0445 65.1935 82.4362 58.9735 84.3231C52.7535 86.2099 46.1641 86.5336 39.789 85.2655C33.414 83.9975 27.4501 81.1767 22.4256 77.0532C17.4011 72.9297 13.4711 67.6307 10.9837 61.6256C8.49625 55.6204 7.52822 49.0945 8.16532 42.6259C8.80243 36.1572 11.025 29.9456 14.6362 24.5411C18.2473 19.1366 23.1356 14.7061 28.868 11.6421C34.6005 8.57802 41.0001 6.975 47.5 6.975V0Z" fill="#217AFF"/>
              </svg>

              <p class="circle-wrap__val1 d-md-none">1 324 520 306</p>

              <p class="circle-wrap__val2 d-md-none">1 838 931 834</p>

              <p class="circle-wrap__value">Фонд<br />оплаты<br />труда</p>
            </div>
          </div>

          <div class="finance-block__list">

            <div class="finance-block__item">
              <div class="finance-block__inf">
                

                  <svg style="top: 3vw" width="0.833vw" height="0.833vw" class="finance-block__icon">
                  <use href="@/assets/img/sprite.svg#block-graph-icon6"></use>
                </svg>


                <span>
                  <span class="d-lg-none darkblue" :style="{'color' : '#2BD6FB'}">
                    1 324 520 306
                  </span>
                  Из средств бюджета</span>
              </div>
            </div>

            <div class="finance-block__item">
              <div class="finance-block__inf">
                  <svg style="{top: 2vw, left: 0.5vw}" width="0.833vw" height="0.833vw" class="finance-block__icon">
                  <use href="@/assets/img/sprite.svg#block-graph-icon1"></use>
                </svg>

              
                <span>
                  <span class="d-lg-none blue" :style="{'color' : '#217AFF'}">
                    1 838 931 834
                  </span>
                  Из средств от иной <br />
                приносящей доход <br />
                деятельности
              </span>
              </div>
            </div>

          </div>
        </div>

        <div class="finance-block__row">
          <div class="finance-block__circle sec">
            <div class="circle-wrap">
              <svg class="d-md-none"
                  width="6.771vw"
                  height="6.771vw"
                  viewBox="0 0 130 131"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
              >
                <path
                    d="M112.119 95.9138C119.072 85.118 122.117 72.2656 120.744 59.4979C119.372 46.7303 113.667 34.8182 104.578 25.7464L96.3156 34.0243C103.512 41.207 108.029 50.6386 109.115 60.7477C110.202 70.8568 107.792 81.0329 102.286 89.5807L112.119 95.9138Z"
                    fill="#FB9B2B"
                />
                <path
                    d="M64.8976 8C54.9251 8 45.1241 10.5936 36.4569 15.5262C27.7897 20.4588 20.5545 27.5607 15.4615 36.1347C10.3685 44.7086 7.59303 54.4597 7.40753 64.4304C7.22203 74.4012 9.6329 84.2487 14.4034 93.0062C19.1739 101.764 26.14 109.13 34.6177 114.381C43.0954 119.633 52.7932 122.589 62.7588 122.96C72.7243 123.331 82.6151 121.104 91.4597 116.497C100.304 111.89 107.799 105.062 113.207 96.6839L98.686 87.3104C94.9033 93.1705 89.6615 97.946 83.4755 101.168C77.2894 104.39 70.3717 105.948 63.4017 105.688C56.4316 105.429 49.6489 103.361 43.7195 99.6882C37.79 96.0152 32.9178 90.8632 29.5813 84.7382C26.2447 78.6131 24.5585 71.7256 24.6883 64.7519C24.818 57.7782 26.7592 50.9582 30.3213 44.9615C33.8834 38.9648 38.9439 33.9976 45.0058 30.5477C51.0677 27.0978 57.9227 25.2837 64.8976 25.2837V8Z"
                    fill="#FD6A6A"
                />
                <path
                    d="M109.092 21.3058C97.3708 9.58482 81.4737 3.00002 64.8976 3L64.8976 22.8203C76.217 22.8203 87.0727 27.3169 95.0767 35.3209L109.092 21.3058Z"
                    fill="#FFC01D"
                />
                <rect
                    x="87.3742"
                    y="13.6751"
                    width="7"
                    height="7"
                    transform="rotate(-115.824 87.3742 13.6751)"
                    fill="white"
                    stroke="#FFC01D"
                    stroke-width="3"
                />
                <rect
                    x="23.4808"
                    y="26.4784"
                    width="7"
                    height="7"
                    transform="rotate(-88.5032 23.4808 26.4784)"
                    fill="white"
                    stroke="#FD6A6A"
                    stroke-width="3"
                />
                <rect
                    x="114.271"
                    y="91.6378"
                    width="7"
                    height="7"
                    transform="rotate(-114.55 114.271 91.6378)"
                    fill="white"
                    stroke="#FB9B2B"
                    stroke-width="3"
                />
              </svg>

              <svg
                  class="d-lg-none circle-finance-right"
                  width="8vw"
                  height="8vw"
                  viewBox="0 0 111 111" fill="none" xmlns="http://www.w3.org/2000/svg">
                <circle cx="55.9723" cy="55.9723" r="34" stroke="#FD6A6A"/>
                <path d="M89.9412 21.9124C80.9394 13.0045 68.7305 8.00001 56.0001 8L56.0001 15.125C66.8209 15.125 77.1985 19.3788 84.85 26.9506L89.9412 21.9124Z" fill="#FFC01D"/>
                <path d="M96.0124 81.7606C101.908 72.6067 104.489 61.7089 103.326 50.883C102.162 40.057 97.3245 29.9566 89.6183 22.2645L84.5714 27.3206C91.1217 33.8589 95.2338 42.4443 96.2228 51.6463C97.2117 60.8484 95.0178 70.1115 90.0064 77.8923L96.0124 81.7606Z" fill="#FB9B2B"/>
                <path d="M56.5 9C48.2619 9 40.1654 11.1426 33.0056 15.2173C25.8457 19.2921 19.8687 25.1589 15.6615 32.2417C11.4543 39.3245 9.16149 47.3797 9.00825 55.6164C8.85501 63.8531 10.8466 71.9881 14.7875 79.2225C18.7283 86.4569 24.4829 92.5419 31.4862 96.8802C38.4896 101.218 46.5008 103.661 54.7332 103.967C62.9656 104.274 71.1362 102.434 78.4427 98.628C85.7491 94.8224 91.9402 89.182 96.4079 82.2606L90.4218 78.3965C86.6242 84.2797 81.3617 89.0741 75.1513 92.3088C68.9408 95.5436 61.9958 97.1075 54.9982 96.8471C48.0006 96.5866 41.1911 94.5107 35.2383 90.8232C29.2855 87.1357 24.3941 81.9633 21.0443 75.8141C17.6946 69.6649 16.0018 62.7502 16.132 55.749C16.2623 48.7478 18.2112 41.9008 21.7873 35.8804C25.3634 29.86 30.4439 24.8733 36.5297 21.4097C42.6156 17.9462 49.4976 16.125 56.5 16.125L56.5 9Z" fill="#FD6A6A"/>
              </svg>
              <p class="circle-wrap__val3 d-md-none">3 163 452 141</p>

              <p class="circle-wrap__val4 d-md-none">60 007 599</p>

              <p class="circle-wrap__val5 d-md-none">83 112 948</p>

              <p class="circle-wrap__value is--orange">Затраты</p>
            </div>
          </div>

          <div class="finance-block__list">
            <div class="finance-block__item">
              <div class="finance-block__inf">
                <svg width="0.833vw" height="0.833vw" class="finance-block__icon">
                  <use href="@/assets/img/sprite.svg#block-graph-icon7"></use>
                </svg>

                <span>
                  <span class="d-lg-none blue" :style="{'color' : '#FD6A6A'}">
                   3 163 452 141
                  </span>
                  Фонд оплаты труда
                </span>
              </div>
            </div>

            <div class="finance-block__item">
              <div class="finance-block__inf">
                <svg width="0.833vw" height="0.833vw" class="finance-block__icon">
                  <use href="@/assets/img/sprite.svg#block-graph-icon2"></use>
                </svg>

                <span>
                  <span class="d-lg-none blue" :style="{'color' : '#FB9B2B'}">
                    83 112 948 
                  </span>
                  Земельный налог
                </span>
              </div>
            </div>

            <div class="finance-block__item">
              <div class="finance-block__inf">
                <svg width="0.833vw" height="0.833vw" class="finance-block__icon">
                  <use href="@/assets/img/sprite.svg#block-graph-icon8"></use>
                </svg>
                <span>
                  <span class="d-lg-none blue" :style="{'color' : '#FFC01D'}">
                    60 007 599
                  </span>
                  Имущественный налог
                </span>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="progress progress--left1">
        <p class="progress__text">01.12.2021</p>
        <svg
            width="5.208vw"
            height="0.625vw"
            viewBox="0 0 100 12"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
            class="progress__icon"
        >
          <path d="M4.5 0H0.5L11.5 12H15.5L4.5 0Z" fill="#FB9B2B" />
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

      <!-- <Progress class="progress--left1" v-bind:progress="progress.text1"/> -->

      <Progress class="progress--right1" v-bind:progress="progress.text2" />
    </div>


  </div>
</template>

<script>
import Progress from "./Progress.vue";

export default {
  name: "BlockFinance",
  data() {
    return {
      progress: {
        text1: "01.12.2021",
        text2: "92% год",
        scaleLeft: "img/scale-finance-left.svg",
      },
    };
  },
  methods: {
    fin_click: function () {
      this.connection.send("fin_click");
    },
  },
  created() {
    const ws_url = "ws://195.211.102.43:8999";
    this.connection = new WebSocket(ws_url);

    this.connection.onerror = (error) => {
      console.log(error);
    };
  },

  components: {
    Progress,
  },
};
</script>

<style lang="scss" scoped>
.finance-block {
  cursor: pointer;
}

.finance-tablet{
  @media (min-width: 768px) and (max-width: 1199.98px) {
    display: flex;
  }
}

.finance-tablet-left{
  position: relative;
  width: 8vw;

  svg{
    position: absolute;
  }

  .cirlce-block__contains {
    z-index: 1;
    position: relative;
    height: 8.5vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .cirlce-block__wrap {
      text-align: center;

      .circle-block__value{
        font-size: 1.6vw;
        position: relative;

        svg{
          right: -1.1vw;
          top: 1.4vw;
        }

      }

        
    }

    .circle-block__text{
      font-size: 0.9vw;
      color: #627DAE;
      text-align: center;
      text-transform: uppercase;
      line-height: 1.3vw;
    }

  }

  .circle-block__wrapper {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 50%;
    right: 0;
    transform: translateY(-50%);
  }

}

.finance-block__list {
  padding-top: 1vw;
  padding-left: 2vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    padding-left: 1.4vw;
  }
}

.circle-wrap__val1,
.circle-wrap__val2,
.circle-wrap__val3,
.circle-wrap__val4,
.circle-wrap__val5 {
  position: absolute;
  font-size: 0.469vw;
}

.circle-wrap__val1 {
  top: -0.2vw;
  right: -1.5vw;
}

.circle-wrap__val2 {
  bottom: -0.2vw;
  left: -1.5vw;
}

.circle-wrap__val3 {
  top: 0;
  left: -1.2vw;
}

.circle-wrap__val4 {
  top: -0.8vw;
  right: 0;
}

.circle-wrap__val5 {
  bottom: 1.2vw;
  right: -2vw;
}

.finance-block__inf {
  display: flex;
  align-items: flex-start;
  span {
    font-size: 0.677vw;
    letter-spacing: 0.03em;
    color: #fff;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      font-size: 0.8vw;
    }

    >span{
      display: block;
    }
  }
}

.finance-block__item {
  margin-bottom: 0.6vw;
}

.circle-wrap {
  position: relative;

  svg {
    transform: translateX(-0.2vw);
  }
}

.circle-finance-right{
  transform: scale(1.2) !important;
  margin-top: 0.24vw;
}

.circle-wrap__value {
  font-size: 0.469vw;
  text-transform: uppercase;
  font-weight: 700;
  text-align: center;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  color: #fff;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 0.64vw;
  }

  &:after {
    content: "";
    border-radius: 50%;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    width: 3.594vw;
    height: 3.594vw;
    border: 1px solid #217aff;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      height: 0;
      width: 0;
      position: relative;
      border: none;
    }
  }

  &.is--orange:after {
    border-color: #fd6a6a;
  }

  
}

.finance-block__icon {
  flex: 0 0 auto;
  margin-right: 0.26vw;
  margin-top: 0.2vw;
}

.finance-block__row {
  display: flex;
}

.finance-block__circle {
  width: 10.417vw;
  margin-right: 0.521vw;
  padding-left: 4vw;
  padding-top: 1vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    padding-top: 0;
    width: 11.6vw;
    margin-right: 0;

    &.sec{
      width: 12vw;
    }
  }
}

.finance-block__graph {
  width: 19.688vw;
  height: 15.365vw;
  position: absolute;
  left: 50%;
  top: 0;
  transform: translateX(-50%);
}

.finance-block__bottom {
  margin-top: -1vw;
  position: relative;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    display: flex;
    align-items: center;
    justify-content: center;
  }
}

.finance-block__top {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1.563vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    align-items: center;
    justify-content: flex-start;
  }
}

.progress--right .progress__icon {
  transform: scaleX(-1);
}

.progress--left1 {
  bottom: 0.4vw;
  left: 0.8vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    flex-direction: row-reverse;
    display: flex;
    align-items: center;
  }
}

.progress--right1 {
  bottom: 0.6vw;
  right: 0.8vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    display: flex;
    align-items: center;
  }
}

.finance-block {
  position: relative;
  width: 22.865vw;
  height: 22.135vw;
  margin-bottom: 1.5vw;
  margin-left: auto;
  margin-right: auto;
  z-index: 0;
  display: block;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    width: 51vw;
    height: 16.6vw;
    margin-left: 0.6vw;
    margin-bottom: 0;
  }
}

.finance-block__bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
}

.finance-block__title {
  font-size: 0.938vw;
  line-height: 1.042vw;
  letter-spacing: 0.05em;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1.5vw;
  }
}

.finance-block__text {
  font-size: 0.938vw;
  line-height: 1.042vw;
  letter-spacing: 0.05em;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1.5vw;
    padding-left: 2vw;
  }

  span {
    font-size: 0.469vw;
    color: #627dae;
    text-transform: uppercase;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      font-size: 0.6vw;
    }
  }
}

</style>
