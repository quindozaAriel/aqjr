<template>
  <div class="navigation-bar">
    <a class="brand-logo" href="#"></a>
    <ul class="top-nav nav-menu">
      <li>
        <a href="#">About</a>
      </li>
      <li>
        <a href="#">Portfolio</a>
      </li>
      <li>
        <a href="#">Contact</a>
      </li>
    </ul>
    <ul class="top-nav nav-trigger">
      <li><font-awesome-icon icon="bars"/></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "NavBar",

};
</script>

<style lang="scss" scoped>
@import "../assets/animation.scss";
@import "../assets/mediascreens.scss";

.navigation-bar {
  position: fixed;
  width: 100%;
  height: 100px;
  color: white;
  font-weight: 100;
  margin-top:20px;
}

.brand-logo{
  width:100px;
  height:100%;
  float:left;
  margin-left:50px;
  background-image:url("../assets/initial.png");
  background-size:100px 80px;
  background-repeat:no-repeat;
  background-position:center;
}

.top-nav {
  list-style-type: none;
  margin: 0;
  padding: 0;
  height: 100%;
  float: right;
  display: flex;
  align-items: center;
  transition:all 1s;
  @include animation(0, 0.5s, slideLeft, 1, linear);

  a {
    color: White;
    text-decoration: none;
  }

  li {
    display: inline;
    font-size: 20px;
    margin-right: 80px;
    cursor: pointer;
  }
}

@include xs{
   .nav-menu{
     display:none;
   }
}

@include sm{
   .nav-menu{
     display:none;
   }
}

@include md{
  .nav-menu{
     display:flex;
   }

   .nav-trigger{
     display:none;
   }
}

@include lg{
  .nav-menu{
     display:flex;
   }

   .nav-trigger{
     display:none;
   }
}

@include xl{
   .nav-menu{
     display:flex;
   }

   .nav-trigger{
     display:none;
   }
}
</style>