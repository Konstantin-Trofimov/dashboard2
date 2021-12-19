<template>
  <main class="layout">

    <div class="top_pagination" v-if="showToHome">
      <div class="go_to_home" @click="back_click" >
        <svg width="8vw" height="2.4vw" viewBox="0 0 160 52" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M0.5 38V38.2071L0.646447 38.3536L13.6464 51.3536L13.7929 51.5H14H158.5H159V51V11V10.7929L158.854 10.6464L148.854 0.646447L148.707 0.5H148.5H1H0.5V1V38Z" stroke="#217AFF" stroke-opacity="0.4"/>
          <path d="M31.75 32.6518L21.7222 25.5L31.75 18.3482L31.75 32.6518Z" stroke="#217AFF" stroke-width="2"/>
        </svg>
        <span>
            На главную
          </span>
      </div>
    </div>

    <div v-if="showSciense == 7">
      <div class="top_pagination_list">
        <ul class="result_pagination">
          <li
              @click="handlerPaginate(1)"
              :class="{ active: isActive == 1 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>1</span>
          </li>

          <li
              @click="handlerPaginate(2)"
              :class="{ active: isActive == 2 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>2</span>
          </li>

          <li
              @click="handlerPaginate(3)"
              :class="{ active: isActive == 3 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>3</span>
          </li>

          <li
              @click="handlerPaginate(4)"
              :class="{ active: isActive == 4 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>4</span>
          </li>

          <li
              @click="handlerPaginate(5)"
              :class="{ active: isActive == 5 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>5</span>
          </li>
        </ul>
      </div>

      <img v-if="showResult == 1" src="../assets/img/result-1.svg" alt="" class="result-img"/>
      <img v-if="showResult == 2" src="../assets/img/result-2.svg" alt="" class="result-img"/>
      <img v-if="showResult == 3" src="../assets/img/result-3.svg" alt="" class="result-img"/>
      <img v-if="showResult == 4" src="../assets/img/result-4.svg" alt="" class="result-img"/>
      <img v-if="showResult == 5" src="../assets/img/result-5.svg" alt="" class="result-img"/>

    </div>

    <div v-if="showSciense == 14">
      <div class="top_pagination_list">
        <ul class="result_pagination">
          <li
              @click="handlerPaginateSite(1)"
              :class="{ active: isActiveSite == 1 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>1</span>
          </li>

          <li
              @click="handlerPaginateSite(2)"
              :class="{ active: isActiveSite == 2 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>2</span>
          </li>

          <li
              @click="handlerPaginateSite(3)"
              :class="{ active: isActiveSite == 3 }"
          >
            <svg width="2.4vw" height="2.4vw" viewBox="0 0 110 110" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M80.9858 109L109 80.9858V1H22.4142L1 22.4142V109H80.9858Z" stroke="#217AFF" stroke-width="2"/>
            </svg>
            <span>3</span>
          </li>
        </ul>
      </div>
      <img v-if="showResultSite == 1" src="../assets/img/univer-1.png" alt="" class="uni-img"/>
      <img v-if="showResultSite == 2" src="../assets/img/univer-2.png" alt="" class="uni-img"/>
      <img v-if="showResultSite == 3" src="../assets/img/univer-3.png" alt="" class="uni-img"/>
    </div>

    <div class="btn_bg" v-on:click="bg_click" v-if="showSciense == 0">
      <svg width="52" height="52" viewBox="0 0 52 52" fill="none" xmlns="http://www.w3.org/2000/svg" class="test">
        <path
            d="M51.5 38V38.2071L51.3536 38.3536L38.3536 51.3536L38.2071 51.5H38H1H0.5V51V11V10.7929L0.646446 10.6464L10.6464 0.646447L10.7929 0.5H11H51H51.5V1V38Z"
            stroke="#217AFF"
            stroke-opacity="0.4"
        />
        <path d="M32.6657 17C35.2923 18.9086 37 22.0048 37 25.5C37 31.299 32.299 36 26.5 36C20.701 36 16 31.299 16 25.5C16 22.0048 17.7077 18.9086 20.3343 17" stroke="#217AFF" stroke-width="2" />
        <path d="M26.5 13V27" stroke="#217AFF" stroke-width="2" />
      </svg>
    </div>

    <img v-if="showSciense == 0" @click="handler" src="../assets/img/ph.svg" alt="" class="ph-img" width="100%" />
<!--    <img v-if="showSciense == 1" @click="handler" src="../assets/img/science.svg" alt="" class="br-img" width="100%" />-->
    <img v-if="showSciense == 2" @click="handler" src="../assets/img/finance.svg" alt="" class="br-img" width="100%" />
    <img v-if="showSciense == 4" @click="handler" src="../assets/img/branches.svg" alt="" class="degree-img" width="100%" />
    <img v-if="showSciense == 5" @click="handler" src="../assets/img/students.svg" alt="" class="result-img" width="100%" />
    <img v-if="showSciense == 9" @click="handler" src="../assets/img/international.svg" alt="" class="result-img" width="100%" />
    <img v-if="showSciense == 10" @click="handler" src="../assets/img/all_branches.svg" alt="" class="br-img" width="100%" />
    <img v-if="showSciense == 11" @click="handler" src="../assets/img/cadres.svg" alt="" class="result-img" width="100%" />
    <img v-if="showSciense == 12" @click="handler" src="../assets/img/bachelors.svg" alt="" class="degree-img" width="100%" />
    <img v-if="showSciense == 13" @click="handler" src="../assets/img/masters.svg" alt="" class="degree-img" width="100%" />
    <!--		<img v-if="showSciense == 7" @click="handler" src="/img/group232.svg" alt="" class="test-img" width="100%" />-->
    <img v-if="showSciense == 8" @click="handler" src="../assets/img/priority.svg" alt="" class="priority-img"/>
    <img v-if="showSciense == 15" @click="handler" src="../assets/img/other.svg" alt="" class="other-img"/>

    <div v-if="showSciense == 3 || (showSciense == 0 && activeBg)" class="video">
      <video autoplay="" loop="" muted="" playsinline="">
        <source src="../assets/img/video.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"' />
        Тег video не поддерживается вашим браузером.
      </video>
    </div>

    <img v-if="showSciense == 3" @click="handler" src="../assets/img/gif2.png" alt="" class="test-img" height="95%" width="auto" />

    <div v-if="showSciense == 6">
      <div class="bg-grey"></div>

      <div class="video">
        <video autoplay="" loop="" muted="" playsinline="">
          <source src="../assets/img/video.mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"' />
          Тег video не поддерживается вашим браузером.
        </video>
      </div>

      <img @click="handler" src="../assets/img/gif2.png" alt="" class="test-img portret__foto" height="95%" width="auto" />

      <div class="portret__title" >Плеханов Георгий Валентинович<br />Философ<br />1856 - 1918 гг.</div>
    </div>


    <div v-if="showSciense == 1" @click="handler" class="scientific">
      <p class="scientific__title">Научная Деятельность</p>
      <div class="scientific-content">
        <div class="scientific__left">
          <div class="scientific__left-content">
            <div class="scientific__left-percent">
              <div class="scientific__left-percent-title">
                <p>Выполнение плана</p>
                <p>Годовой план</p>
              </div>
              <svg ref="styleObject" class="percent-bar" width="26vw" height="1.2vw" viewBox="0 0 1079 49" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M15.2074 0.126953H0.933418L40.1868 48.9997H54.4607L15.2074 0.126953Z" fill="#217AFF"/>
                <path d="M36.1527 0.126953H21.8787L61.1321 48.9997H75.406L36.1527 0.126953Z" fill="#ffffff"/>
                <path d="M57.0982 0.126953H42.8243L82.0776 48.9997H96.3516L57.0982 0.126953Z" fill="#ffffff"/>
                <path d="M78.0435 0.126953H63.7696L103.023 48.9997H117.297L78.0435 0.126953Z" fill="#ffffff"/>
                <path d="M98.9891 0.126953H84.7152L123.968 48.9997H138.242L98.9891 0.126953Z" fill="#ffffff"/>
                <path d="M119.935 0.126953H105.661L144.914 48.9997H159.188L119.935 0.126953Z" fill="#ffffff"/>
                <path d="M140.88 0.126953H126.606L165.859 48.9997H180.133L140.88 0.126953Z" fill="#ffffff"/>
                <path d="M161.825 0.126953H147.551L186.805 48.9997H201.079L161.825 0.126953Z" fill="#ffffff"/>
                <path d="M182.771 0.126953H168.497L207.75 48.9997H222.024L182.771 0.126953Z" fill="#ffffff"/>
                <path d="M203.716 0.126953H189.443L228.696 48.9997H242.97L203.716 0.126953Z" fill="#ffffff"/>
                <path d="M224.662 0.126953H210.388L249.641 48.9997H263.915L224.662 0.126953Z" fill="#ffffff"/>
                <path d="M245.607 0.126953H231.333L270.587 48.9997H284.861L245.607 0.126953Z" fill="#ffffff"/>
                <path d="M266.553 0.126953H252.279L291.532 48.9997H305.806L266.553 0.126953Z" fill="#ffffff"/>
                <path d="M287.498 0.126953H273.224L312.478 48.9997H326.752L287.498 0.126953Z" fill="#ffffff"/>
                <path d="M308.444 0.126953H294.17L333.423 48.9997H347.697L308.444 0.126953Z" fill="#ffffff"/>
                <path d="M328.807 0.126953H314.533L353.787 48.9997H368.061L328.807 0.126953Z" fill="#ffffff"/>
                <path d="M349.753 0.126953H335.479L374.732 48.9997H389.006L349.753 0.126953Z" fill="#ffffff"/>
                <path d="M370.698 0.126953H356.424L395.678 48.9997H409.952L370.698 0.126953Z" fill="#ffffff"/>
                <path d="M391.644 0.126953H377.37L416.623 48.9997H430.897L391.644 0.126953Z" fill="#ffffff"/>
                <path d="M412.589 0.126953H398.315L437.569 48.9997H451.842L412.589 0.126953Z" fill="#ffffff"/>
                <path d="M433.341 0.126953H419.067L458.32 48.9997H472.594L433.341 0.126953Z" fill="#ffffff"/>
                <path d="M454.286 0.126953H440.012L479.266 48.9997H493.54L454.286 0.126953Z" fill="#ffffff"/>
                <path d="M475.232 0.126953H460.958L500.211 48.9997H514.485L475.232 0.126953Z" fill="#ffffff"/>
                <path d="M496.177 0.126953H481.903L521.157 48.9997H535.43L496.177 0.126953Z" fill="#ffffff"/>
                <path d="M517.122 0.126953H502.849L542.102 48.9997H556.376L517.122 0.126953Z" fill="#ffffff"/>
                <path d="M537.486 0.126953H523.212L562.466 48.9997H576.74L537.486 0.126953Z" fill="#ffffff"/>
                <path d="M558.432 0.126953H544.158L583.411 48.9997H597.685L558.432 0.126953Z" fill="#ffffff"/>
                <path d="M579.377 0.126953H565.103L604.357 48.9997H618.63L579.377 0.126953Z" fill="#ffffff"/>
                <path d="M600.323 0.126953H586.049L625.302 48.9997H639.576L600.323 0.126953Z" fill="#ffffff"/>
                <path d="M621.268 0.126953H606.994L646.247 48.9997H660.521L621.268 0.126953Z" fill="#ffffff"/>
                <path d="M642.407 0.126953H628.133L667.387 48.9997H681.661L642.407 0.126953Z" fill="#ffffff"/>
                <path d="M663.353 0.126953H649.079L688.332 48.9997H702.606L663.353 0.126953Z" fill="#ffffff"/>
                <path d="M684.298 0.126953H670.024L709.278 48.9997H723.552L684.298 0.126953Z" fill="#ffffff"/>
                <path d="M705.244 0.126953H690.97L730.223 48.9997H744.497L705.244 0.126953Z" fill="#ffffff"/>
                <path d="M726.189 0.126953H711.915L751.169 48.9997H765.442L726.189 0.126953Z" fill="#ffffff"/>
                <path d="M746.553 0.126953H732.279L771.532 48.9997H785.806L746.553 0.126953Z" fill="#ffffff"/>
                <path d="M767.498 0.126953H753.225L792.478 48.9997H806.752L767.498 0.126953Z" fill="#ffffff"/>
                <path d="M788.444 0.126953H774.17L813.423 48.9997H827.697L788.444 0.126953Z" fill="#ffffff"/>
                <path d="M809.389 0.126953H795.115L834.369 48.9997H848.643L809.389 0.126953Z" fill="#ffffff"/>
                <path d="M830.335 0.126953H816.061L855.314 48.9997H869.588L830.335 0.126953Z" fill="#ffffff"/>
                <path d="M851.474 0.126953H837.2L876.453 48.9997H890.727L851.474 0.126953Z" fill="#ffffff"/>
                <path d="M872.42 0.126953H858.146L897.399 48.9997H911.673L872.42 0.126953Z" fill="#ffffff"/>
                <path d="M893.365 0.126953H879.091L918.344 48.9997H932.618L893.365 0.126953Z" fill="#ffffff"/>
                <path d="M914.311 0.126953H900.037L939.29 48.9997H953.564L914.311 0.126953Z" fill="#ffffff"/>
                <path d="M935.256 0.126953H920.982L960.235 48.9997H974.509L935.256 0.126953Z" fill="#ffffff"/>
                <path d="M955.62 0.126953H941.346L980.599 48.9997H994.873L955.62 0.126953Z" fill="#ffffff"/>
                <path d="M976.565 0.126953H962.291L1001.54 48.9997H1015.82L976.565 0.126953Z" fill="#ffffff"/>
                <path d="M997.51 0.126953H983.236L1022.49 48.9997H1036.76L997.51 0.126953Z" fill="#ffffff"/>
                <path d="M1018.46 0.126953H1004.18L1043.44 48.9997H1057.71L1018.46 0.126953Z" fill="#ffffff"/>
                <path d="M1039.4 0.126953H1025.13L1064.38 48.9997H1078.65L1039.4 0.126953Z" fill="#ffffff"/>
              </svg>

              <div class="scientific__left-percent-text">
                <p>
                  {{this.activeWidth}}%
                  <span>355 310,7 тыс. руб.</span>
                </p>
                <p>
                  100%
                  <span>503 760,6 руб.</span>
                </p>
              </div>
              <svg width="100%" height="3" viewBox="0 0 1079 3" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path opacity="0.7" d="M0.93335 1.40039H1078.27" stroke="#217AFF" stroke-width="2.13333" stroke-dasharray="2.13 6.4"/>
              </svg>
            </div>
            <div class="scientific__left-scopus">
              <div class="scientific__left-scopus-top">
                <p>
                  <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="4.52548" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.52548 15.085)" stroke="#217AFF" stroke-width="6.4"/>
                  </svg>
                  Число публикаций Scopus,
                </p>
                <p>
                  <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="4.52548" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.52548 15.085)" stroke="#44BCFF" stroke-width="6.4"/>
                  </svg>
                  в т.ч.: Q1-Q2
                </p>
              </div>
              <ul class="counts-mounts-list">
                <li>
                  <div>
                    <span style="height: 70%"><span>70</span></span>
                    <span style="height: 28%"><span>28</span></span>
                  </div>
                  <p>Июль</p>
                </li>
                <li>
                  <div>
                    <span style="height: 94%"><span>94</span></span>
                    <span style="height: 45%"><span>45</span></span>
                  </div>
                  <p>Август</p>
                </li>
                <li>
                  <div>
                    <span style="height: 59%"><span>59</span></span>
                    <span style="height: 33%"><span>33</span></span>
                  </div>
                  <p>Сентябрь</p>
                </li>
                <li>
                  <div>
                    <span style="height: 77%"><span>77</span></span>
                    <span style="height: 31%"><span>31</span></span>
                  </div>
                  <p>Октябрь</p>
                </li>
                 <li>
                  <div>
                    <span style="height: 78%"><span>78</span></span>
                    <span style="height: 43%"><span>43</span></span>
                  </div>
                  <p>Ноябрь</p>
                </li>
                <li>
                  <div>
                    <span style="height: 27%"><span>27</span></span>
                    <span style="height: 17%"><span>17</span></span>
                  </div>
                  <p>Декабрь</p>
                </li>
              </ul>
              <svg width="100%" height="2vw" viewBox="0 0 1079 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="0.933105" y="9.59961" width="1077.33" height="2.13333" fill="#B2CEF6"/>
                <rect x="75.6001" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 75.6001 10.7422)" fill="white"/>
                <rect x="259.067" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 259.067 10.7422)" fill="white"/>
                <rect x="436.133" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 436.133 10.7422)" fill="white"/>
                <rect x="619.6" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 619.6 10.7422)" fill="white"/>
                <rect x="798.8" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 798.8 10.7422)" fill="white"/>
                <rect x="982.267" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 982.267 10.7422)" fill="white"/>
              </svg>
            </div>
            <svg class="scientific__left-scopus-border" width="100%" height="3" viewBox="0 0 1079 3" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path opacity="0.7" d="M0.93335 1.40039H1078.27" stroke="#217AFF" stroke-width="2.13333" stroke-dasharray="2.13 6.4"/>
            </svg>
            <div class="scientific__left-scopus">
              <div class="scientific__left-scopus-top">
                <p>
                  <svg width="0.8vw" height="0.8vw" viewBox="0 0 32 31" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="5.45883" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 5.45883 15.085)" stroke="#FB9B2B" stroke-width="6.4"/>
                  </svg>
                  Число публикаций Scopus,
                </p>
                <p>
                  <svg width="0.8vw" height="0.8vw" viewBox="0 0 32 31" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="5.45883" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 5.45883 15.085)" stroke="#F0D182" stroke-width="6.4"/>
                  </svg>
                  в т.ч.: Q1-Q2
                </p>
              </div>
              <ul class="counts-mounts-list sec">
                
                
                <li>
                  <div>
                    <span style="height: 61%"><span>61</span></span>
                    <span style="height: 6%"><span>6</span></span>
                  </div>
                  <p>Июль</p>
                </li>
                <li>
                  <div>
                    <span style="height: 68%"><span>68</span></span>
                    <span style="height: 8%"><span>8</span></span>
                  </div>
                  <p>Август</p>
                </li>
                <li>
                  <div>
                    <span style="height: 44%"><span>44</span></span>
                    <span style="height: 6%"><span>6</span></span>
                  </div>
                  <p>Сентябрь</p>
                </li>
                <li>
                  <div>
                    <span style="height: 57%"><span>57</span></span>
                    <span style="height: 18%"><span>18</span></span>
                  </div>
                  <p>Октябрь</p>
                </li>
                <li>
                  <div>
                    <span style="height: 31%"><span>31</span></span>
                    <span style="height: 22%"><span>22</span></span>
                  </div>
                  <p>Ноябрь</p>
                </li>
                <li>
                  <div>
                    <span style="height: 21%"><span>21</span></span>
                    <span style="height: 7%"><span>7</span></span>
                  </div>
                  <p>Декабрь</p>
                </li>
              </ul>
              <svg width="100%" height="2vw" viewBox="0 0 1079 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                <rect x="0.933105" y="9.59961" width="1077.33" height="2.13333" fill="#B2CEF6"/>
                <rect x="75.6001" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 75.6001 10.7422)" fill="white"/>
                <rect x="259.067" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 259.067 10.7422)" fill="white"/>
                <rect x="436.133" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 436.133 10.7422)" fill="white"/>
                <rect x="619.6" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 619.6 10.7422)" fill="white"/>
                <rect x="798.8" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 798.8 10.7422)" fill="white"/>
                <rect x="982.267" y="10.7422" width="14.9333" height="14.9333" transform="rotate(-45 982.267 10.7422)" fill="white"/>
              </svg>
            </div>
          </div>

          <svg width="29.5vw" height="38vw" viewBox="0 0 1210 1544" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M1.93335 70.5335V1505.2V1507.33L37.1334 1542.53H233.4L251.533 1524.4H296.333L309.133 1538.27H389.133L413.667 1512.67H940.6L965.133 1538.27H1176.33L1208.33 1505.2V60.9335L1168.87 21.4669H531L510.733 1.2002H107.533L87.2667 21.4669H51L1.93335 70.5335Z" fill="#112054" fill-opacity="0.68" stroke="#217AFF" stroke-opacity="0.4" stroke-width="2.13333"/>
          </svg>

        </div>
        <div class="scientific__center">
          <p class="scientific__center-title">
            Значение показателя за 2021 год <br>
            по состоянию на 16.12.2021
          </p>
          <div class="scientific__center-item-f">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="4.99216" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.99216 15.085)" stroke="white" stroke-width="6.4"/>
            </svg>
            <p class="scientific__center-item-title">
              355 310.7
              <span>тыс <br> руб.</span>
            </p>
            <p class="scientific__center-item-text">
              Объём фактических поступлений денежных средств по НИР
            </p>
          </div>
          <div class="scientific__center-item-sec">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="4.99216" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.99216 15.085)" stroke="white" stroke-width="6.4"/>
            </svg>
            <p class="scientific__center-item-title">
              101 749.4
              <span>тыс <br> руб.</span>
            </p>
            <p class="scientific__center-item-text">
              Объём ожидаемых поступлений
              по заключённым договорам на выполнение НИР до 31.12.2021 г
            </p>
          </div>
          <div class="scientific__center-item-th">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="4.99216" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.99216 15.085)" stroke="#217AFF" stroke-width="6.4"/>
            </svg>

            <p class="scientific__center-item-title blue">
              832
            </p>
            <p class="scientific__center-item-text">
              Число публикаций Scopus
            </p>
          </div>
          <div class="scientific__center-item-fr">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 32 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="5.45883" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 5.45883 15.085)" stroke="#FB9B2B" stroke-width="6.4"/>
            </svg>
            <p class="scientific__center-item-title yellow">
              470
            </p>
            <p class="scientific__center-item-text">
              Число публикаций WoS
            </p>
          </div>
          <div class="scientific__center-item-five">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 31 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="4.99216" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 4.99216 15.085)" stroke="#44BCFF" stroke-width="6.4"/>
            </svg>
            <p class="scientific__center-item-title blue-light">
              372
            </p>
            <p class="scientific__center-item-text">
              В том числе Q1-Q2
            </p>
          </div>
          <div class="scientific__center-item-six">
            <svg width="0.8vw" height="0.8vw" viewBox="0 0 32 31" fill="none" xmlns="http://www.w3.org/2000/svg">
              <rect x="5.45883" y="15.085" width="14.9333" height="14.9333" transform="rotate(-45 5.45883 15.085)" stroke="#F0D182" stroke-width="6.4"/>
            </svg>
            <p class="scientific__center-item-title yellow-light">
              143
            </p>
            <p class="scientific__center-item-text">
              В том числе Q1-Q2
            </p>
          </div>


          <svg width="31vw" height="38vw" viewBox="0 0 1209 1544" fill="none" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
            <path d="M1.26672 70.5335V1505.2V1507.33L36.4667 1542.53H232.733L250.867 1524.4H295.667L308.467 1538.27H388.467L413 1512.67H939.933L964.467 1538.27H1175.67L1207.67 1505.2V60.9335L1168.2 21.4669H530.333L510.067 1.2002H106.867L86.6001 21.4669H50.3334L1.26672 70.5335Z" fill="#112054" fill-opacity="0.68" stroke="#217AFF" stroke-opacity="0.4" stroke-width="2.13333"/>
            <rect x="73.8" y="255.066" width="499.2" height="349.867" fill="url(#pattern0)"/>
            <rect x="73.8" y="681.733" width="499.2" height="770.133" fill="url(#pattern1)"/>
            <rect x="641" y="682" width="499.2" height="770.133" fill="url(#pattern2)"/>
            <rect x="641.267" y="255.066" width="499.2" height="349.867" fill="url(#pattern3)"/>
            <path d="M65.2667 589.999L65.2667 608.133L82.3334 608.133" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M632.733 1441.2L632.733 1459.33L649.8 1459.33" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M632.733 589.999L632.733 608.133L649.8 608.133" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M576.2 589.999L576.2 608.133L559.133 608.133" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M1143.67 1441.2L1143.67 1459.33L1126.6 1459.33" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M1143.67 589.999L1143.67 608.133L1126.6 608.133" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M83.4001 246.533L65.2667 246.533L65.2667 263.6" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M650.867 673.2L632.733 673.2L632.733 690.267" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M650.867 246.533L632.733 246.533L632.733 263.6" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M558.067 246.533L576.2 246.533L576.2 263.6" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M65.2667 1441.2L65.2667 1459.33L82.3334 1459.33" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M576.2 1441.2L576.2 1459.33L559.133 1459.33" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M83.4001 673.2L65.2667 673.2L65.2667 690.267" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M558.067 673.2L576.2 673.2L576.2 690.267" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M1125.53 673.2L1143.67 673.2L1143.67 690.267" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <path d="M1125.53 246.533L1143.67 246.533L1143.67 263.6" stroke="#217AFF" stroke-opacity="0.5" stroke-width="2.13333"/>
            <defs>
              <pattern id="pattern0" patternContentUnits="objectBoundingBox" width="0.615385" height="0.646616">
                <use xlink:href="#image0" transform="scale(0.000815079 0.00116298)"/>
              </pattern>
              <pattern id="pattern1" patternContentUnits="objectBoundingBox" width="0.615385" height="0.293754">
                <use xlink:href="#image0" transform="scale(0.000815079 0.000528334)"/>
              </pattern>
              <pattern id="pattern2" patternContentUnits="objectBoundingBox" width="0.615385" height="0.293754">
                <use xlink:href="#image0" transform="scale(0.000815079 0.000528334)"/>
              </pattern>
              <pattern id="pattern3" patternContentUnits="objectBoundingBox" width="0.615385" height="0.646616">
                <use xlink:href="#image0" transform="scale(0.000815079 0.00116298)"/>
              </pattern>
              <image id="image0" width="755" height="556" xlink:href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAvMAAAIsCAYAAAB/bSYtAAAACXBIWXMAAAsTAAALEwEAmpwYAAAF8WlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSLvu78iIGlkPSJXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQiPz4gPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iQWRvYmUgWE1QIENvcmUgNi4wLWMwMDIgNzkuMTY0MzUyLCAyMDIwLzAxLzMwLTE1OjUwOjM4ICAgICAgICAiPiA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPiA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvbW0vIiB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIiB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2RjL2VsZW1lbnRzLzEuMS8iIHhtbG5zOnBob3Rvc2hvcD0iaHR0cDovL25zLmFkb2JlLmNvbS9waG90b3Nob3AvMS4wLyIgeG1wOkNyZWF0b3JUb29sPSJBZG9iZSBQaG90b3Nob3AgMjEuMSAoV2luZG93cykiIHhtcDpDcmVhdGVEYXRlPSIyMDIxLTAyLTAzVDE3OjE2OjQ4KzAyOjAwIiB4bXA6TWV0YWRhdGFEYXRlPSIyMDIxLTAyLTAzVDE3OjE2OjQ4KzAyOjAwIiB4bXA6TW9kaWZ5RGF0ZT0iMjAyMS0wMi0wM1QxNzoxNjo0OCswMjowMCIgeG1wTU06SW5zdGFuY2VJRD0ieG1wLmlpZDpmMzdlNWQwZi0wNzY2LTkxNDUtYjQ0Yy1lYzcyN2UyNjk1ODAiIHhtcE1NOkRvY3VtZW50SUQ9ImFkb2JlOmRvY2lkOnBob3Rvc2hvcDpkMTQwMTA4NS03MGRlLTE0NGMtYWRhZC0zZjFjMGNlYTA3YjciIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDplZDQ3MjdjYy05ZTAwLTI3NGQtOGQ1Yy02Njc3ZTM3MDZlZmUiIGRjOmZvcm1hdD0iaW1hZ2UvcG5nIiBwaG90b3Nob3A6Q29sb3JNb2RlPSIzIiBwaG90b3Nob3A6SUNDUHJvZmlsZT0ic1JHQiBJRUM2MTk2Ni0yLjEiPiA8eG1wTU06SGlzdG9yeT4gPHJkZjpTZXE+IDxyZGY6bGkgc3RFdnQ6YWN0aW9uPSJjcmVhdGVkIiBzdEV2dDppbnN0YW5jZUlEPSJ4bXAuaWlkOmVkNDcyN2NjLTllMDAtMjc0ZC04ZDVjLTY2NzdlMzcwNmVmZSIgc3RFdnQ6d2hlbj0iMjAyMS0wMi0wM1QxNzoxNjo0OCswMjowMCIgc3RFdnQ6c29mdHdhcmVBZ2VudD0iQWRvYmUgUGhvdG9zaG9wIDIxLjEgKFdpbmRvd3MpIi8+IDxyZGY6bGkgc3RFdnQ6YWN0aW9uPSJzYXZlZCIgc3RFdnQ6aW5zdGFuY2VJRD0ieG1wLmlpZDpmMzdlNWQwZi0wNzY2LTkxNDUtYjQ0Yy1lYzcyN2UyNjk1ODAiIHN0RXZ0OndoZW49IjIwMjEtMDItMDNUMTc6MTY6NDgrMDI6MDAiIHN0RXZ0OnNvZnR3YXJlQWdlbnQ9IkFkb2JlIFBob3Rvc2hvcCAyMS4xIChXaW5kb3dzKSIgc3RFdnQ6Y2hhbmdlZD0iLyIvPiA8L3JkZjpTZXE+IDwveG1wTU06SGlzdG9yeT4gPC9yZGY6RGVzY3JpcHRpb24+IDwvcmRmOlJERj4gPC94OnhtcG1ldGE+IDw/eHBhY2tldCBlbmQ9InIiPz4J1NhoAAA76klEQVR4nO3ce7CddZ3n+/cmF5KQkE1CSLgkO5AY7jdBRVo0AhoVmW7FETtybEbE6+mWwSNNt810tGe6sKedDp4+HsZpjl3NEQ/dhZ4a4ZhWUZFuRAVEbiLXnQRICIQECLkn+/zx3du99mY9KzWPVfP7/qrer6pd2VL+8annWc9nfdbzrKSPVYMAS4HlwEfJ6avADcCPCufoZgnwJeD80kEarAAeIY5fNjOAHwKnlw7S4KNExi+VDtLgR8R1+0zhHN2cT/TKZwrnaGKntLcCO6Ut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"/>
            </defs>
          </svg>
        </div>
        <div class="scientific__right">
          <svg width="32vw" height="28vw" viewBox="0 0 1158 1179" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g filter="url(#filter0_d)">
              <path d="M766.054 605.042C766.054 755.513 745.621 891.717 712.599 990.287C696.087 1039.57 676.437 1079.42 654.641 1106.94C632.841 1134.47 608.952 1149.58 583.958 1149.58C558.965 1149.58 535.076 1134.47 513.276 1106.94C491.48 1079.42 471.829 1039.57 455.318 990.287C422.296 891.717 401.862 755.513 401.862 605.042C401.862 454.572 422.296 318.368 455.318 219.798C471.829 170.511 491.48 130.661 513.276 103.143C535.076 75.6192 558.965 60.5 583.958 60.5C608.952 60.5 632.841 75.6192 654.641 103.143C676.437 130.661 696.087 170.511 712.599 219.798C745.621 318.368 766.054 454.572 766.054 605.042Z" stroke="#44BCFF"/>
            </g>
            <g opacity="0.5" filter="url(#filter1_d)">
              <circle cx="840" cy="32" r="1" fill="#44BCFF"/>
            </g>
            <g filter="url(#filter2_d)">
              <path d="M583.958 787.138C433.487 787.138 297.283 766.705 198.713 733.683C149.426 717.171 109.576 697.521 82.0579 675.725C54.5344 653.925 39.4153 630.036 39.4153 605.042C39.4153 580.049 54.5344 556.16 82.0579 534.36C109.576 512.564 149.426 492.913 198.713 476.401C297.283 443.379 433.487 422.946 583.958 422.946C734.428 422.946 870.632 443.379 969.202 476.402C1018.49 492.913 1058.34 512.564 1085.86 534.36C1113.38 556.16 1128.5 580.049 1128.5 605.042C1128.5 630.036 1113.38 653.925 1085.86 675.725C1058.34 697.521 1018.49 717.171 969.202 733.683C870.632 766.705 734.428 787.138 583.958 787.138Z" stroke="#44BCFF"/>
            </g>
            <g filter="url(#filter3_d)">
              <path d="M455.196 733.803C348.798 627.405 266.935 516.645 220.586 423.596C197.41 377.069 183.127 334.995 179.081 300.125C175.034 265.248 181.235 237.665 198.908 219.992C216.581 202.319 244.164 196.118 279.041 200.165C313.911 204.211 355.984 218.494 402.511 241.67C495.561 288.019 606.32 369.882 712.719 476.28C819.117 582.679 900.98 693.439 947.329 786.488C970.505 833.015 984.788 875.088 988.834 909.958C992.881 944.835 986.68 972.418 969.007 990.091C951.334 1007.76 923.751 1013.97 888.874 1009.92C854.004 1005.87 811.931 991.589 765.404 968.413C672.354 922.064 561.595 840.202 455.196 733.803Z" stroke="#44BCFF"/>
            </g>
            <g filter="url(#filter4_d)">
              <path d="M712.719 733.804C606.321 840.202 495.561 922.065 402.512 968.414C355.985 991.59 313.912 1005.87 279.041 1009.92C244.164 1013.97 216.581 1007.77 198.908 990.092C181.235 972.419 175.034 944.836 179.081 909.959C183.127 875.089 197.41 833.016 220.586 786.489C266.935 693.439 348.798 582.68 455.197 476.281C561.595 369.883 672.355 288.02 765.404 241.671C811.931 218.495 854.004 204.212 888.874 200.166C923.751 196.119 951.334 202.32 969.007 219.993C986.68 237.666 992.882 265.249 988.835 300.126C984.789 334.996 970.505 377.069 947.33 423.596C900.98 516.646 819.118 627.405 712.719 733.804Z" stroke="#44BCFF"/>
            </g>
            <g filter="url(#filter5_d)">
              <circle cx="581.67" cy="610.993" r="27.3305" fill="url(#paint0_radial)"/>
            </g>
            <g filter="url(#filter6_d)">
              <circle cx="194.511" cy="224.748" r="13.489" fill="#44BCFF"/>
            </g>
            <g filter="url(#filter7_d)">
              <circle cx="993.54" cy="273.259" r="22.4597" fill="#44BCFF"/>
            </g>
            <g filter="url(#filter8_d)">
              <circle cx="53.5598" cy="646.688" r="5.44044" fill="#44BCFF"/>
            </g>
            <g opacity="0.5" filter="url(#filter9_d)">
              <circle cx="193" cy="1115" r="1" fill="#44BCFF"/>
            </g>
            <g filter="url(#filter10_d)">
              <circle cx="729.373" cy="947.374" r="12.6267" fill="#44BCFF"/>
            </g>
            <defs>
              <filter id="filter0_d" x="372.989" y="31.6267" width="421.939" height="1146.83" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="0.915268" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="13.729"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.4875 0 0 0 0 0.90775 0 0 0 0 1 0 0 0 1 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter1_d" x="808" y="0" width="64" height="64" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="10" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="10.5"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter2_d" x="10.542" y="394.073" width="1146.83" height="421.939" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="0.915268" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="13.729"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.4875 0 0 0 0 0.90775 0 0 0 0 1 0 0 0 1 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter3_d" x="41.0661" y="62.1501" width="1085.78" height="1085.78" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="0.915268" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="13.729"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.4875 0 0 0 0 0.90775 0 0 0 0 1 0 0 0 1 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter4_d" x="41.0665" y="62.1511" width="1085.78" height="1085.78" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="0.915268" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="13.729"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.4875 0 0 0 0 0.90775 0 0 0 0 1 0 0 0 1 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter5_d" x="459" y="488.323" width="245.339" height="245.339" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="31.7796" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="31.7796"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter6_d" x="103.201" y="133.437" width="182.621" height="182.621" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="25.9404" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="25.9404"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter7_d" x="862.405" y="142.123" width="262.271" height="262.271" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="36.2253" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="36.2253"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter8_d" x="0.115522" y="593.243" width="106.889" height="106.889" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="16.0013" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="16.0013"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter9_d" x="161" y="1083" width="64" height="64" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="10" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="10.5"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <filter id="filter10_d" x="655.649" y="873.65" width="147.448" height="147.448" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                <feFlood flood-opacity="0" result="BackgroundImageFix"/>
                <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
                <feMorphology radius="20.3657" operator="dilate" in="SourceAlpha" result="effect1_dropShadow"/>
                <feOffset/>
                <feGaussianBlur stdDeviation="20.3657"/>
                <feColorMatrix type="matrix" values="0 0 0 0 0.168627 0 0 0 0 0.83749 0 0 0 0 0.984314 0 0 0 0.84 0"/>
                <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
                <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
              </filter>
              <radialGradient id="paint0_radial" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(581.67 610.993) rotate(90) scale(27.3305)">
                <stop stop-color="#44BCFF"/>
                <stop offset="1" stop-color="#44BCFF" stop-opacity="0"/>
              </radialGradient>
            </defs>
          </svg>
        </div>
      </div>
    </div>



  </main>
</template>

<script>
export default {
  name: 'Sciense',
  data() {
    return {
      activeProgress: 0,
      activeWidth: 70.53,
      showToHome: false,
      showResult: 1,
      showResultSite: 1,
      isActive: 1,
      isActiveSite: 1,
      showSciense: 0,
      activeGif: false,
      activeBg: false,
      urlImg: '../assets/img/gif1.png',
      urlImg2: '../assets/img/gif2.png',

    }
  },
  components: {},
  methods: {
    handler() {
      this.activeGif = !this.activeGif

      if (this.activeGif) {
        this.urlImg = '../assets/img/gif1.gif'
        this.urlImg2 = '../assets/img/gif2.gif'
      } else {
        this.urlImg = '../assets/img/gif1.png'
        this.urlImg2 = '../assets/img/gif2.png'
      }
    },

    handlerPaginate(evn){
      this.showResult = false;
      this.showResult = evn;
      this.isActive = evn
    },

    handlerPaginateSite(evn){
      this.showResultSite = false;
      this.showResultSite = evn;
      this.isActiveSite = evn
    },

    bg_click() {
      this.activeBg = !this.activeBg
    },

    back_click: function() {

      this.connection.send('back_click')
    },

    svgActive: function () {
      const svg = this.$refs.styleObject;
      //console.log(svg)

      if (svg) {
        for (let i = 0; i < this.activeProgress; i++) {
          svg.childNodes[i].setAttribute("fill", "#217AFF");
        }
      }

    }

  },
  created() {
    const ws_url = 'ws://195.211.102.43:8999'
    this.connection = new WebSocket(ws_url)

    this.connection.onerror = error => {
      console.log(error)
    }

    this.connection.onmessage = e => {
      console.log(e.data)
      if (e.data == 'sc_click') {
        this.showSciense = 1
        this.showToHome = true
        //this.svgActive();
      }
      if (e.data == 'r_click' || e.data == 'back_click') {
        this.showSciense = 0
        this.showToHome = false
      }
      if (e.data == 'fin_click') {
        this.showSciense = 2
        this.showToHome = true
      }

      if (e.data == 'prt_click') {
        this.showSciense = 3
        this.showToHome = true
      }

      if (e.data == 'prt2_click') {
        this.showSciense = 6
        this.showToHome = false
      }

      if (e.data == 'memb_click') {
        this.showSciense = 4
        this.showToHome = true
      }

      if (e.data == 'stud_click') {
        this.showSciense = 5
        this.showToHome = true
      }

      if (e.data == 'cr1_click') {
        this.showSciense = 7
        this.showToHome = true
      }

      if (e.data == 'create_priority_img') {
        this.showSciense = 8
        this.showToHome = true
      }

      if (e.data == 'int_activity_click') {
        this.showSciense = 9
        this.showToHome = true
      }

      if (e.data == 'all_branches') {
        this.showSciense = 10
        this.showToHome = true
      }

      if (e.data == 'staff_branches') {
        this.showSciense = 11
        this.showToHome = true
      }

      if (e.data == 'bachelors_click') {
        this.showSciense = 12
        this.showToHome = true
      }

      if (e.data == 'masters_click') {
        this.showSciense = 13
        this.showToHome = true
      }

      if (e.data == 'site_click') {
        this.showSciense = 14
        this.showToHome = true
      }

      if (e.data == 'digitalization_click') {
        this.showSciense = 15
        this.showToHome = true
      }

    }

    const a = Math.floor(this.activeWidth.toFixed()/2 )
    this.activeProgress = a;
    console.log(a)
  },
  mounted() {
    //console.log('mounted')
    //this.svgActive();
  },
  watch: {
    showSciense: function (newVal, oldVal) {
      if (newVal === 1) {
        //console.log('ch')
        setTimeout(() => {
          this.svgActive();
        }, 200);
      }
    }
  }
}
</script>

<style lang="scss">
.btn_bg {
  z-index: 999;
  cursor: pointer;
}

.priority-img {
  width: 100vw;
  height: 50vw;
}

.test {
  position: absolute;
  left: 45px;
  top: 45px;
  cursor: pointer;
  z-index: 999;
}

.test-img {
  z-index: 998;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.video {
  position: absolute;
  overflow: hidden;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 9;

  video {
    width: 100%;
    display: block;
    height: 100%;
    object-fit: cover;
  }
}

.top_pagination{
  position: absolute;
  top: 2vw;
  left: 4vw;
  display: flex;
  z-index: 999;
}

.top_pagination_list{
  position: absolute;
  top: 2vw;
  left: 12.7vw;
  display: flex;
  z-index: 99;
}

.go_to_home{
  position: relative;
  margin-right: 1vw;
  cursor: pointer;
}

.go_to_home span{
  font-family: Rubik;
  font-weight: 700;
  font-size: 0.625vw;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: #217aff;
  position: absolute;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 1.2vw;
  right: 0;
  bottom: 0;
}

.result_pagination{
  display: flex;
  list-style-type: none;
}

.result_pagination li{
  position: relative;
  cursor: pointer;
  opacity: .55;
}

.result_pagination li.active{
  opacity: 1;
}

.result_pagination li+li{
  margin-left: .7vw;
}

.result_pagination li span{
  font-family: Rubik;
  font-weight: 700;
  font-size: 0.75vw;
  letter-spacing: 0.1em;
  color: #217aff;
  position: absolute;
  margin: auto;
  display: flex;
  align-items: center;
  justify-content: center;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}

.result-img {
  width: 91vw;
  margin: 3.4vw auto 0 auto;
  height: 50vw;
}

.other-img {
  width: 140%;
  height: 54vw;
}

.uni-img {
  width: 91vw;
  margin: 6.4vw auto 9vw auto;
}

.degree-img {
  width: 92vw;
  margin: 0 auto 0 auto;
  height: 52vw;
}

.br-img {
  width: 92vw;
  margin: 1vw auto auto auto;
  height: 50vw;
}

.ph-img{
  margin: auto;
  height: 100vh;
  width: 60%;
}

.scientific{
  width: 91vw;
  margin: 6vw auto auto auto;
  height: 50vw;

  .scientific__title{
    font-size: 1.8vw;
    letter-spacing: 0.04vw;
    margin-bottom: 1.3vw;
  }

  .scientific-content{
    display: flex;
    align-items: center;

    .scientific__center{
      margin-left: 1vw;
      position: relative;

      .scientific__center-title{
        position: absolute;
        font-size: 1vw;
        letter-spacing: 0.04vw;
        top: 1.4vw;
        left: 2.2vw;
      }

      &-item-title{
        font-size: 1.9vw;
        letter-spacing: 0.04vw;
        font-weight: 500;
        position: relative;
        display: flex;

        >span{
          font-size: 0.75vw;
          font-weight: normal;
          position: relative;
          right: -0.4vw;
          top: 0.34vw;
        }

        &.blue{
          color: #217AFF;
          font-size: 2.5vw;
          margin-bottom: 0.2vw;
        }

        &.yellow{
          color: #FB9B2B;
          font-size: 2.5vw;
          margin-bottom: 0.2vw;
        }

        &.blue-light{
          color: #44BCFF;
          font-size: 2.5vw;
          margin-bottom: 0.2vw;
        }

        &.yellow-light{
          color: #FFDD85;
          font-size: 2.5vw;
          margin-bottom: 0.2vw;
        }

      }


      &-item-text{
        font-size: 0.7vw;
        font-weight: normal;
        line-height: 1vw;
        padding: 0 1vw;
      }

      &-item-f{
        position: absolute;
        top: 7.3vw;
        width: 12.4vw;
        left: 2.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

      &-item-sec{
        position: absolute;
        top: 7.3vw;
        width: 12.4vw;
        left: 16.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

      &-item-th{
        position: absolute;
        top: 18.5vw;
        width: 12.4vw;
        left: 2.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

      &-item-fr{
        position: absolute;
        top: 18.5vw;
        width: 12.4vw;
        left: 16.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

      &-item-five{
        position: absolute;
        top: 27.3vw;
        width: 12.4vw;
        left: 2.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

      &-item-six{
        position: absolute;
        top: 27.3vw;
        width: 12.4vw;
        left: 16.4vw;
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: center;
        align-items: center;
      }

    }

    .scientific__left{
      position: relative;

      &-content{
        position: absolute;
        top: 2.5vw;
        display: flex;
        flex-direction: column;
        width: 26vw;
        left: 1.8vw;

        .percent-blue{
          width: 100%;
          overflow: hidden;
          position: relative;
          top: -1.2vw;
        }

        .scientific__left-percent{

          .percent-bar{
            display: flex;
            justify-content: space-between;

            span{
              background-color: #ffffff;
              height: 30px;
              width: 2px;
              transform: rotate(-40deg);
              display: block;
            }
          }

          &-title{
            display: flex;
            justify-content: space-between;
            font-size: 0.7vw;
            letter-spacing: 0.04vw;
            margin-bottom: 0.6vw;
          }

          &-text{
            display: flex;
            justify-content: space-between;
            margin-top: 0.4vw;
            padding-bottom: 1vw;

            p{
              font-size: 0.9vw;
              font-weight: 600;

              span{
                display: block;
                font-size: 0.8vw;
                font-weight: 100;
                opacity: .8;
              }

              &:last-child{
                text-align: right;
              }

            }
          }
        }

        .scientific__left-scopus{
          padding-top: 1vw;

          &-border{
            margin-top: 1.7vw;
          }

          &-top{
            left: -1.1vw;
            position: relative;

            p{
              margin: 0;
              font-size: 0.9vw;
              font-weight: 500;
              display: flex;
              align-items: center;
              svg{
                margin-right: 0.3vw;
              }
            }
          }

          .counts-mounts-list{
            list-style-type: none;
            margin-top: 2.5vw;
            display: flex;
            justify-content: space-between;
            padding: 0 0.4vw;
            margin-bottom: -1vw;

            &.sec{
              li{
                >div{
                  >span{
                    &:first-child{
                      background-color: #FB9B2B;
                    }
                    &:last-child{
                      background-color: #FFDD85;
                    }
                  }
                }
              }
            }

            li{
              height: 4.5vw;

              >p{
                text-align: center;
                padding-top: 0.6vw;
                font-size: 0.65vw;
              }

              >div{
                display: flex;
                height: 100%;
                align-items: flex-end;

                >span{
                  width: 1.7vw;

                  >span{
                    margin-top: -0.95vw;
                    width: 1.7vw;
                    text-align: center;
                    display: block;
                    font-size: 0.6vw;
                  }

                  &:first-child{
                    background-color: #217AFF;
                  }
                  &:last-child{
                    background-color: #44BCFF;
                  }
                }
              }


            }
          }

        }


      }
    }

  }
}

</style>

