<h1 style="margin-top: -15px; padding-top:20px; background:none; font-size: 6vh; font-weight:100; font-style: italic;">Contact</h1>
    <br>


<body>
    


<div class="responsive-example">
  <div class="responsive-item">
      <h2>Facebook</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil doloribus magni soluta in velit neque, at explicabo ipsam ea placeat itaque consequatur deserunt officiis quam! Accusamus corporis repellendus nihil ipsa.</p>
    <a href="/">Visit</a> <br><br>
  </div>
  <div class="responsive-item">
      <h2>Phone</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil doloribus magni soluta in velit neque, at explicabo ipsam ea placeat itaque consequatur deserunt officiis quam! Accusamus corporis repellendus nihil ipsa.</p>
    <a href="/">Call</a> <br><br>
  </div>
  <div class="responsive-item">
      <h2>Email</h2>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil doloribus magni soluta in velit neque, at explicabo ipsam ea placeat itaque consequatur deserunt officiis quam! Accusamus corporis repellendus nihil ipsa.</p>
    <a href="/">Mail</a> <br><br>
  </div>
 

</div>
</body>
<style lang="scss">
 @import 'components';

 

 body {
     overflow-y: hidden;
 }
 
       
    
    .responsive-example {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 10px;
    margin: 10px;

}
    
    .responsive-item {
    @include greenBack();
     margin: 20px auto;

h2 {
     margin: 5% auto;
 }

      a {
            
            position: relative;
            padding: 10px 20px;
            margin: 20%;
            color: $textColorMain;
            text-decoration: none;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-size: 3vw;
            overflow: hidden;
            transition: 0.2s;
            -webkit-box-reflect: below 1px linear-gradient(transparent,#0003);
        }

        

        a:hover {
            background: $highlight;
            color:rgb(201, 201, 201) ;
            box-shadow: 0 0 50px $highlight;
            transition-delay: 0.2s;
        }

        a:before {
            content: '';
            position: absolute;
            top:0;
            left: 0;
            width: 10px;
            height: 10px;
            border-top: 2px solid  $textColorMain;
            border-left: 2px solid  $textColorMain;
            transition: 0.1s;
            transition-delay: 0.2s;
        }

        a:hover:before {
            width: 100%;
            height: 100%;
            border-top: 2px solid rgb(201, 201, 201) ;
            border-left: 2px solid rgb(201, 201, 201) ;
            transition-delay: 0.5;
        }

        a:after {
            content: '';
            position: absolute;
            bottom:0;
            right: 0;
            width: 10px;
            height: 10px;
            border-bottom: 2px solid  $textColorMain;
            border-right: 2px solid  $textColorMain;
            transition: 0.2s;
            transition-delay: 0;
        }

        a:hover:after {
            width: 100%;
            height: 100%;
            border-bottom: 2px solid rgb(201, 201, 201) ;
            border-right: 2px solid rgb(201, 201, 201) ;
            transition-delay: 0.2s;
        }

    }

</style>