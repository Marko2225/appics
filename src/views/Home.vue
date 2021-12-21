<template>
  <div class="home">
    <div class="side-bar">
      <sidebar />
    </div>
    <div class="main-content">
      <header>
        <div class="search-container">
          <form>
            <button type="submit" class="button">
              <img class="nav-icon" src="../../public/icons/icon_search.svg" />
            </button>
            <input
              type="text"
              class="input"
              placeholder="search your favorite content"
            />
          </form>
        </div>
        <!--  end search container -->
        <!-- <input type="checkbox" id="ck" /> -->
        <label for="click" id="hamburger"
          ><img class="nav-icon" src="../../public/icons/icon_hamburger.svg" />
        </label>
        <img
          id="logo-tablet"
          src="@/assets/logo_icon_tablet.svg"
          alt="logo icon tablet"
        />
        <img
          id="search-tablet"
          src="../../public/icons/icon_search_tablet.svg"
          alt="search button tablet "
        />
        <div class="username">
          Hello <span>Martin Flenders</span>
          <img src="@/assets/username.png" alt="username" />
        </div>
      </header>
      <categories-slider />
      <!-- <b-button variant="outline-primary">Button</b-button> -->
      <div class="top-creators">
        <h6>TOP CONTENT CREATORS</h6>
        <p>THIS WEEK</p>
        <ul>
          <li>
            <div class="creator">
              <!-- <img src="https://mooresvilleeyecare.com/wp-content/uploads/2019/01/sunglasses-optical-store-near-you-mooresville-nc.jpg" alt="creator 1"> -->
              <img src="@/assets/creator1.png" alt="creator 1" />
              <p>Lex Maybour</p>
              <span>Sports</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://lh3.googleusercontent.com/Ca_sXZA6EgOFa0MuKvUMgm6dBFCw4LrKMvxsPqNczhZfxzqsNlDuQUB9qIP8OOroUjTWnP8RKxVUDIcgb-uQQg4A3xz4wrXNsmw=w315" alt="creator 2"> -->
              <img src="@/assets/creator2.png" alt="creator 2" />
              <p>Antoine Braxton</p>
              <span>Lifestyle</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://miami.momcollective.com/wp-content/uploads/2019/08/facial-expression-fashion-hairstyle-1674752-e1566182464204-600x523.jpg" alt="creator 3"> -->
              <img src="@/assets/creator3.png" alt="creator 3" />
              <p>Luisanne Boa</p>
              <span>Art</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://ronfieldsnutrition.co.uk/wp-content/uploads/2020/05/lyndsay.png" alt="creator 4"> -->
              <img src="@/assets/creator4.png" alt="creator 4" />
              <p>Mariah Xamons</p>
              <span>Beauty</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://loveincorporated.blob.core.windows.net/avatars/users/358111.jpg" alt="creator 5"> -->
              <img src="@/assets/creator5.png" alt="creator 5" />
              <p>Jung Su</p>
              <span>Tech</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://yt3.ggpht.com/ytc/AKedOLSl1xdUqFKVK9Fxl9RW8o2FWpY1IXJVswhlv1yVLQ=s900-c-k-c0x00ffffff-no-rj" alt="creator 6"> -->
              <img src="@/assets/creator6.jpg" alt="creator 6" />
              <p>Max Harison</p>
              <span>Travel</span>
            </div>
          </li>
          <li>
            <div class="creator">
              <!-- <img src="https://lh3.googleusercontent.com/dXSfCQrVvlMka86ggFIDzzbdBSDgNpJg-9ivvnSvkl4bzZnMk7VV0gpypvxoDtRopoOD-A=s85" alt="creator 7"> -->
              <img src="@/assets/creator7.png" alt="creator 7" />
              <p>Sarah Maron</p>
              <span>Music</span>
            </div>
          </li>
        </ul>
      </div>
      <!--  end top creators -->
      <div class="categories">
        <div id="travel">
          <img
            class="icon_category"
            src="../../public/icons/icon_travel_categories.svg"
          />
          <p>TRAVEL</p>
        </div>
        <div id="fashion">
          <img
            class="icon_category"
            src="../../public/icons/icon_fashion_categories.svg"
          />
          <p>FASHION</p>
        </div>
        <div id="music">
          <img
            class="icon_category"
            src="../../public/icons/icon_music_categories.svg"
          />
          <p>MUSIC</p>
        </div>
        <div id="food">
          <img
            class="icon_category"
            src="../../public/icons/icon_food_categories.svg"
          />
          <p>FOOD</p>
        </div>
      </div>
      <!--  end categories -->
      <footer>
        <span
          >Powered By &copy;
          <a
            href="https://www.linkedin.com/in/marko-markovic-a3b32066/"
            target="_blank"
            >Marko Markovic</a
          ></span
        >
      </footer>
    </div>
    <!--  end main content -->
  </div>
  <!--  end Home -->
</template>

<script>
// @ is an alias to /src

import CategoriesSlider from '../components/CategoriesSlider.vue'
import Sidebar from '../components/Sidebar.vue'

export default {
  name: 'Home',
  components: {
    CategoriesSlider,
    Sidebar
  }
}
</script>

<style scoped>
body {
}
.home {
  position: relative;
}
.side-bar {
  height: 100%;
  width: 320px;
  position: absolute;
  top: 0;
  left: 0;
  /* padding-top:20px; */
  background-color: #12192c;
}
.main-content {
  margin-left: 320px;
  width: auto;
  /* height: 100vh; */
  background-color: #1f273e;
  /* padding: 30px 0px; */
  /* overflow-x: clip; */
}
/*header*/
header {
  width: 100%;
  height: 107px;
  /* background-color: inherit; */
  /* background: rebeccapurple;
    opacity: 0.9; */
  /* background: rgba(76, 175, 80, 0.1); */
  background: rgba(31, 39, 62, 0.2);
  position: sticky;
  top: 0;
  z-index: 1;
}
.search-container {
  height: 27px;
  width: 215px;
  /* background-color: rgb(217, 255, 0); */
  position: absolute;
  left: 49.56px;
  top: 56px;
}
form {
  background: transparent;
  display: flex;
}
.button {
  cursor: pointer;
  background: transparent;
  border: 0;
  margin: 0;
  padding: 0;
}
.input {
  height: 50%;
  width: 238px;
  padding: 0;
  line-height: 16.8px;
  border: 0;
  padding-left: 10px;
  background: transparent;
  /* Font-family: Roboto; */
  font-style: Regular;
  font-size: 14px;
  color: white;
}
::-webkit-input-placeholder {
  color: #949292;
}
.username {
  height: 40px;
  width: 200px;
  color: #c59c66;
  font-size: 13px;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  position: absolute;
  right: 81px;
  top: 46px;
}
.username > span {
  padding: 0 19px 0 7px;
  color: #ffffff;
}
.username > img {
  height: 40px;
  width: 40px;
  border-radius: 50%;
}

#hamburger {
  display: none;
}
#logo-tablet {
  display: none;
}
#search-tablet {
  display: none;
}
/* top creators div */
.top-creators {
  width: calc(100% - 76px);
  height: 309px;
  /* background-color: lightblue; */
  margin-left: 76px;
  text-align: left;
  overflow-x: clip;
}
.top-creators > h6 {
  font-size: 16px;
  font-weight: 700;
  color: white;
  margin-top: -2px;
  padding-left: 8px;
  letter-spacing: 1.2px;
}
.top-creators > p {
  margin-top: 12px;
  margin-bottom: 42px;
  font-size: 14px;
  font-weight: 400;
  color: #949292;
  padding-left: 8px;
}
.top-creators > ul {
  display: flex;
  margin: 0;
  padding: 0;
  justify-content: space-between;
  overflow-x: auto;
  scrollbar-color: RGBA(136, 136, 136, 0) RGBA(241, 241, 241, 0); /* only firefox*/
  scrollbar-width: thin; /* only firefox*/
}
.top-creators > ul:hover {
  scrollbar-color: RGBA(136, 136, 136, 1) RGBA(241, 241, 241, 0.1);
}
.top-creators > ul li {
  list-style-type: none;
  margin: 0 36px 0 0;
  background: #1f273e;
}
.creator {
  text-align: center;
  width: 105px;
  height: 170px;
}
.creator > img {
  width: 84px;
  height: 84px;
  border-radius: 50%;
}
.creator > p {
  margin-top: 17px;
  margin-bottom: 0px;
  font-size: 14px;
  font-weight: 500;
  color: #ffffff;
  width: 106px;
  text-align: center;
}
.creator > span {
  color: #949292;
}
/* categories div */
.categories {
  margin-left: 86px;
  /* background-color: lightcyan; */
  width: calc(100% - 86px);
  padding-bottom: 28px;
  /* margin-bottom: 50px; */
  overflow-x: auto;
  /* height: 260px; */
  /* padding: 0; */
  /* direction: unset; */
  display: grid;
  grid-auto-flow: column;
  scrollbar-color: RGBA(136, 136, 136, 0) RGBA(241, 241, 241, 0); /* only firefox*/
  scrollbar-width: thin; /* only firefox*/
}
.categories:hover {
  scrollbar-color: RGBA(136, 136, 136, 1) RGBA(241, 241, 241, 0.1); /* only firefox*/
  /* opacity: 1; */
}
#travel {
  width: 252px;
  height: 150px;
  /* background-color: #5AB5E8; */
  background-image: linear-gradient(#5ab5e8, #5e9feb);
  border-radius: 16px;
  margin-right: 38px;
}
#fashion {
  width: 252px;
  height: 150px;
  /* background-color: #5AB5E8; */
  background-image: linear-gradient(#e7307d, #f02f56);
  border-radius: 16px;
  margin-right: 38px;
}
#music {
  width: 252px;
  height: 150px;
  /* background-color: #5AB5E8; */
  /* background-image: linear-gradient(#5AB5E8, #5E9FEB); */
  background-color: #fff2c3;
  border-radius: 16px;
  margin-right: 38px;
}
#food {
  width: 252px;
  height: 150px;
  background-color: #c59c66;
  /* background-image: linear-gradient(#5AB5E8, #5E9FEB); */
  border-radius: 16px;
}

#travel > img {
  position: relative;
  float: left;
  padding-left: 62.9px;
  /* bottom: 32%; */
  top: 38%;
}
#travel > p {
  margin-top: 62px;
  /* margin-bottom: 9rem; */
  margin-left: 44px;
  font-size: 18px;
  color: white;
  font-weight: 500;
}
#fashion > img {
  position: relative;
  float: left;
  padding-left: 60.9px;
  /* bottom: 32%; */
  top: 38%;
}
#fashion > p {
  margin-top: 62px;
  /* margin-bottom: 9rem; */
  margin-left: 44px;
  font-size: 18px;
  color: white;
  font-weight: 500;
}
#music > img {
  position: relative;
  float: left;
  padding-left: 70px;
  /* bottom: 32%; */
  top: 38%;
}
#music > p {
  margin-top: 62px;
  /* margin-bottom: 9rem; */
  margin-left: 44px;
  font-size: 18px;
  color: #835a2a;
  font-weight: 500;
}
#food > img {
  position: relative;
  float: left;
  padding-left: 59px;
  /* bottom: 32%; */
  top: 38%;
}
#food > p {
  margin-top: 62px;
  /* margin-bottom: 9rem; */
  margin-left: 44px;
  font-size: 18px;
  color: white;
  font-weight: 500;
}
footer {
  height: 50px;
  color: white;
}
footer > span {
  position: relative;
  top: 20px;
}
footer > span > a {
  text-decoration: auto;
}
@media only screen and (max-width: 600px) {
}

@media only screen and (max-width: 990px) {
  .side-bar {
    /* display: none; */
    position: absolute;
    z-index: 2;
    padding: 0;
    margin: 0;
    /* padding-top: 150px; */
    width: 100%;
    visibility: collapse;
  }
  .main-content {
    margin: 0 !important;
  }
  header {
    height: 77px;
  }
  #hamburger {
    display: flex;
    position: absolute;
    left: 22px;
    top: 31px;
    cursor: pointer;
  }
  #logo-tablet {
    position: inherit;
    top: 22px;
    display: initial;
  }
  #search-tablet {
    top: 21px;
    right: 20px;
    position: absolute;
    display: block;
  }
  header > .search-container {
    display: none;
  }
  header > .username {
    display: none;
  }
  /* top creators div */
  .top-creators {
    width: calc(100% - 19px);
    height: 240px;
    /* background-color: lightblue; */
    margin-left: 19px;
  }
  .top-creators > h6 {
    /* font-size: 16px; */
    /* font-weight: 700; */
    /* color: white; */
    margin-top: -4px;
    padding-left: 10.5px;
  }
  .top-creators > p {
    margin-top: -3px;
    margin-bottom: 14px;
    font-size: 14px;
    font-weight: 400;
    color: #949292;
    padding-left: 9px;
  }
  .top-creators > ul li[data-v-fae5bece] {
    /* list-style-type: none; */
    margin: 0 16px 0 0;
    /* background: #1F273E; */
  }
  .creator[data-v-fae5bece] {
    height: 160px;
  }
  .creator > p[data-v-fae5bece] {
    margin-top: 12px;
    margin-bottom: -3px;
  }
  /* .categories div */
  .categories {
    margin-left: 18px;
    /* background-color: lightcyan; */
    width: calc(100% - 18px);
    margin-bottom: 0px;
  }
  #travel {
    width: 165px;
    height: 98px;
    /* background-color: #5AB5E8; */
    background-image: linear-gradient(#5ab5e8, #5e9feb);
    border-radius: 16px;
    margin-right: 24.83px;
  }
  #travel > img {
    position: relative;
    float: left;
    padding-left: 40.5px;
    /* bottom: 32%; */
    top: 35.28px;
    height: 20.25px;
    /* width: 25px; */
  }
  #travel > p[data-v-fae5bece] {
    margin-top: 36px;
    /* top: 42px; */
    /* margin-bottom: 47px; */
    margin-left: 33px;
    font-size: 13px;
    color: white;
    font-weight: 500;
    /* position: relative; */
    letter-spacing: 0.5px;
  }
  #fashion {
    width: 165px;
    height: 98px;
    /* background-color: #5AB5E8; */
    background-image: linear-gradient(#e7307d, #f02f56);
    border-radius: 16px;
    margin-right: 24.83px;
  }
  #fashion > img {
    position: relative;
    float: left;
    padding-left: 38.78px;
    /* bottom: 32%; */
    top: 31.66px;
    height: 24.29px;
    /* width: 25px; */
  }
  #fashion > p[data-v-fae5bece] {
    margin-top: 36px;
    /* top: 42px; */
    /* margin-bottom: 47px; */
    margin-left: 33px;
    font-size: 13px;
    color: white;
    font-weight: 500;
    /* position: relative; */
    letter-spacing: 0.5px;
  }
  #music {
    width: 165px;
    height: 98px;
    /* background-color: #5AB5E8; */
    /* background-image: linear-gradient(#5AB5E8, #5E9FEB); */
    background-color: #fff2c3;
    border-radius: 16px;
    margin-right: 24.83px;
  }
  #music > img {
    position: relative;
    float: left;
    padding-left: 40.78px;
    /* bottom: 32%; */
    top: 35.66px;
    height: 22px;
    /* width: 25px; */
  }
  #music > p {
    margin-top: 36px;
    /* top: 42px; */
    /* margin-bottom: 47px; */
    margin-left: 33px;
    font-size: 13px;
    color: #835a2a;
    font-weight: 500;
    /* position: relative; */
    letter-spacing: 0.5px;
  }
  #food {
    width: 165px;
    height: 98px;
    background-color: #c59c66;
    /* background-image: linear-gradient(#5AB5E8, #5E9FEB); */
    border-radius: 16px;
  }
  #food > img {
    position: relative;
    float: left;
    padding-left: 43.5px;
    /* bottom: 32%; */
    top: 35.28px;
    height: 22.25px;
    /* width: 25px; */
  }
  #food > p {
    margin-top: 36px;
    /* top: 42px; */
    /* margin-bottom: 47px; */
    margin-left: 38px;
    font-size: 13px;
    color: white;
    font-weight: 500;
    /* position: relative; */
    letter-spacing: 0.5px;
  }
  footer {
    display: none;
  }
}
/* ::-webkit-scrollbar  for chromr safari edge opera  */
/* width height */
::-webkit-scrollbar {
  width: 8px;
  height: 8px;
}

/* Track */
::-webkit-scrollbar-track {
  background: RGBA(241, 241, 241, 0);
  border-radius: 10px;
  box-shadow: inset 0 0 5px;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: RGBA(136, 136, 136, 0);
  border-radius: 10px;
}

/* Handle on hover */
/* ::-webkit-scrollbar-thumb:hover  for chromr safari edge opera { */
/* ::-webkit-scrollbar-thumb:hover {} */

.categories:hover::-webkit-scrollbar-thumb {
  background: RGBA(136, 136, 136, 1);
}
.categories:hover::-webkit-scrollbar-track {
  background: RGBA(241, 241, 241, 0.1);
}
.top-creators > ul:hover::-webkit-scrollbar-thumb {
  background: RGBA(136, 136, 136, 1);
}
.top-creators > ul:hover::-webkit-scrollbar-track {
  background: RGBA(241, 241, 241, 0.1);
}
@media only screen and (max-width: 1200px) {
}
</style>
