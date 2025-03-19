<template>
<header>
   <nav class="navbar">
        <i class="fa-solid fa-burger navbar__logo">FOOD</i>

        <ul id="nav_list">
          <li class="nav-item">
            <a href="#home">Inicio</a>
          </li>
          <li class="nav-item">
            <a href="#menu">Cardapio</a>
          </li>
          <li class="nav-item">
            <a href="#testimonials">Avaliaçoes</a>
          </li>
        </ul>

        <button class="btn-default">
          Peça Aqui
        </button>

        <button id="mobile_btn" type="button" @click="toggleMenu">
          <i class="fa-solid fa-bars"></i>
        </button>
   </nav>
   <div class="mobile_menu" :class="{ active: isMenuActive }">

        <ul class="mobile_nav">
          <li>
            <a href="#home" class="nav_item_mobile">Inicio</a>
          </li>
          <li>
            <a href="#menu" class="nav_item_mobile">Cardápio</a>
          </li>
          <li>
            <a href="#testimonials" class="nav_item_mobile">Avaliações</a>
          </li>
        </ul>

        <button class="btn-default">
          Peça Aqui
        </button>
   </div>
   </header>

   <main id="content"> 
      <section class="home">
        <div class="shape"></div>
        <div id="cta">
          <h1 class="title">
            O Sabor vai até 
            <span>você</span>
          </h1>

          <P class="description">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quibusdam 
            veritatis ipsum error necessitatibus optio, incidunt dignissimos earum.
          </P>


          <div id="cta_buttons">
            <a href="#" class="btn-default">
              Ver Cardapio
            </a>

            <a href="tel:+40028922" id="phone_button">
              <Button class="btn-default">
                <i class="fa-solid fa-phone"></i>
                (11) 40028922
              </Button>
            </a>
          </div>

          <div class="social-media-buttons">
            <a href="">
              <i class="fa-brands fa-whatsapp"></i>
            </a>

            <a href="">
              <i class="fa-brands fa-instagram"></i>
            </a>

            <a href="">
              <i class="fa-brands fa-facebook"></i>
            </a>
          </div>
        </div>
      </section>
      <div id="banner">
      <img src="hero.png" alt="#">
    </div>phg
   </main>

</template>

  <script>
export default {
  data() {
    return {
      isMenuActive: false, 
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuActive = !this.isMenuActive;
    },
  },

};
</script>

<style lang="scss">

.poppins-thin {
  font-family: "Poppins", sans-serif;
  font-weight: 100;
  font-style: normal;
}

.poppins-extralight {
  font-family: "Poppins", sans-serif;
  font-weight: 200;
  font-style: normal;
}

.poppins-light {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  font-style: normal;
}

.poppins-regular {
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: normal;
}

.poppins-medium {
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-style: normal;
}

.poppins-semibold {
  font-family: "Poppins", sans-serif;
  font-weight: 600;
  font-style: normal;
}

.poppins-bold {
  font-family: "Poppins", sans-serif;
  font-weight: 700;
  font-style: normal;
}

.poppins-extrabold {
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: normal;
}

.poppins-black {
  font-family: "Poppins", sans-serif;
  font-weight: 900;
  font-style: normal;
}

.poppins-thin-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 100;
  font-style: italic;
}

.poppins-extralight-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 200;
  font-style: italic;
}

.poppins-light-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 300;
  font-style: italic;
}

.poppins-regular-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 400;
  font-style: italic;
}

.poppins-medium-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 500;
  font-style: italic;
}

.poppins-semibold-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 600;
  font-style: italic;
}

.poppins-bold-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 700;
  font-style: italic;
}

.poppins-extrabold-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 800;
  font-style: italic;
}

.poppins-black-italic {
  font-family: "Poppins", sans-serif;
  font-weight: 900;
  font-style: italic;
}

* {
    font-family: "Poppins", sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
  background-color: rgb(252, 244, 232);
}

section{
    padding: 28px 6%;

}

header {
  width: 100%;
  padding: 20px 8%;
}

.navbar {
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;

    &__logo{
  font-size: 24px;
  color: darkorange;
}
}

#nav_list {
  display: flex;
  list-style: none;
  gap: 48px;
}

#mobile_btn {
  display: none;
}

.mobile_menu {
  display: none;

  .nav_item_mobile {
  text-decoration: none;
  color: #1d1d1dad;
  font-weight: 600;

  &:hover{
    color:#f1dd45;
  }
}

}



.nav-item a{
  text-decoration: none;
  color: #1d1d1dad;
  font-weight: 600;
  position: relative;
  
  &::before{
    content: '';
    width: 0;
    height: 2px;
    position: absolute;
    bottom: -2px;
    left: 0;
    transition: .5s ease-in-out;
    background-color: #fac53e;
  }

  &:hover{

  &::before{
    width: 100%;

  }
  }
}

.nav-item.active a{
    color: black;
    border-bottom: 3px solid #f1f0e1;
    
}

.nav_item_mobile a{
  text-decoration: none;
  color: #1d1d1dad;
  font-weight: 600;
}



.btn-default {
  border: none;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #fac53e;
  border-radius: 12px;
  padding: 10px 14px;
  font-weight: 600;
  box-shadow: 0px 0px 10px 2px rgba(0, 0, 0, 0.1);
  cursor: pointer;
  transition: background-color .3s ease;
}

.btn-default:hover{
  background-color: #f7ddad;
}

@media screen and (max-width: 1170px){
    #nav_list,
    .navbar .btn-default {
      display:none;
    }

    #mobile_btn{
      display:block;
      border: none;
      background-color: transparent;
      font-size: 1.5rem;
      cursor: pointer;
    }

    .mobile_menu.active {
      display:flex;
      flex-direction: column;
      align-items: center;
    }

    .mobile_nav{
      display: flex;
      flex-direction: column;
      gap: 12px;
      margin: 12px 0px; 
      list-style: none;
      text-align: center;

    .nav_item_mobile {
      list-style-type: none;
      color: gray;
    }
    }
   
  }


  #cta {
  display: flex;
  min-height: 100vh - 75;
  
  }
  
</style>
