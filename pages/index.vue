<template>
  <!--Dressage Dancers: this is the main page - preview page-->
  <section class="container">
<head>
   <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.11.2/css/all.css" integrity="sha384-KA6wR/X5RY4zFAHpv/CnoG2UW1uogYfdnP67Uv7eULvTveboZJg0qUpmJZb5VqzN" crossorigin="anonymous">
</head>

<h1 class="title">
  Dressage Dancers
</h1>
<h2 class="subtitle">
  Home for all of your Horse Needs
</h2>

  <main>
    <!--main menu item circle-->
    <div class="circular circleW">
      <h1 class="menu-title">Menu</h1>
       <div class="text">
       <div class="horse-nav">
         <nuxt-link to="/horsetwo" class="horse-list">About</nuxt-link>
         <nuxt-link to="/horsethree" class="horse-list">Services</nuxt-link>
         <nuxt-link to="/horsefour" class="horse-list">Trainer</nuxt-link>
       </div>
       </div>
     </div>

    <!--About Boarding Sevices preview item-->
    <div class="circular one">
      <div class="text">
        <div class="preview-title">
          <h1 class="white-title boarding">Our Boarding Services</h1>
        </div>
        <p class="transbox">We provide a number of services for horse needs: boarding, trailer parking and turnout.
         <br><nuxt-link to="/horsethree" class="preview-link">Click here for more information</nuxt-link></p>
      </div>
    </div>

    <!--About Us preview item circle-->
    <div class="circular two">
      <div class="text">
        <div class="preview-title">
          <h1 class="white-title about">About Us</h1>
        </div>
        <p class="transbox">Dressage Dancers is a barn owned and managed by Carol Hopkins. There are also pasture and arena areas along with an inhouse barn assistant.
         <br><nuxt-link to="/horsetwo" class="preview-link">Click here for more information</nuxt-link></p>
      </div>
    </div>

    <!--Riding Trainer preview item circle-->
    <div class="circular three">
      <div class="text">
        <div class="preview-title">
          <h1 class="white-title trainer">Riding Trainer</h1>
        </div>
        <p class="transbox">We have on-sight trainers who can provide dressage lessons for all skill levels.
         <br><nuxt-link to="/horsefour" class="preview-link">Click here for more information</nuxt-link></p>
      </div>
    </div>

    <!--<img src="@/assets/images/horsearena.jpg" alt="woman in riding helmet in a horse arena">-->

  </main>
  <br>
  <!--footer stuff-->
  <div class="horse-box">
    <footer>

      <div class="horse-foot">
        <h3>We Are Located at:</h3>
        <p>21718 NE 161st St.</p>
        <p>Woodenville, WA 98077</p>
      </div>

      <div class="horse-foot">
          <div class="fb-layout">
        <h3>Connect</h3>
        <!--facebook stuff-->

   <i class="fab fa-facebook social-horse"></i>
   <a href="https://www.facebook.com/DressageDancers/"><button class="dressage-facebook">Facebook</button></a>
 </div>
      </div>

      <div class="horse-foot">
        <h3 class="less">Contact Us</h3>
        <p>Email: dressagedancers@gmail.com</p>
        <p>Phone: 425-889-6468</p>
      </div>

    </footer>
  </div>
</section>
</template>

<script>

</script>

<style>
* {
  box-sizing: border-box;
}

.container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  background-position: center center;
  background-repeat: no-repeat;
  background: linear-gradient(rgba(242, 42, 42, 0.72),
      rgba(242, 42, 42, 0.72)),
    url('../assets/images/horsearena.jpg');
  background-size: cover;
}

.title {
  font-family: 'Tangerine', cursive, Arial, serif;
  text-align: center;
  /* 1 */
  display: block;
  font-weight: 300;
  font-size: 850%;
  color: black;
  letter-spacing: 1px;
}

.subtitle {
  text-align: center;
  font-weight: 300;
  font-size: 200%;
  color: #ffa64d;
  word-spacing: 5px;
  padding-bottom: 10px;
}

/*container for the main page preview circles*/
main {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

/*this is the circle template for all of the preview objects*/

.circular {
  width: 200px;
  height: 200px;
  margin-left: 1%;
  border-radius: 50%;
  transition: all 0.3s ease-in-out;
}

/*All the hover effects - tada!*/
.circular:hover {
  border-radius: 0;
  height: 400px;
  cursor: pointer;
}

.circular:hover .text {
  padding-top: 40px;
  opacity: 1;
  }


  .text {
    color: black;
    font-weight: bold;
    opacity: 0;
    text-align: left;
    margin: auto 0;
    transition: all 0.3s ease-in-out;
  }



.menu-title {
  margin-top: 30%;
  text-align: center;
  color: white;
  font-weight: normal;
  font-size: 250%;
  }

.white-title {
  text-align: center;
  color: white;
  &.boarding {
    padding: 1%;
  }
  &.about {
    margin: 50%;
    padding: 30%;
  }
  &.trainer {
    padding: 10%;
  }
}

/*Here is the welcome menu - hope to add a verticle nav bar*/
.circleW {
/*  background: url(https://d13yacurqjgara.cloudfront.net/users/212457/screenshots/2212523/yo.jpg) #000;
*/
background-color: black;
}

/*this is the About Our School menu item*/
.one {
  background: url("../assets/images/barnandstable.jpg");
  background-position: right 35% top 35%;
}

/*this is the Bording Policies menu item*/
.two {
  background: url("../assets/images/carolandhorse.jpg");
  background-position: center top 60%;
  background-size: 140%;
  background-repeat: no-repeat;
}

/*this is the Student Success Stories menu item*/
.three {
  background: url("../assets/images/whitehorsehead.jpg");
  background-size: 160%;
  background-position: right 10% top 50%;
  background-repeat: no-repeat;
}

/*styling for specific items*/
a {
  color: white;
  text-decoration: none;
}

.horse-list {
padding: 10px;
}

.horse-nav {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-left: 2.5rem;
  color: white;
  font-size: 150%;
  list-style: none;
  }

  .preview-link {
    font-size: 80%;
    color: blue;
  }
/*this is a fancy frame around the headers like a frame for a protrait*/
.preview-title {
  border: 20px solid #b88846;
  margin-bottom: 1.5rem;
  border-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='75' height='75'%3E%3Cg fill='none' stroke='%23B88846' stroke-width='2'%3E%3Cpath d='M1 1h73v73H1z'/%3E%3Cpath d='M8 8h59v59H8z'/%3E%3Cpath d='M8 8h16v16H8zM51 8h16v16H51zM51 51h16v16H51zM8 51h16v16H8z'/%3E%3C/g%3E%3Cg fill='%23B88846'%3E%3Ccircle cx='16' cy='16' r='2'/%3E%3Ccircle cx='59' cy='16' r='2'/%3E%3Ccircle cx='59' cy='59' r='2'/%3E%3Ccircle cx='16' cy='59' r='2'/%3E%3C/g%3E%3C/svg%3E")25;
}

.transbox {
  width: 100%;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
  }

footer {
  display: flex;
  flex-direction: row;
  justify-content: center;
}

.horse-box {
  width: 100%;
  background-color: #ffffff;
  border: 1px solid black;
  opacity: 0.6;
}

.horse-foot {
  padding: 5%;
}

.fb-layout {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.social-horse {
  margin-top: 2%;
  font-size: 30px;
  color: blue;
}

.dressage-facebook {
  background-color: blue;
  color: white;
  font-weight: bold;
  border-radius: 2rem;
  cursor: pointer;
}

@media only screen and (max-width: 600px) {
  main {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .circular:hover .text {
      font-size: 80%;
      padding-top: 4px;
      }

      .preview-title {
        margin-bottom: .5rem;
          }

/*this is the About Our School menu item*/
      .one {
      background-position: right 35% bottom 80%;
      background-size: 200%;
      background-repeat: no-repeat;
      }

      /*this is the Bording Policies menu item*/
      .two {
        background-position: left 65% bottom 60%;
        background-size: 200%;
        }

      /*this is the Student Success Stories menu item*/
      .three {
        background-size: 160%;
        background-position: right 10% top 5%;
      }

  .about-section-one{
    display: flex;
    flex-direction: column-reverse;
    align-items: center;
  }
  .about-link {
    margin-right: .5rem;
  }

.arrow {
  display: none;
}

  footer {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .horse-foot {
    text-align:center;
    }

}

@media only screen and (max-width: 780px) {
.circular {
  width: 150px;
  height: 150px;
}

  footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    }
    .horse-foot {
      text-align: center;
    }
}
</style>
