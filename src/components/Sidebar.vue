<template>
<div class="sidebar">
    <input type="checkbox" id="click">
    <div id="logo">
        <label for="click"><img src="@/assets/logo_icon.svg"/></label>
    </div>
    <div id="sidebar-content">
            <div id="close-sidebar">
                <img id="logo-tablet-close" src="../assets/logo_icon_tablet.svg" alt="logo icon tablet">
                <label for="click"><img id="close-icon" src="../../public/icons/icon_close.svg" alt="close icon tablet"/></label>
            </div>
            <div class="nav-btn links active">
                <img class="nav-icon" src="../../public/icons/icon-nav1.svg"/>
                Trending
            </div>
            <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon-nav2.svg"/>
                HOT
            </div>

            <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon-nav3.svg"/>
                New
            </div>

        <div class="sidebar-section-space">
            <p>TOP CATEGORIES</p>
        </div>
        <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon_beauty.svg"/>
                    BEAUTY
             </div>
        <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon_sports.svg"/>
                SPORTS
             </div>
        <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon_food.svg"/>
                FOOD
             </div>
        <div class="nav-btn links">
                <img class="nav-icon" src="../../public/icons/icon_travel.svg"/>
                TRAVEL
             </div>

        <div class="sidebar-section-space-2">
            <p>SPECIAL CONTETNT</p>
            <div class="about">
                <div class="nav-btn2">USER STORIES</div>
                <div class="nav-btn2">TIPPS & TRICKS</div>
                <div class="nav-btn2">CHARITY</div>
            </div>
            <button id="sidebar-btn" class="links">
                became a creator
            </button>
        </div>

    </div>

</div>
</template>

<script>
export default {
  name: 'sidebar'
}
</script>

<style scoped>

.sidebar {
    height: 100%;
    width: 100%;
}
input  {
    display: none;
}

.body-text {
margin-left: 150px;
font-size: 18px;
}

#logo {
    position:relative;
    float: left;
    margin-left: 47px;
    margin-top: 47px;
    margin-bottom: 5px;
    display:block;
}

#sidebar-content {
    float:left;
    margin-top: 0px;
    width: 100%;
    text-align: left;
    color:white;
    padding: 0;
    font-family: 'Gotham', sans-serif;
    font-size: 13px !important;
    background-color: rgb(18,25,44);
    display: table;
    margin-bottom: 0;
}
/* #click:checked ~ #sidebar-content{
      width: 100%;
      display: block;
      z-index: 1!important;
    visibility: visible;
    position: absolute;
    } */
    #close-sidebar {
        height: 93px;
        width: 100%;
        display: block;
    }
    img#logo-tablet-close {
    width: 29px;
    height: 29px;
    top: 22px;
    position: relative;
    /* visibility: visible; */
    display: none;
}
img#close-icon {
    height: 23px;
    width: 23px;
    position: absolute;
    left: 24.54px;
    top: 27.04px;
    /* visibility: visible; */
    display: none;
}

.links {
  letter-spacing: 0px;
  line-height: 36px;
  color: #FFFFFF;
  display: block;
  /* transition: 0.3s; */
  /* margin-bottom: 9px; */
 height: 35px;
 border-left: 2px solid;
border-color: rgba(197,156,102, 0);
}
.active {
     background-image: linear-gradient(to right, rgba(197,156,102, 0.1), rgba(18,25,44, 1));
    border-left: 2px solid;
    border-color: rgba(197,156,102, 0.8);
    color: #C59C66;
}

.sidebar-section-space{
    margin-top: 56px;
    /* padding: 0 25px; */
    margin-bottom: 13px;
}
.sidebar-section-space-2{
    margin-top: 63px;
    /* margin-left: 54px; */
    letter-spacing: -0.5px;
}
.sidebar p{
    font-size: 11px;
    color: #888;
    font-weight: 500;
    /* margin: revert; */
    /* margin-bottom: 13px; */
    padding-left: 54px;
    margin: 0;
}

#special-content {
    padding: 0;
    margin-left: 25px;
    font-family: 'Gotham', sans-serif;
    font-size: 13px !important;
}

.nav-btn {
    padding-left: 52px;
    margin-bottom: 8.7px;
    /* margin-top: 4px; */
}
.nav-btn2{
    margin: 25.3px 0;
}
.about{
    /* margin-top: 20px; */
    margin-top: -6.5px;
    line-height: 20px;
    /* margin-left: 54px; */
    padding-left: 54px;
}

.nav-icon {
    margin-right: 15px;
    margin-top: -2px;
}

#sidebar-btn {
    /* padding: 5px 18px; */
    color: #D4A268;
    line-height: 17px;
    border: 2px solid #D4A268;
    margin:44.5px 0 46px 42px;
    /* padding: 5px 25px; */
    width: auto;
    font-size: 14px;
    /* transition: all 0.7s ease; */
    background: rgba(212,162,104,0) !important;
    width: 180px;
    height: 45px;
    letter-spacing: -0.8px;

}

#sidebar-btn:hover {
color:#a87e51;
border: 2px solid #a87e51;
background-color: #090d17;
}
 /* #ck:checked ~ .main-content
 header input label img:before {
     content: url("../../public/icons/icon-nav2.svg");
     position: relative;
    } */

.sidebar-item{
    display: block;
    position: relative;
    padding-left: 25px !important;
}

.block {
    display:block;
    margin: 0 !important;
    padding: 10px 0 10px 25px !important;
}
@media only screen and (max-width: 990px) {
    #click:checked ~ #sidebar-content{
      width: 100%;
      display: block;
      z-index: 1!important;
    visibility: visible;
    position: absolute;
    height: inherit;
    }
     #close-sidebar {
        display: flex;
        justify-content: center;
    }
    img#logo-tablet-close {
display: flex;
}
img#close-icon {
display: flex;
cursor: pointer;
}
.nav-btn[data-v-7d622f5c] {
    padding-left: 24px;
    margin-bottom: 9px;
    /* margin-top: 4px; */
}
.active[data-v-7d622f5c] {
    background-image: linear-gradient(to right, rgba(197,156,102, 0.1), rgba(18,25,44, 1));
    border-left: 4px solid;
}
.sidebar-section-space {
    margin-top: 56px;
    margin-top: 35px;
    /* padding: 0 25px; */
    margin-bottom: 11.5px;
    font-family: inherit;
}
.sidebar p {
    padding-left: 26px;
}
.sidebar-section-space-2[data-v-7d622f5c] {
    margin-top: 30px;
    /* margin-left: 54px; */
    letter-spacing: -0.5px;
}
.about {
    margin-top: 22px;
    margin-top: -7px;
    line-height: 16px;
    /* margin-left: 54px; */
    font-size: 13px;
    padding-left: 26px;
}
#sidebar-btn[data-v-7d622f5c] {
    color: #D4A268;
    border: 2px solid #D4A268;
    /* margin: 35.5px 0 38px 25px; */
    margin: 36.5px 0 45px 25px;
}
}
</style>
