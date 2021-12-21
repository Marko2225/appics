<template>
  <div id="categories-slider">

  <carousel-3d :width="811" :height="381" :perspective="0" :space="160" :display="5" :scaling="200" >

      <slide v-for="category in categories" :key="category.heading" :index="category.index" class="slide"
      v-bind:style="{ backgroundImage: 'url(' + category.image + ')' }">
        <h1 id="heading"> {{category.heading}} </h1>
        <div class="split">
        <h5 id="posts"> {{category.posts}} </h5>
        <h5 id="usd"> {{category.usd}} </h5>
        </div>
        </slide>

  </carousel-3d>
  </div>
</template>

<script>

import { Carousel3d, Slide } from 'vue-carousel-3d'

export default {
  name: 'categories-slider',
  components: {
    Carousel3d,
    Slide
  },
  data: function () {
    return {
      categories: [
        { index: 0, heading: 'Beauty', posts: '2050 POSTS', usd: 'USD 45.000', image: require('../assets/beauty.png') },
        { index: 1, heading: 'Art', posts: '1005 POSTS', usd: 'USD 30.000', image: 'https://wallpaperaccess.com/full/1816883.jpg' },
        { index: 2, heading: 'Music', posts: '1315 POSTS', usd: 'USD 50.000', image: 'https://img.freepik.com/free-photo/acoustic-classic-guitar-head-blue-background_23-2147926804.jpg?size=626&ext=jpg' },
        { index: 3, heading: 'Fashion', posts: '900 POSTS', usd: 'USD 35.000', image: 'https://i1.wp.com/cooldigital.photography/wp-content/uploads/2013/06/Fashion-photo-of-a-beautiful-elegant-young-woman-in-a-pretty-suit-with-flowers-holding-handbag-posing-over-pink-background.jpg?resize=620%2C413&ssl=1' },
        { index: 4, heading: 'Nature', posts: '650 POSTS', usd: 'USD 6.000', image: 'https://ak.picdn.net/shutterstock/videos/1030633697/thumb/1.jpg' }
      ]
    }
  }
}
</script>

<style scoped>

#categories-slider {
    background-color:#1f273e;
    padding-bottom: 35px;
    padding-top: 52px;
    display: flex;
    justify-content: center;
}
.carousel-3d-slider div[style]  {
  width:811px;
  /* height:381px !important; visina slajdera ako se definise ovde*/
}
.carousel-3d-slider[data-v-07917306] {
  transform-style: unset;
  perspective: 20000;
  overflow: initial;
  }
.carousel-3d-slider {
        height: 202px !important;
}
.slide {
  border-radius: 25px;
  border: 0;
  color:white;
  /* width:550px; */
  /* :width="811" :height="381" */
}

.current {
      border-width: 1px;
    /* width: 812px !; ovde isto moze da se definise duzina */
    /* height: 382px !important; */
    transition: transform 500ms ease 0s, opacity 500ms ease 0s, visibility 500ms ease 0s;
    background-image: url(https://wallpaperaccess.com/full/1816883.jpg);
    background-size: cover;
    background-position: center center;
    position: relative;
}

.right-1 {
    border-width: 1px;
    /* width: 362px; */
    height: 382px !important;
    transition: transform 500ms ease 0s, opacity 500ms ease 0s, visibility 500ms ease 0s;
    background-image: url(https://wallpaperaccess.com/full/1816883.jpg);
    transform: translateX(151px) translateZ(-251.6px) rotateY(0deg)!important;
    z-index: 998;
    opacity: 1;
    visibility: visible;
}

.left-1 {
    border-width: 1px;
    height: 382px !important;
    transition: transform 500ms ease 0s, opacity 500ms ease 0s, visibility 500ms ease 0s;
    background-image: url(https://ak.picdn.net/shutterstock/videos/1030633697/thumb/1.jpg);
    transform: translateX(-151px) translateZ(-251.6px) rotateY(0deg)!important;
    z-index: 998;
    opacity: 1;
    visibility: visible;
}

.left-2 {
  height: 382px !important;
      transform: translateX(-366px) translateZ(-623px) rotateY(0deg)!important;
}

.right-2 {
  height: 382px !important;
  transform: translateX(366px) translateZ(-623px) rotateY(0deg)!important;
}

#heading {
  position: absolute;
  top: 221px;;
  left: 50%;
  font-size: 90px;
  transform: translateX(-50%) translateY(-50%);
  font-family: 'Gotham';
  font-weight: bold
}

#posts {
  position: absolute;
  /* bottom: 60px; */
  left: 50px;
  font-size: 16px;
  top: 308px;
  font-family: 'Gotham';
}

#usd {
  position: absolute;
  /* bottom: 50px; */
  top: 308px;
  right: 49px;
  font-size: 16px;
  font-family: 'Gotham';
}

  @media only screen and (max-width: 1280px) {
    #categories-slider{
      width: 95%;
      margin: 0 auto ;
      /* height: 202px !important; dodati i za flex podesavanja i namestiti padding i margin ili position i top*/
    }

    .carousel-3d-container div[style]{
      width: 301.43px !important;
      height: 202px ;
    }
    .carousel-3d-container{
      overflow: initial;
       width: 301px;
            height: 202px !important;
            /* dodati margin */
    }
    div.carousel-3d-slider {
      /* width: 301.43px !important; */
      /* height: 202px !important; */
    }
  .carousel-3d-slider div[style]{
    height: 202px !important;
        /* position: relative; */
    margin: 0 auto;
    /* transform-style: preserve-3d;
    perspective: 1000px; */
      }
       .carousel-3d-slider {
        height: 202px !important;
      }
    .slide{
        /* margin: 0 18%; */
        border-radius: 15px;
            width: 301px;
            height: 202px;
    }
    .right-1[data-v-0de157cd] {
    /* transform: translateX(151px) translateZ(-251.6px) rotateY(0deg)!important; */
        transform: translate3d(54px,10px,-251px)!important;
    }
    .right-2[data-v-0de157cd] {
    /* transform: translateX(310px) translateZ(-623px) rotateY(0deg)!important; */
        transform: translate3d(131px,19.5px,-623px)!important;
    }
.left-1 {
  transform: translate3d(-54px,10px,-251px)!important;
  }
  .left-2 {
    /* transform: translateX(-310px) translateZ(-623px) rotateY(0deg)!important; */
        transform: translate3d(-131px,19.5px,-623px)!important;
    }
    #heading {
  position: absolute;
  top: 118.39px;;
  left: 50%;
  font-size: 30px;
  transform: translateX(-50%) translateY(-50%);
  font-family: 'Gotham';
  /* font-weight: bold */
}
#posts {
  position: absolute;
  /* bottom: 60px; */
  left: 18.83px;
  font-size: 8px;
  top: 162.76px;
  font-family: 'Gotham';
}
#usd {
  position: absolute;
  top: 162.76px;
  /* bottom: 50px; */
  right: 18.83px;
  font-size: 8px;
  font-family: 'Gotham';
}
  }

  @media only screen and (max-width: 990px) {
    #categories-slider {
    padding-bottom: 35px;
    padding-top: 12px;
}
    .carousel-3d-container div[style]{
      /* width: 320px !important;
      height: 180px !important; */
    }
    .slide{
        /* margin: 0 0 0 18% !important; */
    }
  }

</style>
