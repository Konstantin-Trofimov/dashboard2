

<template>
  <div>
    <a class="site__btn" v-on:click="site_click">
      <svg class="d-md-none" width="91" height="52" viewBox="0 0 91 52" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g filter="url(#filter0_i)">
          <path d="M90.5 38V38.2926L90.2449 38.4359L67.1049 51.4359L66.9908 51.5H66.86H1H0.5V51V11V10.7074L0.755104 10.5641L18.5551 0.564082L18.6692 0.5H18.8H90H90.5V1V38Z" fill="black" fill-opacity="0.1" stroke="#FB9B2B"/>
        </g>
        <defs>
          <filter id="filter0_i" x="0" y="0" width="91" height="56" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
            <feFlood flood-opacity="0" result="BackgroundImageFix"/>
            <feBlend mode="normal" in="SourceGraphic" in2="BackgroundImageFix" result="shape"/>
            <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
            <feOffset dy="4"/>
            <feGaussianBlur stdDeviation="2"/>
            <feComposite in2="hardAlpha" operator="arithmetic" k2="-1" k3="1"/>
            <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0"/>
            <feBlend mode="normal" in2="shape" result="effect1_innerShadow"/>
          </filter>
        </defs>
      </svg>

      <p class="site__btn-text">сайт РЭУ</p>
    </a>


    <div class="circle-block">

      <div class="circle-block__first" v-on:click="all_branches">
        <svg class="circle-first__icon" width="12.82vw" height="7.813vw">
          <use href="@/assets/img/sprite.svg#first-icon"></use>

        </svg>

          <span class="circle-block__link">Все филиалы</span>
      </div>

      <div class="circle-block__second">
        <svg class="circle-second__icon" width="15.625vw" height="7.813vw">
          <use href="@/assets/img/sprite.svg#second-icon"></use>
        </svg>

        <div class="cirlce-block__contains">
          <div class="cirlce-block__wrap">
            <svg class="circle-block__icon" width="1.042vw" height="1.042vw">
              <use href="../assets/img/sprite.svg#star-icon"></use>
            </svg>
            <span class="circle-block__value">5</span>
          </div>
          <p class="circle-block__text">
            Рейтинг Вуза по <br />
            QS WUR
          </p>
        </div>
      </div>

      <div class="circle-block__third">
        <svg class="circle-third__icon">
          <use href="@/assets/img/sprite.svg#third-icon"></use>
        </svg>

        <div class="circle-block__wrapper" v-on:click="staff_branches">
          <div class="cirlce-block__contains ">
            <div class="cirlce-block__wrap">
              <span class="circle-block__value">1 299</span>
              <!-- <svg class="circle-block__icon" width="0.781vw" height="0.781vw">
                <use href="../assets/img/sprite.svg#icon1"></use>
              </svg> -->
              <svg style="right: -0.1vw;top: 1.2vw;position: absolute;" class="circle-block__icon" width="0.781vw" height="0.781vw">
                <use href="../assets/img/sprite.svg#icon2"></use>
              </svg>
            </div>
            <p class="circle-block__text">Преподавателей</p>
          </div>

          <div class="cirlce-block__contains">
            <p class="circle-block__text">Кадры в <br>г. Москве</p>
          </div>

          <div class="cirlce-block__contains">
            <div class="cirlce-block__wrap">
              <span class="circle-block__value">482</span>
              <!-- <svg class="circle-block__icon down" width="0.781vw" height="0.781vw">
                            <use href="../assets/img/sprite.svg#icon1"></use>
                          </svg> -->
             <svg class="circle-block__icon" width="0.781vw" height="0.781vw">
               <use href="../assets/img/sprite.svg#icon2"></use>
             </svg>
            </div>
            <p class="circle-block__text">
              научных <br />
              работников
            </p>
          </div>
        </div>
      </div>

      <div class="circle-block__fourth">
        <svg class="circle-fourth__icon">
          <use href="@/assets/img/sprite.svg#fourth-icon"></use>
        </svg>

        <div class="cirlce-block__contains">
          <span class="circle-block__value">4.2</span>
          <p class="circle-block__text">средний балл</p>
        </div>
      </div>

      <div class="circle-block__fifth" v-on:click="cr_click" >
        <svg class="circle-fifth__icon">
          <use href="@/assets/img/sprite.svg#fifth-icon"></use>
        </svg>

        <div class="cirlce-block__wrapper">
          <div class="cirlce-block__contains ">
            <span class="circle-block__value">1302</span>
            <p class="circle-block__text">
              кол-во <br />
              публикаций
            </p>
          </div>

          <div class="cirlce-block__contains">
            <span class="circle-block__value">70,5</span>
            <p class="circle-block__text">
              Выполнение <br />
              плана, %
            </p>
          </div>

          <div class="cirlce-block__contains">
            <span class="circle-block__value small">133</span>
            <p class="circle-block__text">
              заключенные <br />
              договоры
            </p>
          </div>
        </div>
      </div>

      <div class="circle-block__sixth">
        <svg class="circle-sixth__icon">
          <use href="@/assets/img/sprite.svg#sixth-icon"></use>
        </svg>

        <div class="cirlce-block__wrapper">
          <div class="cirlce-block__contains">
            <div class="cirlce-block__wrap">
              <span class="circle-block__value">3,77<span></span></span>
              <!-- <svg class="circle-block__icon circle-block__icon__top" width="0.781vw" height="0.781vw">
                <use href="../assets/img/sprite.svg#icon1"></use>
              </svg> -->
              <svg class="circle-block__icon circle-block__icon__down" width="0.781vw" height="0.781vw">
               <use href="../assets/img/sprite.svg#icon2"></use>
             </svg>
            </div>
            <p class="circle-block__text">Денежные <br />Средства, млрд.</p>
          </div>

          <div class="cirlce-block__contains">
            <div class="cirlce-block__wrap">
              <span class="circle-block__value">5,75<span></span></span>
              <svg style="top: 0.5vw" class="circle-block__icon arrow-cash circle-block__icon__top" width="0.781vw" height="0.781vw">
                <use href="../assets/img/sprite.svg#icon1"></use>
              </svg>
              <!-- <svg class="circle-block__icon circle-block__icon__down" width="0.781vw" height="0.781vw">
               <use href="../assets/img/sprite.svg#icon2"></use>
             </svg> -->
            </div>
            <p class="circle-block__text">Касса, млн.</p>
          </div>
        </div>
      </div>

      <div class="circle-block__middle">
        <span>43 511</span>
        <p>ОБучающихся</p>
      </div>

      <div class="circle__parts">
        <div class="circle__part-top">
          <div class="circle__part-text">
            <span class='span_84'>80%</span>
            <span class='span_text'
            >Абсолютная <br />
						успеваемость</span
            >
          </div>

          <svg width="17.6vw" height="9.467vw" viewBox="0 0 355 193" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M161.461 48.3743C164.192 47.9193 166.946 47.5471 169.722 47.2602L165.094 2.49881C161.389 2.88185 157.711 3.37872 154.065 3.98631L161.461 48.3743Z" fill="#FB9B2B"/>
            <path d="M103.906 72.4005C106.152 70.7817 108.456 69.2266 110.816 67.7388L86.8184 29.6714C83.6677 31.6576 80.5917 33.7338 77.5929 35.8953L103.906 72.4005Z" fill="#FB9B2B"/>
            <path d="M173.873 46.8958C176.634 46.6966 179.414 46.5817 182.21 46.5533L181.754 1.55565C178.027 1.59342 174.319 1.74667 170.634 2.01252L173.873 46.8958Z" fill="#FB9B2B"/>
            <path d="M114.375 65.5713C116.761 64.1684 119.202 62.8325 121.696 61.567L101.333 21.4377C98.009 23.1245 94.7533 24.9063 91.5688 26.7784L114.375 65.5713Z" fill="#FB9B2B"/>
            <path d="M186.377 46.5753C189.144 46.6324 191.926 46.7746 194.722 47.0041L198.405 2.15513C194.692 1.85018 190.99 1.66098 187.305 1.58492L186.377 46.5753Z" fill="#FB9B2B"/>
            <path d="M125.44 59.7393C127.946 58.5635 130.503 57.457 133.11 56.4233L116.523 14.5917C113.059 15.965 109.658 17.4367 106.322 19.0026L125.44 59.7393Z" fill="#FB9B2B"/>
            <path d="M211.243 49.3684C213.99 49.9348 216.7 50.5815 219.371 51.3055L231.142 7.87239C227.585 6.90823 223.98 6.04811 220.331 5.29568L211.243 49.3684Z" fill="#FB9B2B"/>
            <path d="M148.966 51.2157C151.679 50.5054 154.395 49.8833 157.111 49.3476L148.401 5.19852C144.785 5.91191 141.172 6.7395 137.568 7.68319L148.966 51.2157Z" fill="#FB9B2B"/>
            <path d="M198.894 47.4212C201.682 47.7282 204.44 48.1187 207.168 48.5897L214.826 4.24614C211.194 3.61888 207.524 3.09963 203.821 2.69171L198.894 47.4212Z" fill="#FB9B2B"/>
            <path d="M137.035 54.9466C139.669 53.9856 142.315 53.1123 144.968 52.3251L132.168 9.18391C128.635 10.2323 125.116 11.3941 121.616 12.6707L137.035 54.9466Z" fill="#FB9B2B"/>
            <path d="M63.3283 119.353C64.6088 116.899 65.9698 114.475 67.4113 112.086L28.8827 88.8366C26.9584 92.0255 25.1413 95.2613 23.4315 98.5387L63.3283 119.353Z" fill="#FB9B2B"/>
            <path d="M47.8668 179.775C47.9261 177.007 48.0712 174.231 48.3039 171.451L3.4607 167.698C3.15005 171.409 2.95626 175.115 2.87708 178.811L47.8668 179.775Z" fill="#FB9B2B"/>
            <path d="M69.6193 108.552C71.1222 106.228 72.704 103.939 74.3648 101.688L38.1591 74.9649C35.9453 77.9642 33.8354 81.0175 31.8298 84.1197L69.6193 108.552Z" fill="#FB9B2B"/>
            <path d="M48.7156 167.304C49.0319 164.554 49.4345 161.801 49.9253 159.048L5.62365 151.151C4.96946 154.821 4.43237 158.493 4.01031 162.163L48.7156 167.304Z" fill="#FB9B2B"/>
            <path d="M76.8906 98.3745C78.6019 96.1993 80.3904 94.063 82.2563 91.9693L48.6609 62.0301C46.1822 64.8116 43.8031 67.6531 41.5241 70.5499L76.8906 98.3745Z" fill="#FB9B2B"/>
            <path d="M50.7198 154.958C51.2891 152.249 51.9448 149.541 52.6887 146.837L9.30075 134.9C8.31247 138.493 7.44017 142.094 6.68203 145.701L50.7198 154.958Z" fill="#FB9B2B"/>
            <path d="M94.0897 80.1997C96.1955 78.3474 98.3433 76.5727 100.529 74.8755L72.9335 39.3302C70.0221 41.5906 67.1653 43.9512 64.3679 46.412L94.0897 80.1997Z" fill="#FB9B2B"/>
            <path d="M58.0757 131.041C59.1416 128.447 60.2797 125.904 61.4866 123.413L20.9899 103.791C19.3827 107.108 17.869 110.491 16.4529 113.937L58.0757 131.041Z" fill="#FB9B2B"/>
            <path d="M85.1011 88.8883C87.0244 86.8471 88.9968 84.8794 91.0147 82.9852L60.2157 50.1763C57.5284 52.699 54.9049 55.3165 52.3499 58.028L85.1011 88.8883Z" fill="#FB9B2B"/>
            <path d="M53.8723 142.814C54.691 140.132 55.5863 137.494 56.5549 134.901L14.4008 119.152C13.1108 122.605 11.9201 126.114 10.8324 129.678L53.8723 142.814Z" fill="#FB9B2B"/>
            <path d="M308.343 137.63C309.209 140.26 309.997 142.925 310.704 145.624L354.236 134.224C353.293 130.621 352.241 127.062 351.084 123.551L308.343 137.63Z" fill="#0C1C52"/>
            <path d="M275.814 84.7822C277.768 86.7434 279.668 88.7719 281.511 90.8666L315.297 61.1433C312.837 58.3469 310.3 55.6385 307.691 53.0199L275.814 84.7822Z" fill="#0C1C52"/>
            <path d="M222.867 51.819C225.488 52.7102 228.091 53.6857 230.672 54.746L247.774 13.1225C244.329 11.707 240.854 10.4046 237.354 9.21455L222.867 51.819Z" fill="#FB9B2B"/>
            <path d="M284.214 94.0377C285.977 96.1716 287.683 98.3701 289.328 100.632L325.725 74.1712C323.533 71.1559 321.259 68.2235 318.906 65.3757L284.214 94.0377Z" fill="#0C1C52"/>
            <path d="M234.501 56.3893C237.028 57.5202 239.532 58.7343 242.009 60.0326L262.898 20.175C259.596 18.4445 256.257 16.8249 252.885 15.3158L234.501 56.3893Z" fill="#FB9B2B"/>
            <path d="M291.726 104.039C293.283 106.327 294.781 108.677 296.214 111.087L334.891 88.0845C332.987 84.8823 330.995 81.7571 328.92 78.7106L291.726 104.039Z" fill="#0C1C52"/>
            <path d="M245.669 62.0229C248.08 63.3825 250.464 64.8243 252.817 66.349L277.283 28.5809C274.156 26.5553 270.985 24.6374 267.774 22.8268L245.669 62.0229Z" fill="#FB9B2B"/>
            <path d="M303.867 125.919C304.998 128.486 306.043 131.069 307.002 133.665L349.214 118.073C347.937 114.616 346.548 111.18 345.045 107.771L303.867 125.919Z" fill="#0C1C52"/>
            <path d="M266.254 76.2497C268.406 78.0483 270.487 79.9003 272.498 81.8021L303.419 49.1082C300.741 46.5755 297.972 44.1121 295.114 41.7228L266.254 76.2497Z" fill="#FB9B2B"/>
            <path d="M298.294 114.729C299.66 117.178 300.942 119.652 302.139 122.147L342.709 102.676C341.114 99.3534 339.409 96.0627 337.595 92.8089L298.294 114.729Z" fill="#0C1C52"/>
            <path d="M256.296 68.6914C258.607 70.2809 260.852 71.9302 263.032 73.6356L290.76 38.1934C287.857 35.9223 284.87 33.7286 281.801 31.617L256.296 68.6914Z" fill="#FB9B2B"/>
          </svg>

        </div>

        <div class="circle__part-bottom">
          <div class="circle__part-text">
            <span>37%</span>
            <span>Качественная <br> успеваемость</span>
          </div>

          <svg data-v-e096734a="" width="18.229vw" height="9.167vw" viewBox="0 0 350 176" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path data-v-e096734a="" d="M0.799844 17.79C0.449844 14.13 0.209844 10.4 0.0898438 6.72L40.1798 5.42999C40.2698 8.26999 40.4598 11.15 40.7198 13.98L0.799844 17.79Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M3.16016 34.27C2.46016 30.65 1.87016 26.96 1.41016 23.27L41.2002 18.2C41.5602 21.02 42.0102 23.86 42.5502 26.64L3.16016 34.27Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M7.0898 50.46C6.0898 46.93 5.0898 43.31 4.2998 39.71L43.4298 30.86C44.0598 33.63 44.7798 36.42 45.5798 39.14L7.0898 50.46Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M12.56 66.21C11.18 62.78 9.9 59.27 8.75 55.77L46.85 43.23C47.73 45.92 48.72 48.62 49.78 51.23L12.56 66.21Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M19.4802 81.32C17.7802 78.04 16.1802 74.68 14.7002 71.32L51.4302 55.19C52.5702 57.78 53.8102 60.37 55.1102 62.9L19.4802 81.32Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M27.8194 95.71C25.8194 92.61 23.8994 89.41 22.1094 86.2L57.1094 66.65C58.4894 69.12 59.9694 71.59 61.5094 73.98L27.8194 95.71Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M37.4904 109.25C35.2104 106.36 33.0004 103.36 30.9004 100.33L63.9004 77.53C65.5204 79.87 67.2304 82.19 68.9804 84.42L37.4904 109.25Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M48.3902 121.81C45.8502 119.15 43.3902 116.36 40.9902 113.55L71.6902 87.74C73.5202 89.91 75.4402 92.06 77.4002 94.12L48.3902 121.81Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M60.44 133.29C57.66 130.88 54.91 128.35 52.29 125.76L80.42 97.16C82.42 99.16 84.57 101.11 86.71 102.97L60.44 133.29Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M73.5194 143.59C70.5194 141.45 67.5195 139.19 64.6895 136.86L89.9995 105.73C92.2094 107.52 94.4995 109.27 96.8195 110.92L73.5194 143.59Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M87.5396 152.61C84.3496 150.77 81.1696 148.79 78.0996 146.74L100.34 113.36C102.71 114.94 105.15 116.46 107.61 117.88L87.5396 152.61Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M102.35 160.25C98.9896 158.72 95.6396 157.05 92.3496 155.31L111.35 119.96C113.85 121.3 116.43 122.58 119.02 123.76L102.35 160.25Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M117.86 166.45C114.37 165.25 110.86 163.91 107.46 162.45L122.95 125.45C125.57 126.55 128.26 127.58 130.95 128.5L117.86 166.45Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M133.86 171.13C130.28 170.27 126.68 169.28 123.15 168.18L135 129.87C137.72 130.71 140.49 131.47 143.24 132.14L133.86 171.13Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M150.229 174.26C146.569 173.74 142.889 173.1 139.279 172.35L147.439 133.07C150.209 133.65 153.049 134.14 155.859 134.54L150.229 174.26Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M166.79 175.81C163.11 175.64 159.39 175.35 155.74 174.95L160.11 135.07C162.94 135.38 165.81 135.6 168.65 135.73L166.79 175.81Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M175.06 176C174.15 176 173.24 176 172.33 176L172.93 135.89H175.05C177.19 135.89 179.36 135.84 181.51 135.74L183.41 175.81C180.64 175.93 177.83 176 175.06 176Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M188.95 175.45L185.79 135.45C188.62 135.23 191.49 134.91 194.3 134.51L200 174.23C196.33 174.75 192.62 175.16 188.95 175.45Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M205.46 173.36L198.52 133.85C201.32 133.36 204.13 132.77 206.89 132.1L216.33 171.1C212.75 172 209.09 172.72 205.46 173.36Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M221.71 169.69L211 131C213.73 130.24 216.48 129.39 219.16 128.46L232.3 166.36C228.84 167.6 225.27 168.71 221.71 169.69Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M237.54 164.49L223.21 127C225.85 126 228.5 124.88 231.08 123.7L247.78 160.18C244.42 161.73 241 163.17 237.54 164.49Z" fill="#0b1b51"></path>
            <path data-v-e096734a="" d="M252.77 157.81L234.92 121.89C237.46 120.63 239.99 119.27 242.45 117.89L262.54 152.61C259.35 154.41 256.07 156.17 252.77 157.81Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M267.3 149.71L246.12 115.64C248.53 114.14 250.92 112.55 253.23 110.9L276.53 143.55C273.53 145.69 270.42 147.76 267.3 149.71Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M281 140.26L256.68 108.36C258.94 106.64 261.17 104.82 263.32 102.96L289.6 133.27C286.81 135.68 283.92 138 281 140.26Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M293.73 129.56L266.51 100.1C268.6 98.17 270.65 96.1 272.62 94.1L301.62 121.79C299.09 124.45 296.43 127.07 293.73 129.56Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M305.4 117.71L275.52 90.95C277.41 88.83 279.27 86.63 281.03 84.39L312.55 109.21C310.26 112.1 307.86 115 305.4 117.71Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M315.91 104.79L283.63 81C285.32 78.71 286.95 76.34 288.49 73.95L322.22 95.67C320.22 98.75 318.1 101.83 315.91 104.79Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M325.15 90.93L290.75 70.29C292.21 67.85 293.62 65.29 294.92 62.81L330.56 81.22C328.87 84.5 327.05 87.76 325.15 90.93Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M333 76.24L296.83 59C298.05 56.43 299.21 53.79 300.26 51.16L337.51 66C336.14 69.47 334.63 72.9 333 76.24Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M339.5 60.84L301.8 47.12C302.8 44.45 303.67 41.72 304.46 39L343 50.28C341.92 53.82 340.76 57.37 339.5 60.84Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M344.43 44.93L305.6 34.88C306.31 32.14 306.94 29.33 307.47 26.54L346.87 34.08C346.18 37.71 345.36 41.36 344.43 44.93Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M347.83 28.61L308.21 22.33C308.65 19.53 309.02 16.67 309.28 13.84L349.22 17.61C348.87 21.28 348.41 25 347.83 28.61Z" fill="#217AFF"></path>
            <path data-v-e096734a="" d="M349.65 12.08L309.65 9.56999C309.83 6.73999 309.92 3.85998 309.92 0.999985V0.669983H350V0.999985C350 4.68998 349.88 8.41999 349.65 12.08Z" fill="#217AFF"></path>
          </svg>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BlockCircle',
  methods: {
    cr_click: function() {
      this.connection.send('cr1_click')
    },

    site_click: function() {
      this.connection.send('site_click')
    },

    all_branches: function() {
      this.connection.send('all_branches')
    },

    staff_branches: function() {
      this.connection.send('staff_branches')
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

.site__btn {
  position: relative;
  width: 5.3vw;
  height: 2.8vw;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: -1vw auto 0.8vw auto;
}

.site__btn svg {
  position: absolute;
  width: 5.3vw;
  height: 2.8vw;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
}

.site__btn-text {
  font-size: 0.9vw;
  color: #fb9b2b;
  font-weight: 500;
  text-transform: uppercase;
}

.circle-block__sixth {
  width: 15.365vw;
  height: 18.229vw;
  transform: translate(-1.5vw, -7.2vw);

  .circle-sixth__icon {
    width: 15.365vw;
    height: 18.229vw;
  }

  .cirlce-block__wrapper {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 0;
    left: 0;
  }

  .cirlce-block__contains {
    position: static;

    &:first-of-type {
      transform: translate(5vw, 5vw);
    }

    &:last-of-type {
      transform: translate(1vw, 6vw);
    }

    .circle-block__text {
      text-align: center;
    }

    .circle-block__icon {
      position: absolute;
      top: 1.5vw;
      right: 0.5vw;
      margin-right: 0;
    }

    .circle-block__icon__top {
      right: 0.3vw;
      bottom: 1.9vw;
    }

    
  }

  .cirlce-block__wrap {
    position: relative;
  }

}
.circle-block__fifth {
  width: 14.167vw;
  height: 16.667vw;
  position: absolute;
  bottom: 0.5vw;
  left: -0.3vw;
  cursor: pointer;

  .circle-fifth__icon {
    width: 14.167vw;
    height: 16.667vw;
  }

  .cirlce-block__wrapper {
    display: flex;
    flex-direction: column;
    position: absolute;
    top: 0;
    left: 0;
  }

  .circle-block__value {
    font-size: 1.563vw;
  }

  .circle-block__text {
    font-size: 0.521vw;
    line-height: 0.833vw;
  }

  .span_text{
    position: absolute;
    width: 76px;
    height: 34px;
    left: 768px;
    top: 546px;

    font-family: Oswald;
    font-style: normal;
    font-weight: normal;
    font-size: 10px;
    line-height: 15px;
    /* or 155% */

    text-align: center;
    letter-spacing: 0.1em;
    text-transform: uppercase;

    color: #FB9B2B;
  }
  .cirlce-block__contains {
    position: static;

    &:first-of-type {
      transform: translate(1.8vw, 1vw);
    }

    &:nth-of-type(2) {
      transform: translate(3.8vw, 2vw);
    }

    &:last-of-type {
      transform: translate(8vw, 2vw);
    }
  }
}

.circle-block__fourth {
  width: 12.604vw;
  height: 8.177vw;
  position: absolute;
  bottom: -1.4vw;
  left: 50%;
  transform: translateX(-50%);

  .circle-fourth__icon {
    width: 12.604vw;
    height: 8.177vw;
  }
}

svg {
  overflow: visible;
}

.circle-block__third {
  position: absolute;
  bottom: 0;
  right: 0;
  width: 15.417vw;
  height: 17.656vw;
  z-index: 1;
  transform: translate(1.6vw, 0.6vw);
  cursor: pointer;

  .cirlce-block__contains {
    position: static;
    transform: none;
    transform: translate(-1.875vw, -2.083vw);

    .cirlce-block__wrap {
      align-items: flex-start;
      position: relative;
      left: 0.5vw;

      .circle-block__icon {
        margin-left: 0.4vw;
        margin-right: 0;
        //margin-top: 1.4vw;
      }

      .down{
        position: relative;
        top: -1.4vw;
      }

    }

    &:nth-of-type(2) {
      transform: translate(-2.8vw, -1vw);
      .circle-block__text{
        color: #217AFF;
      }
    }

    &:last-of-type {
      transform: translate(-7vw, -.1vw);
      .cirlce-block__wrap {
        align-items: baseline;
      }
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

.circle-third__icon {
  width: 15.417vw;
  height: 17.656vw;
}

.circle__parts {
  position: absolute;
  left: 50%;
  transform: translate(-50%, 0);
  top: 0;
  z-index: 2;
  width: 18.594vw;
  height: 18.594vw;
}

.cirlce-block__wrap {
  display: flex;
  align-items: center;
  justify-content: center;

  .circle-block__icon {
    margin-right: 0.4vw;
  }
}

.circle-block__middle {
  position: absolute;
  width: 12.5vw;
  height: 12.5vw;
  border-radius: 50%;
  border: 1px solid rgba(33, 122, 255, 0.48);
  top: 52%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  z-index: 1;

  span {
    font-weight: 500;
    font-size: 3.646vw;
  }

  p {
    font-size: 0.938vw;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    margin-top: 0px;
  }
}

.circle-block {
  position: relative;
  width: 36.25vw;
  height: 36.25vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    width: auto;
    height: auto;
  }

  &:after {
    content: '';
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 33.542vw;
    height: 33.542vw;
    border-radius: 50%;
    border: 1px solid rgba(33, 122, 255, 0.48);
    z-index: -1;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      display: none;
      position: relative;
      width: 0;
      height: 0;
    }
  }

  &:before {
    content: '';
    position: absolute;
    top: 52%;
    left: 50%;
    transform: translate(-50%, -50%);
    width: 19.833vw;
    height: 19.833vw;
    border-radius: 50%;
    border: 1px solid rgba(33, 122, 255, 0.48);
    z-index: 1;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      display: none;
      position: relative;
      width: 0;
      height: 0;
    }
  }
}

.cirlce-block__contains {
  position: absolute;
  z-index: 1;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

.circle-block__first {
  position: relative;
  display: flex;
  justify-content: center;
  z-index: 3;
  >svg{
    cursor: pointer;
    //height: 7.8vw;
    //width: 15vw;
    //transform: scale(0.8);
    //position: relative;
    //bottom: 0.55vw;
    path{
      width: 12.82vw;
      height: 7.813vw;
    }
  }
}

.circle-block__link {
  display: block;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: #217aff;
  font-size: 0.833vw;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  cursor: pointer;

  &::before {
    content: '';
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    top: -0.781vw;
    width: 0;
    height: 0;
    border-style: solid;
    border-width: 0 0.286vw 0.495vw 0.286vw;
    border-color: transparent transparent #217aff transparent;
  }
}

.circle-block__value {
  color: #fff;
  font-weight: 500;
  font-size: 1.8vw;
}

.circle-block__text {
  text-align: center;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: #627dae;
  font-size: 0.729vw;
  line-height: 1.042vw;
}

.circle-block__second {
  position: absolute;
  right: 0;
  width: 14.323vw;
  height: 17.604vw;
  z-index: 2;
  transform: translate(0.6vw, -6.2vw);

  .circle-block__text {
    position: relative;
    left: 2vw;
  }
}

.circle-second__icon {
  position: absolute;
  top: 0;
  left: 0;
  width: 14.323vw;
  height: 17.604vw;
}

.circle__part-top {
  color: #fb9b2b;
  position: absolute;
  top: 9.8vw;
  left: 0.2vw;

  .circle__part-text {
    position: absolute;
    bottom: -4vw;
    left: 0;
    z-index: 1;
  }
}




.circle__part-text {
  text-align: center;

  span {
    display: block;
  }

  span:first-of-type {
    font-size: 1.146vw;
    line-height: 1.042vw;
    font-weight: 700;
    margin-bottom: 0.156vw;
  }

  span:last-of-type {
    letter-spacing: 0.1em;
    text-transform: uppercase;
    font-size: 0.521vw;
    line-height: 0.781vw;
  }
}

.circle__part-bottom {
  color: #217AFF;
  position: absolute;
  bottom: -9.5vw;
  right: 0.2vw;

  .circle__part-text {
    position: absolute;
    top: -4vw;
    right: -1vw;
    z-index: 1;
  }
}

// .arrow-cash {
//   top: 5vw;
// }

</style>
