<template>
  <div class="main">
    <div class="container">
      <div class="nav">
        <div class="logo">Introduction</div>
        <div class="navlinks">
          <router-link to="#">Home</router-link>
          <router-link to="#">About</router-link>
          <router-link to="#">Contact</router-link>
          
        </div>
      </div>
      <div class="content">
        <div class="left">
          <img src="@/assets/me.png" />
        </div>
        <div class="right">
      <div class="heading">
            Hello, <br />
          This is <span>Suraj Dubey</span> <br />
          A Front End Developer.
      </div>

          <div class="btn-div">
          <button id="btn">See My Work</button>
        </div>
        </div>
        
      </div>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: "App",
  components: {
    // HelloWorld
  },
};
</script>

<style>
body {
  margin: 0;
  padding: 0;
  background-image: url("https://images.unsplash.com/photo-1589691962030-8d2b7f2a1ffe?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80");
  background-repeat: no-repeat;
  background-size: cover;
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: "Arvo", serif;
  font-family: "Lato", sans-serif;
  /* font-family: "Potta One", cursive; */
  font-size: 14px;
  user-select: none;
}
.main {
  display: flex;
  justify-content: center;
  align-items: center;
}
.container {
  color: white;
  border-radius: 30px;
  width: 1000px;
  height: 600px;
  background-color: rgba(255, 255, 255, 0.228);
  display: flex;
  flex-direction: column;
  /* justify-content: center; */
  /* align-items: center; */
  backdrop-filter: blur(15px);
  padding: 20px;
  background: linear-gradient(
    109.41deg,
    rgba(255, 255, 255, 0.2) 0%,
    rgba(255, 254, 254, 0.15) 100%
  );
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  backdrop-filter: blur(50px);
  /* Note: backdrop-filter has minimal browser support */
    box-shadow: 0px 0px 30px rgb(255, 255, 255);
}

.nav {
  padding: 5px 1px;
  border-radius: 30px;
  /* background-color: rgba(255, 255, 255, 0.239); */
  display: flex;
  justify-content: space-around;
  flex-direction: row;
  align-items: center;
}

.logo {
  font-size: 2rem;
  font-weight: 900;
  color: rgb(255, 255, 255);
}
.navlinks router-link {
  font-size: 1.5rem;
  padding: 10px;
}
.content {
  border-radius: 30px;
  margin-top: 20px;
  width: 100%;
  height: 500px;
  display: flex;
  justify-content: space-around;
  align-items: center;
  flex-direction: row;
}
.content .left {
  display: flex;
  justify-content: center;
  align-items: center;
  /* overflow: hidden; */
  /* border-radius: 50%; */
}
.left img {
  margin: 8rem;
  width: 10rem;
  height: 10rem;
  object-fit: cover;
  border-radius: 50%;
  transform: scale(2.0);
  /* border: 10px solid rgb(66, 56, 89); */
  box-shadow: 0px 0px 30px rgb(255, 255, 255);
  /* filter: grayscale(1); */
}
.content .right {

    display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: column;
  font-size: 2.7rem;
}

.right .heading{
    margin: 2rem 3rem;
}

#btn{
  cursor: pointer;
  color: white;
  margin-bottom: 3rem;
  font-size: 1.2rem;
  font-weight: 600;
  outline: none;
  border: none;
  background: none;
  padding: 15px 25px;
  box-shadow: 0px 0px 20px rgb(255, 255, 255);
  border-radius: 1rem;
  transition: all 700ms ease;
   border: .1rem solid white;
}

#btn:hover{
    box-shadow: none;
    border: .1rem solid white;
    animation: btncolor 10000ms ease-in-out infinite;
}
@keyframes btncolor {
  0%{
  box-shadow: 0px 0px 20px #bb7af8 ;
   border: .1rem solid #9845E8 ;
   background: #9845E8 ;
  }
  20%{
     box-shadow: 0px 0px 20px #33D2FF ;
   border: .1rem solid #33D2FF ;
    background: #33D2FF ;
  }
  40%{
   box-shadow: 0px 0px 20px #DD5789  ;
   border: .1rem solid #DD5789  ;
    background: #DD5789 ;
  }
  60%{
  box-shadow: 0px 0px 20px #e84599 ;
   border: .1rem solid #e84599 ;
    background: #e84599 ;
  }
  80%{
 box-shadow: 0px 0px 20px #33ffbb ;
   border: .1rem solid #33ffbb ;
    background: #33ffbb ;
  }
  100%{
  box-shadow: 0px 0px 20px #e28d37  ;
   border: .1rem solid #e28d37  ;
    background: #e28d37 ;
  }


}
span{
  font-weight: Bold;
}

</style>
