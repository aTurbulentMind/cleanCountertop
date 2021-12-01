<div class="art-banner" id="art-banner">
  <div class="art-banner-bg"></div>
  <div class="banner-text">Hello there.</div>
  <div class="badge">
    <p><a href="/">Call!</a></p>
  </div>

  <div class="banner-test">"Kind words Lorem ipsum dolor sit amet, consectetur adipisicing elit." name here</div>
  <div class="banner-test2">"Other words Lorem ipsum dolor sit, amet consectetur adipisicing elit. Numquam, perferendis doloremque? " name here</div>
</div>



<div class="box">

    <h1 class="title">Hello friend.</h1>
    <p class="words">Lorem ipsum dolor sit amet consectetur adipisicing elit. Labore, harum.</p>
    <h2>Other words</h2>
    <p>words and stuff Lorem, ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit sint modi beatae dolor ea officia est aliquam. Cum ullam et ipsam vel. Illum dignissimos veniam odit aspernatur ipsa, qui iste amet praesentium ipsam quaerat animi atque dolores? Aut, sapiente dicta.</p>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error sit sed facere tempora autem, delectus velit sint nesciunt cupiditate. Facere ratione consequatur vel nobis ea quos laboriosam totam?</p>

    <img src="/src/assets/img/tealish2.jpg" alt="">
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit ex ratione, cupiditate earum dolorum reiciendis at inventore. Non modi suscipit earum voluptate! Quam consectetur, a quae delectus soluta accusantium assumenda blanditiis culpa, unde tempora amet.</p>

    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Reprehenderit ex ratione, cupiditate earum dolorum reiciendis at inventore. Non modi suscipit earum voluptate! Quam consectetur, a quae delectus soluta accusantium assumenda blanditiis culpa, unde tempora amet.</p>
</div>


<style lang="scss">
    @import 'components';


    .art-banner {
    background-image: url(/src/assets/img/20211031_105645.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    height: 100vh;
    display: grid;
    grid-template-columns: 20px 1fr 1fr 1fr 20px;
    grid-template-rows: 20px 1fr 1fr 1fr 20px;
    
}

.art-banner-bg {
    opacity: 0.15;
    background: rgba(104, 20, 199, 0.425);
    background-size: cover;
    grid-column: 1 / -1;
    grid-row: 1 / -1;
}

.banner-text {
    color: $backgroundMain;
    font-size: 10vw;
    font-weight: bold;
    grid-column: 2 / span 2;
    grid-row: 2 /* no need to type one*/;
    align-self: center;
    justify-self: center;
}

.badge {
    display: grid;
    align-self: center;
    justify-self: center;
    grid-column: 4 / 5;
    grid-row: 1 / 4;
    background-color: $highlight;
    color: $backgroundMain;
    font-size: 3.6vw;
    font-weight: 700;
    width: 15vw;
    height: 10vw;
    border-radius: 50%;
    transform: rotate(15deg);

p {
    margin:auto;
    transform: scale(1.2);
}

a {
    color: $textColorMain;
    text-decoration: none;

    &:hover {
        text-decoration: underline;
        
    }
}
}

.banner-test {
    @include greenBack();
    color: $backgroundMain;
    font-size: 2.8vh;
    font-weight: bold;
    grid-column: 2 / span 2;
    grid-row: 3 /* no need to type one*/;
    align-self: center;
    justify-self: center;
    width: fit-content;
}

.banner-test2 {
    @include greenBack();
    color: $backgroundMain;
    font-size: 2.8vh;
    font-weight: bold;
    grid-column: 3 / span 2;
    grid-row: 4 /* no need to type one*/;
    align-self: center;
    justify-self: center;
}

.art-banner::before {
    content: "";
    opacity: 0.85;
    border-top: 5px solid $backgroundMain;
    border-right: 5px solid $backgroundMain;
    grid-column: 4;
    grid-row: 2 / span 3;
}

.art-banner::after {
    content: "";
    opacity: 0.85;
    border-bottom: 5px solid $backgroundMain;
    border-left: 5px solid $backgroundMain;
    grid-column: 2;
    grid-row: 4;
}

    .entry {
    
        
        img {
            width: 100%;
            height: 70%;
        }
    }

    .box {
        background: $backgroundMain;

        img {
            width: 100%;
            height: 100%;
            margin: 15px;
            border-radius: 5px;
        }
    }

    .title {
        color:$textColorMain;

        
    }

    .words {
            color:$textColorMain;
        }

</style>