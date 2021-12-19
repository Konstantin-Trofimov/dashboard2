<template>
  <div>
    <div class="science-top d-lg-none" v-on:click="cr_click">
      <svg width="29.5vw" height="8.3vw" viewBox="0 0 290 78" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M16.5 0H273.5L290 17.0959V74.6877V78H15.5H0V17.0959L16.5 0Z" fill="#112054" fill-opacity="0.7"/>
        <path d="M1 17.4998L16.9246 1H273.075L289 17.4998V74.6877V77H15.5H1V17.4998Z" stroke="#217AFF" stroke-opacity="0.9" stroke-width="2"/>
      </svg>
      <div class="science-top__result">
        <div>
          <p>1302</p>
          <span>кол-во публикаций</span>
        </div>
        <div>
          <p>
            70,5
            <!-- <svg class="circle-block__icon circle-block__icon__top" width="0.781vw" height="0.781vw">
              <use href="../assets/img/sprite.svg#icon1"></use>
            </svg> -->
          </p>
          <span>Выполнение плана, %</span>
        </div>
        <div>
          <p>133</p>
          <span>заключенные договоры</span>
        </div>
      </div>
    </div>

    <div class="science-block" id="science_click" v-on:click="sc_click">

      <svg class="science-block__bg d-md-none" width="21.510vw" height="19.375vw">
        <use href="@/assets/img/sprite.svg#science-container"></use>
      </svg>

      <svg class="science-block__bg d-lg-none" width="29.5vw" height="29.3vw" viewBox="0 0 290 283" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 0H290V12.7932V270.982L274.5 283H15.5L0 270.982V12.7932V0Z" fill="#112054" fill-opacity="0.7"/>
        <path d="M1 1H289V12.7932V270.492L274.158 282H15.8423L1 270.492V12.7932V1Z" stroke="#217AFF" stroke-opacity="0.9" stroke-width="2"/>
      </svg>



      <div class="science-block__top">
        <div class="science-block__cols">
          <div class="science-block__col">
            <p class="science-block__title">Научная деятельность</p>
            <p class="science-block__subtitle">Выполнение плана</p>
            <p class="science-block__percent">70,5%</p>

            <svg class="d-lg-none" width="14.5vw" height="4vw"  viewBox="0 0 122 20" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M122 10L0 10" stroke="#627DAE" stroke-opacity="0.2" stroke-width="20" stroke-dasharray="3 2"/>
              <path d="M0 10L65 10" stroke="#A7EB17" stroke-width="20" stroke-dasharray="3 2"/>
            </svg>

            <svg
                class="science-block__bar d-md-none"
                width="11.32vw"
                height="1.6vw"
                viewBox="0 0 163 23" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M6.69088 0.0908813H-2.86102e-05L18.4 23H25.0909L6.69088 0.0908813Z" fill="#A7EB17"/>
              <path d="M65.6 0.0908813H58.9091L77.3091 23H84L65.6 0.0908813Z" fill="#A7EB17"/>
              <path d="M36.1455 0.0908813H29.4546L47.8546 23H54.5455L36.1455 0.0908813Z" fill="#A7EB17"/>
              <path d="M95.0545 0.0908813H88.3636L106.764 23H113.455L95.0545 0.0908813Z" fill="#A7EB17" />
              <path d="M144.145 0.0908813H137.455L155.855 23H162.545L144.145 0.0908813Z" fill="#A7EB17" fill-opacity="0.2"/>
              <path d="M16.5091 0.0908813H9.81821L28.2182 23H34.9091L16.5091 0.0908813Z" fill="#A7EB17"/>
              <path d="M75.4182 0.0908813H68.7273L87.1273 23H93.8182L75.4182 0.0908813Z" fill="#A7EB17" />
              <path d="M124.509 0.0908813H117.818L136.218 23H142.909L124.509 0.0908813Z" fill="#A7EB17" fill-opacity="0.2"/>
              <path d="M45.9636 0.0908813H39.2727L57.6727 23H64.3636L45.9636 0.0908813Z" fill="#A7EB17"/>
              <path d="M104.873 0.0908813H98.1818L116.582 23H123.273L104.873 0.0908813Z" fill="#A7EB17" fill-opacity="0.2"/>
              <path d="M26.3273 0.0908813H19.6364L38.0364 23H44.7273L26.3273 0.0908813Z" fill="#A7EB17"/>
              <path d="M85.2364 0.0908813H78.5454L96.9454 23H103.636L85.2364 0.0908813Z" fill="#A7EB17"/>
              <path d="M134.327 0.0908813H127.636L146.036 23H152.727L134.327 0.0908813Z" fill="#A7EB17" fill-opacity="0.2"/>
              <path d="M55.7818 0.0908813H49.0909L67.4909 23H74.1818L55.7818 0.0908813Z" fill="#A7EB17" />
              <path d="M114.691 0.0908813H108L126.4 23H133.091L114.691 0.0908813Z" fill="#A7EB17" fill-opacity="0.2"/>
            </svg>

            <p class="science-block__text text-right">
              <span>503 760,6 тыс.</span>
            </p>
          </div>

          <div class="science-block__col">
            <div class="science-block__list">
              <div class="science-block__item">
                <div class="science-block__inf">
                  <svg
                      width="0.833vw"
                      height="0.833vw"
                      class="science-block__icon d-md-none"
                  >
                    <use href="@/assets//img/sprite.svg#block-graph-icon4"></use>
                  </svg>

                  <p class="science-block__text">
                    Поступления от НИР <br />
                    за текущий год <br />
                    <span>355 310,7 тыс.</span>
                  </p>
                </div>
              </div>

              <div class="science-block__item">
                <div class="science-block__inf">
                  <svg
                      width="0.833vw"
                      height="0.833vw"
                      class="science-block__icon d-md-none"
                  >
                    <use href="@/assets//img/sprite.svg#block-graph-icon5"></use>
                  </svg>

                  <p class="science-block__text">
                    Ожидаемые поступления <br />
                    от НИР в текущем году <br />
                    <span>101 749,4 тыс.</span>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="science-block__bottom">
        <div class="science-block__rows">
          <div class="science-block__btns">
            <button class="science-btn is--active">
              <svg class="science-btn__active d-md-none">
                <use href="@/assets/img/sprite.svg#science-btn-icon"></use>
              </svg>

              <svg class="science-btn__icon" width="0.521vw" height="0.521vw">
                <use href="@/assets/img/sprite.svg#triangle-icon"></use>
              </svg>
              <span class="science-btn__text">Публикации WoS</span>
            </button>

            <button class="science-btn">
              <svg class="science-btn__icon" width="0.521vw" height="0.521vw">
                <use href="@/assets/img/sprite.svg#triangle-icon"></use>
              </svg>
              <span class="science-btn__text">Публикации Scopus</span>
            </button>

            <button class="science-btn">
              <svg class="science-btn__icon" width="0.521vw" height="0.521vw">
                <use href="@/assets/img/sprite.svg#triangle-icon"></use>
              </svg>
              <span class="science-btn__text">Публикации Q1</span>
            </button>

            <button class="science-btn">
              <svg class="science-btn__icon" width="0.521vw" height="0.521vw">
                <use href="@/assets/img/sprite.svg#triangle-icon"></use>
              </svg>
              <span class="science-btn__text">Публикации Q2</span>
            </button>
          </div>

          <div class="science-block__graph">  


        

        


          <svg width="11.5vw"
              height="7.3vw" viewBox="0 0 242 122" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M5.31626 46.099C4.58292 46.099 4.03292 45.8313 3.66626 45.296C3.30692 44.7533 3.12726 44.0457 3.12726 43.173V40.17C3.12726 39.2093 3.29592 38.443 3.63326 37.871C3.97059 37.299 4.53159 37.013 5.31626 37.013C6.00559 37.013 6.53726 37.2 6.91126 37.574C7.28526 37.948 7.47959 38.4833 7.49426 39.18L7.50526 39.312H6.31726C6.31726 38.8573 6.24392 38.5237 6.09726 38.311C5.95059 38.091 5.69026 37.981 5.31626 37.981C4.64159 37.981 4.30426 38.6153 4.30426 39.884V41.237C4.42159 41.0463 4.59026 40.896 4.81026 40.786C5.03759 40.676 5.30159 40.621 5.60226 40.621C6.29892 40.621 6.79392 40.8447 7.08726 41.292C7.38059 41.732 7.52726 42.3663 7.52726 43.195C7.52726 44.0677 7.34759 44.7717 6.98826 45.307C6.62892 45.835 6.07159 46.099 5.31626 46.099ZM5.31626 45.12C5.68292 45.12 5.94326 44.9697 6.09726 44.669C6.25859 44.3683 6.33926 43.9723 6.33926 43.481C6.33926 43.0337 6.32092 42.678 6.28426 42.414C6.24759 42.15 6.15592 41.9337 6.00926 41.765C5.86259 41.5963 5.63159 41.512 5.31626 41.512C5.08892 41.512 4.88726 41.5707 4.71126 41.688C4.54259 41.8053 4.40692 41.9483 4.30426 42.117V43.448C4.30426 43.954 4.38126 44.361 4.53526 44.669C4.69659 44.9697 4.95692 45.12 5.31626 45.12ZM10.7715 46.099C9.99415 46.099 9.43315 45.8753 9.08848 45.428C8.74382 44.9807 8.57148 44.3353 8.57148 43.492C8.57148 42.9273 8.66315 42.4763 8.84648 42.139C9.03715 41.8017 9.31215 41.523 9.67148 41.303C9.01148 40.863 8.68148 40.1993 8.68148 39.312C8.68148 38.586 8.85382 38.0213 9.19848 37.618C9.54315 37.2147 10.0675 37.013 10.7715 37.013C11.4682 37.013 11.9852 37.2147 12.3225 37.618C12.6672 38.0213 12.8395 38.586 12.8395 39.312C12.8395 39.7887 12.7552 40.1883 12.5865 40.511C12.4178 40.8263 12.1722 41.0903 11.8495 41.303C12.2088 41.5303 12.4838 41.8127 12.6745 42.15C12.8652 42.4873 12.9605 42.9347 12.9605 43.492C12.9605 44.328 12.7882 44.9733 12.4435 45.428C12.0988 45.8753 11.5415 46.099 10.7715 46.099ZM10.7715 40.764C11.3802 40.7567 11.6845 40.2507 11.6845 39.246C11.6845 38.85 11.6112 38.531 11.4645 38.289C11.3252 38.047 11.0942 37.926 10.7715 37.926C10.4488 37.926 10.2105 38.047 10.0565 38.289C9.90982 38.531 9.83648 38.85 9.83648 39.246C9.83648 39.686 9.90615 40.049 10.0455 40.335C10.1848 40.6137 10.4268 40.7567 10.7715 40.764ZM10.7715 45.164C11.1675 45.164 11.4425 45.021 11.5965 44.735C11.7505 44.4417 11.8275 44.0347 11.8275 43.514C11.8275 43.0373 11.7432 42.6487 11.5745 42.348C11.4132 42.0473 11.1455 41.8933 10.7715 41.886C10.3902 41.8933 10.1152 42.0473 9.94648 42.348C9.77782 42.6487 9.69348 43.0373 9.69348 43.514C9.69348 44.0347 9.77048 44.4417 9.92448 44.735C10.0858 45.021 10.3682 45.164 10.7715 45.164Z" fill="white"/>
<rect x="8" y="117" width="204" height="1" fill="#B2CEF6"/>
<rect x="7.56946" y="118.002" width="67.4164" height="1" transform="rotate(-90.1599 7.56946 118.002)" fill="#B2CEF6"/>
<rect x="54" y="53" width="22" height="64" fill="#217AFF"/>
<rect x="22" y="58" width="22" height="59" fill="#217AFF"/>
<rect x="84" y="74" width="22" height="43" fill="#217AFF"/>
<rect x="117" y="61" width="22" height="56" fill="#217AFF"/>
<rect x="149" y="88" width="22" height="29" fill="#217AFF"/>
<rect x="181" y="101" width="22" height="16" fill="#217AFF"/>
<rect x="29.7071" y="117.536" width="4" height="4" transform="rotate(-45 29.7071 117.536)" fill="white" stroke="#B2CEF6"/>
<rect x="4.70711" y="52.5355" width="4" height="4" transform="rotate(-45 4.70711 52.5355)" fill="white" stroke="#B2CEF6"/>
<rect x="61.7071" y="117.536" width="4" height="4" transform="rotate(-45 61.7071 117.536)" fill="white" stroke="#B2CEF6"/>
<rect x="91.7071" y="117.536" width="4" height="4" transform="rotate(-45 91.7071 117.536)" fill="white" stroke="#B2CEF6"/>
<rect x="124.707" y="117.536" width="4" height="4" transform="rotate(-45 124.707 117.536)" fill="white" stroke="#B2CEF6"/>
<rect x="156.707" y="117.536" width="4" height="4" transform="rotate(-45 156.707 117.536)" fill="white" stroke="#B2CEF6"/>
<rect x="188.707" y="117.536" width="4" height="4" transform="rotate(-45 188.707 117.536)" fill="white" stroke="#B2CEF6"/>
<g filter="url(#filter0_d_2008_6106)">
<path d="M216.5 68.4999L218 69.9999H229L230 68.9999L232 66.9999V5.99988L230.5 4.49988L229 2.99988H218L216.5 4.49988L215 5.99988V66.9999L216.5 68.4999Z" fill="#112054"/>
<path d="M218 70.4999H217.793L217.646 70.3534L216.146 68.8534L214.646 67.3534L214.5 67.207V66.9999V5.99988V5.79277L214.646 5.64632L216.146 4.14632L217.646 2.64632L217.793 2.49988H218H229H229.207L229.354 2.64632L230.854 4.14632L232.354 5.64632L232.5 5.79277V5.99988V66.9999V67.207L232.354 67.3534L230.354 69.3534L229.354 70.3534L229.207 70.4999H229H218Z" stroke="#217AFF"/>
</g>
<path d="M225.38 48.86H227.27V49.53H226V54.24H227.27V54.91H225.38V54.61C225.36 54.2567 225.1 54.0167 224.6 53.89C224.1 53.7633 223.4 53.6767 222.5 53.63L220.74 53.56V49.68H225.38V48.86ZM222.54 52.98C223.287 53.0133 223.903 53.0767 224.39 53.17C224.87 53.2633 225.2 53.43 225.38 53.67V50.39H221.37V52.92L222.54 52.98ZM223.59 42.8763V47.2763C224.137 47.2363 224.58 47.0263 224.92 46.6463C225.253 46.2663 225.42 45.7863 225.42 45.2063C225.42 44.8797 225.363 44.5797 225.25 44.3063C225.13 44.033 224.957 43.7963 224.73 43.5963L225.19 43.1963C225.47 43.4297 225.683 43.723 225.83 44.0763C225.977 44.423 226.05 44.8063 226.05 45.2263C226.05 45.7663 225.937 46.2463 225.71 46.6663C225.477 47.0797 225.157 47.403 224.75 47.6363C224.343 47.8697 223.883 47.9863 223.37 47.9863C222.857 47.9863 222.397 47.8763 221.99 47.6563C221.583 47.4297 221.267 47.123 221.04 46.7363C220.813 46.343 220.7 45.903 220.7 45.4163C220.7 44.9297 220.813 44.493 221.04 44.1063C221.267 43.7197 221.583 43.4163 221.99 43.1963C222.39 42.9763 222.85 42.8663 223.37 42.8663L223.59 42.8763ZM221.31 45.4163C221.31 45.923 221.473 46.3497 221.8 46.6963C222.12 47.0363 222.54 47.2297 223.06 47.2763V43.5463C222.54 43.593 222.12 43.7897 221.8 44.1363C221.473 44.4763 221.31 44.903 221.31 45.4163ZM223.66 39.3847V40.5847H226V41.2947H220.74V40.5847H223.05V39.3747L220.74 37.5247V36.7547L223.29 38.8247L226 36.6047V37.4447L223.66 39.3847ZM220.7 33.7718C220.7 33.0851 220.873 32.5585 221.22 32.1918C221.56 31.8251 222.067 31.6418 222.74 31.6418H226V32.3218H225.18C225.453 32.4818 225.667 32.7185 225.82 33.0318C225.973 33.3385 226.05 33.7051 226.05 34.1318C226.05 34.7185 225.91 35.1851 225.63 35.5318C225.35 35.8785 224.98 36.0518 224.52 36.0518C224.073 36.0518 223.713 35.8918 223.44 35.5718C223.167 35.2451 223.03 34.7285 223.03 34.0218V32.3518H222.71C222.257 32.3518 221.913 32.4785 221.68 32.7318C221.44 32.9851 221.32 33.3551 221.32 33.8418C221.32 34.1751 221.377 34.4951 221.49 34.8018C221.597 35.1085 221.747 35.3718 221.94 35.5918L221.41 35.9118C221.183 35.6451 221.01 35.3251 220.89 34.9518C220.763 34.5785 220.7 34.1851 220.7 33.7718ZM225.49 34.0218C225.49 33.6218 225.4 33.2785 225.22 32.9918C225.033 32.7051 224.767 32.4918 224.42 32.3518H223.56V34.0018C223.56 34.9018 223.873 35.3518 224.5 35.3518C224.807 35.3518 225.05 35.2351 225.23 35.0018C225.403 34.7685 225.49 34.4418 225.49 34.0218ZM220.87 27.2017C220.87 26.7151 220.98 26.2817 221.2 25.9017C221.413 25.5151 221.717 25.2151 222.11 25.0017C222.497 24.7884 222.94 24.6817 223.44 24.6817C223.953 24.6817 224.41 24.7951 224.81 25.0217C225.203 25.2417 225.51 25.5517 225.73 25.9517C225.95 26.3517 226.06 26.8117 226.06 27.3317C226.06 28.2051 225.753 28.8817 225.14 29.3617C224.527 29.8417 223.68 30.0817 222.6 30.0817C221.473 30.0817 220.61 29.8684 220.01 29.4417C219.41 29.0084 219.003 28.3351 218.79 27.4217L218.25 25.0617L218.9 24.9417L219.41 27.1617C219.577 27.9151 219.873 28.4684 220.3 28.8217C220.72 29.1751 221.343 29.3684 222.17 29.4017C221.763 29.1884 221.447 28.8917 221.22 28.5117C220.987 28.1317 220.87 27.6951 220.87 27.2017ZM225.47 27.3117C225.47 26.9451 225.387 26.6184 225.22 26.3317C225.047 26.0384 224.807 25.8117 224.5 25.6517C224.193 25.4851 223.847 25.4017 223.46 25.4017C223.073 25.4017 222.733 25.4817 222.44 25.6417C222.147 25.8017 221.92 26.0284 221.76 26.3217C221.593 26.6084 221.51 26.9384 221.51 27.3117C221.51 27.6851 221.593 28.0184 221.76 28.3117C221.92 28.5984 222.147 28.8251 222.44 28.9917C222.733 29.1517 223.073 29.2317 223.46 29.2317C223.847 29.2317 224.193 29.1517 224.5 28.9917C224.807 28.8251 225.047 28.5951 225.22 28.3017C225.387 28.0084 225.47 27.6784 225.47 27.3117ZM220.7 20.4499C220.7 19.9566 220.813 19.5099 221.04 19.1099C221.26 18.7099 221.573 18.3966 221.98 18.1699C222.387 17.9433 222.85 17.8299 223.37 17.8299C223.897 17.8299 224.363 17.9433 224.77 18.1699C225.177 18.3966 225.493 18.7099 225.72 19.1099C225.94 19.5033 226.05 19.9499 226.05 20.4499C226.05 20.8766 225.963 21.2633 225.79 21.6099C225.61 21.9499 225.35 22.2299 225.01 22.4499H227.94V23.1599H220.74V22.4799H221.78C221.433 22.2666 221.167 21.9866 220.98 21.6399C220.793 21.2866 220.7 20.8899 220.7 20.4499ZM225.42 20.4999C225.42 20.1333 225.337 19.7999 225.17 19.4999C224.997 19.1999 224.753 18.9666 224.44 18.7999C224.127 18.6266 223.77 18.5399 223.37 18.5399C222.97 18.5399 222.617 18.6266 222.31 18.7999C221.997 18.9666 221.753 19.1999 221.58 19.4999C221.407 19.7999 221.32 20.1333 221.32 20.4999C221.32 20.8733 221.407 21.2099 221.58 21.5099C221.753 21.8033 221.997 22.0366 222.31 22.2099C222.617 22.3766 222.97 22.4599 223.37 22.4599C223.77 22.4599 224.127 22.3766 224.44 22.2099C224.753 22.0366 224.997 21.8033 225.17 21.5099C225.337 21.2099 225.42 20.8733 225.42 20.4999ZM222.6 14.0445C222.607 13.3845 222.753 12.8845 223.04 12.5445C223.327 12.1978 223.74 12.0245 224.28 12.0245C224.84 12.0245 225.27 12.2111 225.57 12.5845C225.87 12.9511 226.017 13.4845 226.01 14.1845L226 16.3045H220.74V15.5945H222.58L222.6 14.0445ZM225.47 14.2245C225.477 13.7378 225.38 13.3711 225.18 13.1245C224.973 12.8711 224.673 12.7445 224.28 12.7445C223.893 12.7445 223.607 12.8678 223.42 13.1145C223.233 13.3611 223.137 13.7311 223.13 14.2245L223.11 15.5945H225.45L225.47 14.2245Z" fill="white"/>
<defs>
<filter id="filter0_d_2008_6106" x="214" y="1.99988" width="28" height="79" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
<feFlood flood-opacity="0" result="BackgroundImageFix"/>
<feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0" result="hardAlpha"/>
<feOffset dx="5" dy="6"/>
<feGaussianBlur stdDeviation="2"/>
<feColorMatrix type="matrix" values="0 0 0 0 0.0897222 0 0 0 0 0.241933 0 0 0 0 0.633333 0 0 0 0.12 0"/>
<feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_2008_6106"/>
<feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_2008_6106" result="shape"/>
</filter>
</defs>
</svg>


          </div>
        </div>
      </div>

      <div class="progress progress--left1">
        <p class="progress__text">16.12.2021</p>
        <svg
            width="5.208vw"
            height="0.625vw"
            viewBox="0 0 100 12" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M4.5 0H0.5L11.5 12H15.5L4.5 0Z" fill="#F79A2D" />
          <path d="M40.5 0H36.5L47.5 12H51.5L40.5 0Z" fill="#F79A2D"  />
          <path d="M22.5 0H18.5L29.5 12H33.5L22.5 0Z" fill="#F79A2D" />
          <path d="M58.5 0H54.5L65.5 12H69.5L58.5 0Z" fill="#F79A2D"  fill-opacity="0.2"/>
          <path d="M88.5 0H84.5L95.5 12H99.5L88.5 0Z" fill="#F79A2D"  fill-opacity="0.2"/>
          <path d="M10.5 0H6.5L17.5 12H21.5L10.5 0Z" fill="#F79A2D" />
          <path d="M46.5 0H42.5L53.5 12H57.5L46.5 0Z" fill="#F79A2D" />
          <path d="M76.5 0H72.5L83.5 12H87.5L76.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
          <path d="M28.5 0H24.5L35.5 12H39.5L28.5 0Z" fill="#F79A2D" />
          <path d="M64.5 0H60.5L71.5 12H75.5L64.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
          <path d="M16.5 0H12.5L23.5 12H27.5L16.5 0Z" fill="#F79A2D" />
          <path d="M52.5 0H48.5L59.5 12H63.5L52.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
          <path d="M82.5 0H78.5L89.5 12H93.5L82.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
          <path d="M34.5 0H30.5L41.5 12H45.5L34.5 0Z" fill="#F79A2D" />
          <path d="M70.5 0H66.5L77.5 12H81.5L70.5 0Z" fill="#F79A2D" fill-opacity="0.2"/>
        </svg>

      </div>

      <!-- <Progress class="progress--left1" v-bind:progress="progress.text1" /> -->

      <!-- <Progress class="progress--right1" v-bind:progress="progress.text2" /> -->
      <div class="progress progress--right1">
        <p class="progress__text">96% год</p>
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
          <path d="M23.5 0H27.5L16.5 12H12.5L23.5 0Z" fill="#F79A2D" />
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
  </div>

</template>

<script>
import Progress from "./Progress.vue";
export default {
  data() {
    return {
      progress: {
        text1: "05.07.2021",
        text2: "55% год",
      },
    };
  },

  methods: {
    sc_click: function () {
      this.connection.send("sc_click");
    },
    cr_click: function() {
      this.connection.send('cr1_click')
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
.science-block {
  position: relative;
  width: 21.51vw;
  height: 19.375vw;
  z-index: 0;
  margin-left: auto;
  margin-right: auto;
  cursor: pointer;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    height: 29.3vw;
    width: 29.5vw;
    margin-left: 0;
  }
}

.science-top{
  height: 8.3vw;
  width: 29.5vw;

  >svg{
    position: absolute;
  }

  .science-top__result{
    display: flex;
    align-items: center;
    justify-content: space-between;
    z-index: 9;
    position: relative;
    height: 100%;

    div{
      text-align: center;
      padding: 0 2vw;
      line-height: 1vw;

      p{
        font-size: 1.6vw;
        line-height: 2.2vw;
        position: relative;
        display: table;
        margin: 0 auto;

        svg{
          position: absolute;
          right: -1vw;
          top: -0.3vw;
        }
      }
      span{
        font-size: 0.8vw;
        color: #627DAE;
        text-align: center;
        text-transform: uppercase;
      }
    }

  }
}

.progress--right .progress__icon {
  transform: scaleX(-1);
}

.science-btn__active {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  left: 0;
  width: 8.292vw;
  height: 2.615vw;
}

.science-btn__icon {
  stroke: #d2daef;
  margin-right: 0.313vw;
  flex: 0 0 auto;
}

.science-btn__text {
  font-size: 0.66vw;
  letter-spacing: 0.03em;
  color: #fff;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 0.9vw;
  }
}

.science-block__graph{
  position: relative;
  top: -1vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    >svg{
      width: 14.5vw;
    }
  }
}

.science-btn {
  display: flex;
  align-items: center;
  width: 7.8vw;
  height: 1.615vw;
  position: relative;
  padding-left: 0.5vw;

  @media (min-width: 768px) and (max-width: 1199.98px) {
    width: 13.8vw;
    height: 1.9vw;
  }

  &.is--active {
    .science-btn__icon {
      stroke: #217aff;
    }
  }
}

.science-block__percent {
  font-weight: 700;
  font-size: 0.781vw;
  line-height: 1.042vw;
  color: #f79a2d;
  margin-bottom: 0.208vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 2vw;
    color: #A7EB17;
    line-height: 2.5vw;
    font-weight: normal;
  }
}

.science-block__rows {
  display: flex;
}

.science-block__btns {
  width: 9.292vw;
  margin-right: 0.521vw;
  flex: 0 0 auto;
  padding-left: 1.563vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    width: 14.3vw;
  }
}

.science-block__title {
  font-size: 0.938vw;
  line-height: 1.042vw;
  letter-spacing: 0.05em;
  margin-bottom: 1.1vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1.5vw;
    line-height: 2vw;
  }
}

.science-block__cols {
  display: flex;
}

.science-block__col {
  padding-top: 1.354vw;
  padding-left: 1.302vw;
  padding-right: 1.302vw;

  &:first-of-type {
    width: 11.771vw;

    @media (min-width: 768px) and (max-width: 1199.98px) {
      width: 17.5vw;
    }
  }

  &:last-of-type {
    padding-left: 0;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      padding-left: 1.302vw;
      width: 12.5vw;
    }
  }
}

.science-block__inf {
  display: flex;
  align-items: flex-start;
}

.science-block__icon {
  position: relative;
  top: 0.2vw;
  margin-right: 0.104vw;
}

.science-block__text {
  font-size: 0.677vw;
  letter-spacing: 0.03em;
  color: #cdd6ee;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1vw;
  }


  span {
    display: block;
    margin-top: 0.313vw;
    color: #ffffff;
    @media (min-width: 768px) and (max-width: 1199.98px) {
      margin-top: 0;
      font-size: 1vw;
    }
  }
}

.science-block__text.text-right {
  text-align: right;
}

.science-block__bg {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: -1;
}

.science-block__list {
  padding-top: 0.5vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    padding-top: 3.1vw;
    padding-bottom: 1vw;
  }
}

.science-block__item {
  margin-bottom: 0.625vw;
}

.science-block__bar {
  width: 9vw;
}

.science-block__top {
  position: relative;
  &:after {
    content: "";
    position: absolute;
    left: 1.563vw;
    right: 1.563vw;
    bottom: 0;
    border: 1px dashed rgba(33, 122, 255, 0.2);
  }
}

.science-block__bottom {
  padding-top: 0.625vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    position: absolute;
    bottom: 3vw;
  }
}

.science-block__subtitle{
  font-size: 0.74vw;
  @media (min-width: 768px) and (max-width: 1199.98px) {
    font-size: 1vw;
  }
}

</style>

