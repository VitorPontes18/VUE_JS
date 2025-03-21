<template>
<header>
  <div class="container">
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

  </div>
   
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
      <section class="hero">
        <div class="container">
          <div class="shape"></div>
        <div id="cta">
          <h1 class="title">
            O Sabor vai até 
            <span>você</span>

          </h1>

          <P class="description">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
          </P>


          <div id="cta_buttons">
            <a href="#" class="btn-default">
              Ver Cardapio
            </a>

            <a href="tel:+40028922" id="phone_button">
              <Button class="btn-default">
                <i class="fa-solid fa-phone"></i>
              </Button>
              (11) 40028922
            </a>
          </div>

          <div class="social-buttons">
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

        <div class="banner">
            <img src="img/hero.png" alt="">
        </div>

        </div>
        
      </section>

      <section id="sesc">
        <h2 class="sesc-title">Cardápior</h2>
        <div class="Sesc-sub">Nossos pratos especiais</div>

        <div class="pratos">

          <div class="dish">
            <div class="dish_heart">
              <i class="fa-solid fa-heart"></i>
            </div>

            <img src="img/ramen.png" class="dish-heart" alt="">

            <h3 class="dish-title">
              Ramen de misso/shoyu
            </h3>

            <span class="dish-description">
              Deliciosa sopa japonesa com caldo rico e aromático, macarrão artesanal, fatias suculentas de carne
            </span>

            <div class="dish-rate">
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <span>(500+)</span>
            </div>

            <div class="dish-price">
              <h4 class="">R$40,00</h4>
              <button class="btn-default">
                <i class="fa-solid fa-basket-shopping"></i>
              </button>
            </div>
          </div>

          <div class="dish">
            <div class="dish_heart">
              <i class="fa-solid fa-heart"></i>
            </div>

            <img src="img/macarrão.png" class="dish-heart" alt="">

            <h3 class="dish-title">
              Macarrão a moda Italiana
            </h3>

            <span class="dish-description">
              O macarrão um prato tradicional da culinária italiana, feito com massa cozida e acompanhado por diversos molhos.
            </span>

            <div class="dish-rate">
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <span>(350+)</span>
            </div>

            <div class="dish-price">
              <h4 class="">R$25,00</h4>
              <button class="btn-default">
                <i class="fa-solid fa-basket-shopping"></i>
              </button>
            </div>
          </div>

          <div class="dish">
            <div class="dish_heart">
              <i class="fa-solid fa-heart"></i>
            </div>

            <img src="img/churrasco.png" class="dish-heart" alt="">

            <h3 class="dish-title">
              Prato de Churrasco
            </h3>

            <span class="dish-description">
              O churrasco é um prato tradicional que consiste em carnes assadas na grelha ou espeto
            </span>

            <div class="dish-rate">
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <span>(400+)</span>
            </div>

            <div class="dish-price">
              <h4 class="">R$50,00</h4>
              <button class="btn-default">
                <i class="fa-solid fa-basket-shopping"></i>
              </button>
            </div>
          </div>

          <div class="dish">
            <div class="dish_heart">
              <i class="fa-solid fa-heart"></i>
            </div>

            <img src="images.jpg" class="dish-heart" alt="">

            <h3 class="dish-title">
              Esrogonofe de Carne
            </h3>

            <span class="dish-description">
              O estrogonofe de carne é um prato de origem russa que se tornou muito popular no Brasil. 
            </span>

            <div class="dish-rate">
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <div class="fa-solid fa-star"></div>
              <span>(550+)</span>
            </div>

            <div class="dish-price">
              <h4 class="">R$40,00</h4>
              <button class="btn-default">
                <i class="fa-solid fa-basket-shopping"></i>
              </button>
            </div>
          </div>
        </div>
      </section>

      <section id="testimoials">
        <img src="/chef.png" class="test-chef">

        <div id="test_cont">
          <h3 class="secs_title">
            Depoimentos
          </h3>
          <h2 class="secs_sebt">
            O que os clientes falam sobre nós
          </h2>

          <div id="feedbacks">
            <div class="feedbacks">
              <img src="/avatar.png" class="feed-avatar" alt="">

              <div class="feedback-cont">
              <p> <strong>Luzinete</strong> 
                <span>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                </span>
              </p> 
              <p>
                  "Pratos Deliciosos e bem feitos, um otimo atendimento e entrega.
              </p>

              </div>
            </div>
          </div>
        
        
          <div id="feedbacks">
            <div class="feedbacks">
              <img src="/avatar.png" class="feed-avatar" alt="">

              <div class="feedback-cont">
              <p> <strong>Maria</strong> 
                <span>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                  <i class="fa-solid fa-star"></i>
                </span>
              </p> 
              <p>
                  "Pratos Deliciosos e bem feitos, um otimo atendimento e entrega.
              </p>

              </div>
            </div>
          </div>
          
          <button class="btn-default">
            ver mais Avaliaçoes
          </button>
              
        </div>
      </section>
   </main>

   <footer>
    <img src="img/wave.svg" alt="">

    <div id="footer_itens">
      <span id="copyright">
          2025 &copy; Vitor Daniel Pontes
      </span>

      <div class="social-buttons">
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
   </footer>

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

<style src="./scss/style.scss" lang="scss"/>
 


