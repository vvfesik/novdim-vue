<template>
  <div class="component-navigator properties navigator-state">
    <div class="line line--1 line--vert line--dark"></div>
    <div class="line line--2 line--vert line--dark hidden-xs"></div>
    <div class="line line--3 line--vert line--dark hidden-sm"></div>
    <div class="properties-wrapper container-fluid">
      <div class="row height-100">
        <div class="col-xs-offset row absolute height-100" style="z-index:20">
          <app-shared-button-back></app-shared-button-back>
        </div>
        <div class="col-xs relative row height-100 column-direction">
          <div id="navigator-wrapper" style="z-index: 2; visibility: visible; opacity: 1;">
            <div class="navigator">
              <div class="inner-wrapper" :style="'height:' + svgWrapperHeight + 'px; left:' + svgWrapperLeft + 'px;'">
                <div :style="'position: absolute; width: inherit; height: inherit; top:' + topOffset + 'px;'">
                  <svg id="navigatorSVG" viewBox="0 0 1920 1080">
                    <image id="navigatorBG" width="1920" height="1080" xlink:href="static/img/krushynka_map_top_f_1920.jpg" overflow="hidden"/>
                    <g id="sold">
                      <path data-property-id="2" d="M385 506.5L323 619l59.3 31.8 62-112.3z"/>
                      <path data-property-id="4" d="M444.3 538.5l-62 112.5 43.2 23.3 62-112.3z"/>
                      <path data-property-id="6" d="M487.5 562l-62 112.5 43.3 23.3 62-112.3z"/>
                      <path data-property-id="8" d="M530.8 585.5l-62 112.5 42.2 22.8 62-112.3z"/>
                      <path data-property-id="10" d="M573 608.5L511 721l43 23.8 62-112.3z"/>
                      <path data-property-id="12" d="M616 632.3l-62 112.5 43.3 23.2 62-112.2z"/>
                      <path data-property-id="14" d="M659.3 655.8l-62 112.5 42.7 24.2L702 680z"/>
                      <path data-property-id="20" d="M788.3 726.8l-62 112.5 42.7 23 62-112.5z"/>
                      <path data-property-id="22" d="M831 749.8l-62 112.5 42.8 23 62-112.5z"/>
                      <path data-property-id="24" d="M873.7 772.9l-62 112.5 42.8 23 62-112.5z"/>
                      <path data-property-id="5" d="M667.5 534.2L621 619.8l36.9 20.1 47.1-85z"/>
                      <path data-property-id="53" d="M519 415.3l57.5 116.1 41.9-20.9-57.2-116.2z"/>
                      <path data-property-id="55" d="M561.2 394.3l57.6 116.3 42.3-21.4-57.8-116z"/>
                      <path data-property-id="59" d="M645.3 352.2L703 468.4l42.2-21.5L687.5 331z"/>
                      <path data-property-id="7" d="M705 554.9l-47.1 85 36.3 20 46.4-85.5z"/>
                      <path data-property-id="9" d="M740.7 574.4l-46.5 85.5 36 19.9 46.1-86.2z"/>
                      <path data-property-id="11" d="M776.3 593.6l-46.1 86.2 35.1 19.4 47.2-85.7z"/>
                      <path data-property-id="15" d="M812.5 613.5l-47.2 85.7 36.1 19.9 46.7-86z"/>
                      <path data-property-id="17" d="M848.1 633.1l-46.7 86 35.9 19.8 46.7-86.2z"/>
                      <path data-property-id="16" d="M702 680l-62 112.5 43.3 23.3 62-112.3z"/>
                      <path data-property-id="27" d="M1027.2 731l-46.1 85.3 35.6 19.5 47-84.9z"/>
                      <path data-property-id="29" d="M1063.7 750.9l-47 84.9 35 19.2 47-84.8z"/>
                      <path data-property-id="54" d="M1109.9 666.7l-46.2 84.2 35 19.3 46.2-84.3z"/>
                      <path data-property-id="52" d="M1073.8 646.9l-46.6 84.1 36.4 20 46.3-84.3z"/>
                      <path data-property-id="78" d="M1238.8 830.2l-29.4 39-107.2-59.6 22.9-41.5z"/>
                      <path data-property-id="86" d="M1126.8 992.3l-31 46.7-92.6-49.7 27.9-50.8z"/>
                    </g>
                    <path data-property-id="26" d="M916.5 795.9l-62 112.5 44 24.7 62-112.5z"/>
                    <path data-property-id="28" d="M960.5 820.6l-62 112.5 42.7 23 62-112.5z"/>
                    <path data-property-id="30" d="M1003.2 843.7l-62 112.5 42.7 23 62-112.5z"/>
                    <path data-property-id="25" d="M991.7 711.5l-47 85.8 36.5 19.1 46-85.4z"/>
                    <path data-property-id="50" d="M1038.3 627.5l-46.6 84 35.5 19.5 46.6-84.1z"/>
                    <path data-property-id="48" d="M1002.7 608l-46.5 84.1 35.5 19.4 46.6-84z"/>
                    <path data-property-id="46" d="M967.2 588.6l-46.6 84 35.6 19.5 46.5-84.1z"/>
                    <path data-property-id="44" d="M931.7 569.1l-46.6 84.1 35.5 19.4 46.6-84z"/>
                    <path data-property-id="42" d="M895.4 549.3l-46.6 84 36.3 19.9 46.6-84.1z"/>
                    <path data-property-id="40" d="M859.1 529.4l-46.6 84.1 36.3 19.8 46.6-84z"/>
                    <path data-property-id="38" d="M822.8 509.6l-46.5 84 36.2 19.9 46.6-84.1z"/>
                    <path data-property-id="36" d="M787.3 490.2l-46.6 84 35.6 19.4 46.6-84.1z"/>
                    <path data-property-id="34" d="M751.6 470.9l-46.6 84 35.7 19.3 46.6-84z"/>
                    <path data-property-id="49" d="M1162.4 570l-46.2 84.5 35.6 19.2 46.1-84.2z"/>
                    <path data-property-id="47" d="M1126.8 550.5l-46.2 84.5 35.6 19.5 46.2-84.5z"/>
                    <path data-property-id="45" d="M1090.4 530.8l-46 84.2 36.2 20 46.1-84.3z"/>
                    <path data-property-id="43" d="M1054.9 511.2l-46.1 84.4 35.6 19.4 46.1-84.4z"/>
                    <path data-property-id="41" d="M1019.4 491.7l-46.2 84.4 35.6 19.5 46.1-84.4z"/>
                    <path data-property-id="39" d="M983.8 472.3l-46.1 84.3 35.5 19.5 46.2-84.4z"/>
                    <path data-property-id="37" d="M948.2 452.8l-46.1 84.4 35.6 19.4 46.1-84.3z"/>
                    <path data-property-id="35" d="M912.7 433.3l-46.2 84.4 35.6 19.5 46.1-84.4z"/>
                    <path data-property-id="33" d="M877.1 413.9L831 498.3l35.5 19.4 46.2-84.4z"/>
                    <path data-property-id="70" d="M1208.5 485.6l-46.2 84.5 35.6 19.4 46.2-84.4z"/>
                    <path data-property-id="68" d="M1172.1 465.9l-46 84.2 36.2 20 46.1-84.3z"/>
                    <path data-property-id="66" d="M1136.6 446.3l-46.1 84.3 35.6 19.5 46.1-84.4z"/>
                    <path data-property-id="64" d="M1101.1 426.8l-46.2 84.4 35.6 19.4 46.1-84.3z"/>
                    <path data-property-id="62" d="M1065.5 407.3l-46.1 84.4 35.5 19.5 46.2-84.4z"/>
                    <path data-property-id="60" d="M1029.9 387.9l-46.1 84.4 35.6 19.4 46.1-84.4z"/>
                    <path data-property-id="58" d="M994.4 368.4l-46.2 84.4 35.6 19.5 46.1-84.4z"/>
                    <path data-property-id="56" d="M965.5 352.6l-104.9 52.2 87.6 48 46.2-84.4z"/>
                    <path data-property-id="57" d="M702.9 468.2l-41.8 21-57.8-116 42-21z"/>
                    <path data-property-id="61" d="M787.3 425.9l-42.1 21L687.5 331l42.1-21z"/>
                    <path data-property-id="63" d="M828.8 405.3l-41.5 20.6L729.6 310l41.5-20.6z"/>
                    <path data-property-id="65" d="M870.3 384.5l-41.5 20.8-57.7-115.9 41.6-20.9z"/>
                    <path data-property-id="67" d="M912 363.7l-41.7 20.8-57.6-116 41.9-20.8z"/>
                    <path data-property-id="69" d="M954.8 342.4L912 363.7l-57.5-116 42-20.9z"/>
                    <path data-property-id="71" d="M996.6 321.4l-41.8 21-58.3-115.6 42.1-20.9z"/>
                    <path data-property-id="73" d="M1033.3 303l-36.7 18.4-58-115.5 42-21.1 36.4 71.9 9.3 24.6z"/>
                    <path data-property-id="73a" d="M1056.2 353.5l-22.9-50.5-7-21.7-9.3-24.6-36.4-71.9 128.9 72.8z"/>
                    <path data-property-id="99" d="M1139.2 140l-56.3 102.6-102.3-57.8 126.6-63.1z"/>
                    <path data-property-id="97" d="M1181.7 164.2l-56.1 102.3-42.7-23.9 56.3-102.6z"/>
                    <path data-property-id="95" d="M1224.2 188.5l-55.7 102-42.9-24 56.1-102.3z"/>
                    <path data-property-id="93" d="M1266.7 212.8l-55.5 101.7-42.9-24.1 55.9-101.9z"/>
                    <path data-property-id="91" d="M1309.1 237l-55.3 101.5-42.6-24 55.5-101.7z"/>
                    <path data-property-id="89" d="M1351.6 261.3l-55.1 101.2-42.7-24 55.3-101.5z"/>
                    <path data-property-id="87" d="M1394.1 285.5l-55 101-42.6-24 55.1-101.2z"/>
                    <path data-property-id="85" d="M1433.9 308.3L1379 409l-39.9-22.5 55-101z"/>
                    <path data-property-id="75a" d="M1145.5 278.1l-66.4 120.3-36.6-20 67.1-120.9z"/>
                    <path data-property-id="75" d="M1187.7 301.4l-65.1 120.7-43.5-23.7 66.4-120.3z"/>
                    <path data-property-id="77" d="M1230.9 325.6l-66.1 119.5-42.2-23 65.1-120.7z"/>
                    <path data-property-id="79" d="M1273.9 349.8l-66.1 118.8-43-23.5 66.1-119.5z"/>
                    <path data-property-id="81" d="M1316.9 374l-66.1 118-43-23.4 66.1-118.8z"/>
                    <path data-property-id="83" d="M1379 409l-84.2 107-44-24 66.1-118z"/>
                    <path data-property-id="122" d="M1283.5 69.1l-57 104.3-102-58.5 126.8-63.6z"/>
                    <path data-property-id="120" d="M1323.7 91.4l-57.2 104.8-40-22.8 57-104.3z"/>
                    <path data-property-id="118" d="M1364 113.6l-57.6 105.6-39.9-23 57.2-104.8z"/>
                    <path data-property-id="116" d="M1404.3 135.9l-58 106.2-39.9-22.9 57.6-105.6z"/>
                    <path data-property-id="114" d="M1445.4 158.6l-58.9 106.6-40.2-23.1 58-106.2z"/>
                    <path data-property-id="112" d="M1486.5 181.4l-59.2 107.2-40.8-23.4 58.9-106.6z"/>
                    <path data-property-id="110" d="M1526.6 203.6L1467 311.3l-39.7-22.7 59.2-107.2z"/>
                    <path data-property-id="108" d="M1567.5 226.1L1505.9 337l-26.4-18.5-12.5-7.2 59.6-107.7z"/>
                    <path data-property-id="106" d="M1608.3 248.7l-63.9 115.2-38.5-26.9 61.6-110.9z"/>
                    <path data-property-id="104" d="M1657 275.6L1573 384l-28.6-20.1 63.9-115.2z"/>
                    <path data-property-id="102" d="M1562.8 400.6l-29.6 39.2-103.2-72.7 30.8-38.4z"/>
                    <path data-property-id="100" d="M1533.2 439.8l-29.5 39.1-104.4-73.4 30.7-38.4z"/>
                    <path data-property-id="98" d="M1503.7 478.9l-29.5 39.2-105.6-74.3 30.7-38.3z"/>
                    <path data-property-id="96" d="M1474.2 518.1l-29.6 39.2-106.7-75.1 30.7-38.4z"/>
                    <path data-property-id="94" d="M1444.6 557.3l-29.5 39.2-108-76 30.8-38.3z"/>
                    <path data-property-id="92" d="M1415.1 596.5l-29.6 39.1-109.1-76.7 30.7-38.4z"/>
                    <path data-property-id="90" d="M1385.5 635.6l-29.5 39.2-110.3-77.6 30.7-38.3z"/>
                    <path data-property-id="88" d="M1356 674.8l-24.9 33.1-125.9-64 6-3.6 34.5-43.1z"/>
                    <path data-property-id="72" d="M1331.1 707.9l-32.4 42.9-126.3-68.5 15.3-27.8 17.5-10.6z"/>
                    <path data-property-id="74" d="M1298.7 750.8l-30 39.7-119.8-65.5 23.5-42.7z"/>
                    <path data-property-id="76" d="M1268.7 790.5l-29.9 39.7-113.7-62.1 23.8-43.1z"/>
                    <path data-property-id="80" d="M1209.4 869.2l-27 40.2-104.2-56.1 24-43.7z"/>
                    <path data-property-id="82" d="M1182.4 909.4l-27.8 41.5-99.7-55.5 23.3-42.1z"/>
                    <path data-property-id="84" d="M1154.6 950.9l-27.8 41.4-95.7-53.8 23.8-43.1z"/>
                    <path data-property-id="18" d="M745.3 703.5l-62 112.5 43.2 23.3 62-112.3z"/>
                    <path data-property-id="19" d="M884 652.7l-46.7 86.2 36.2 19.6 46.9-85.9z"/>
                    <path data-property-id="21" d="M920.4 672.6l-46.9 85.9 35.8 19.7 46.9-86.1z"/>
                    <path data-property-id="23" d="M956.2 692.1l-46.9 86.1 35.4 19.1 47-85.8z"/>
                  </svg>
                </div>
                <div id="markers">
                  <div class="fullSize">
                    <div class="navigatorUnit" 
                      v-for="(property, index) in properties" 
                      :key="index" 
                      :data-property-id="property.id" 
                      style="opacity: 1;" 
                      :class="markerClasses(property)"
                    >
                      <div class="item-wrapper" style="left: 50vw; top: 30px; display: none;">
                        <h2 class="headline" v-text="markerHeadline(property)"></h2>
                        <p v-if="property.forsale" v-text="markerText1(property)"></p>
                        <p v-if="property.forsale" v-text="markerText2(property)"></p>
                      </div>
                    </div>
                    <div class="navigatorUnit soldInitial" data-property-id="00" style="opacity: 1;">
                      <div class="item-wrapper" style="left: 50vw; top: 30px; display: none;">
                        <h2 class="headline">Будинок проданий</h2>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="back-wrapper row bottom-xs hidden-xs" style="flex: 1 1 auto; max-width: 26em;">
          <a href="#" @click.prevent="$modal.show('formBooking')" class="btn btn--gold" data-id="" id="closeGallery" style="flex-grow: 1; display:block; opacity:1; min-width:12vw; z-index:20;">
            <span class="text"><span class="inner">Замовити перегляд</span></span>
            <span class="hover"><span class="inner">Замовити перегляд</span></span>
          </a>
        </div>
        <div class="col-xs-offset relative hidden-xs"></div>
      </div>
    </div>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
import ButtonBack from '@/components/shared/ButtonBack'
import Formbooking from '@/components/shared/Formbooking'

export default {
  name: 'navigator',
  components: {
    'app-shared-button-back': ButtonBack,
    'app-shared-form-booking': Formbooking
  },
  data () {
    return {
      windowHeight: window.innerHeight || document.body.clientHeight,
      windowWidth: window.innerWidth || document.body.clientWidth,
      topOffset: 0
    }
  },
  metaInfo () {
    return {
      title: 'Територія ' + ' - ' + this.websiteTitle
    }
  },
  props: [
    'websiteTitle'
  ],
  computed: {
    ...mapGetters([
      'properties'
    ]),
    svgWrapperHeight () {
      if (this.windowWidth > this.windowHeight) {
        let height = this.windowWidth * 0.5625
        if (height < this.windowHeight) {
          return this.windowHeight
        } else {
          return height
        }
      } else {
        return this.windowHeight
      }
    },
    svgWrapperLeft () {
      if (this.windowWidth > this.windowHeight) {
        return 0
      } else {
        let width = this.windowHeight * 1.777777777777778
        let left = 0 - (width - this.windowWidth) / 2
        return left
      }
    }
  },
  mounted () {
    this.$store.dispatch('imgLoaded')
    window.addEventListener('resize', this.handleWindowResize)
    this.svgWrapperTop()
    setTimeout(() => {
      this.$store.dispatch('animateNavigatorSvg')
    }, 1000)
  },
  beforeRouteLeave (to, from, next) {
    this.$store.dispatch('preloader')
    setTimeout(function () {
      next()
    }, 2000)
  },
  beforeDestroy () {
    window.removeEventListener('resize', this.handleWindowResize)
  },
  methods: {
    handleWindowResize (event) {
      this.windowWidth = window.innerWidth || document.body.clientWidth
      this.windowHeight = window.innerHeight || document.body.clientHeight
      this.svgWrapperTop()
    },
    svgWrapperTop () {
      if (this.windowWidth > this.windowHeight) {
        let topOffset = Math.round((this.windowHeight - this.svgWrapperHeight) / 2)
        this.topOffset = topOffset
      } else {
        this.topOffset = 0
      }
    },
    markerClasses (property) {
      if (property.forsale === false) return 'soldUnit'
      if (property.landplan) return 'landUnit'
      else return ''
    },
    markerHeadline (property) {
      if (property.landplan) {
        if (property.forsale) return 'Вільна ділянка'
        else return 'Ділянка продана'
      } else {
        if (property.forsale) return 'вул. Щаслива, ' + property.id
        else return 'Будинок проданий'
      }
    },
    markerText1 (property) {
      if (property.forsale === false) return
      if (property.landplan) return 'Площа: ' + property.landsize
      else return 'Площа: ' + property.planselect.display
    },
    markerText2 (property) {
      if (property.forsale === false) return
      if (property.landplan) return
      else return 'Ділянка: ' + property.landsize
    }
  }
}
</script>

<style scoped>
#markers .navigatorUnit .item-wrapper {
  background: rgba(0, 0, 0, .5);
}
#markers .navigatorUnit p {
  text-align: right;
  padding-top: 0.5rem;
}
#navigatorSVG path {
  opacity: 0.5;
}
#navigatorSVG #sold path, #navigatorSVG path.sold {
  fill:maroon;
  cursor:default;
}
#navigatorSVG path.sale {
  fill:gold;
}
#navigatorSVG path.land {
  fill:darkolivegreen;
}
</style>
