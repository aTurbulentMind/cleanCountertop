<div class="nav">
<nav>
	<ul sveltekit:prefetch class="menu">
		<li>
			<a  href="/">Home</a>
		</li>
		<li>
			<a href="/menu">Menu</a>
		</li>
		<li>
			<a href="/events">Events</a>
		</li>
		<li>
			<a href="/contact">Contact</a>
		</li>
		<li>
			<a href="tel:+13603778516">Call now!</a>
		</li>
		
	</ul>
</nav> <p>Menu</p>
</div>

<style lang="scss">

	@import 'vari';
	
	@mixin nav() {
    position: fixed;
    bottom: -80px;
    right: 0;
    transform: translateY(-30%);
    z-index: 4;
    font-weight: bold;
	
    .menu {
      transform: scale(0);
      transition: transform 0.4s 0.02s;
    }

    &:hover .menu {
  transition: transform 0.4s 0.04s, z-index 0s 0.2s;
  transform: scale(1);
}

	p {
	margin-left: 50px;
	background: rgba( 56, 229, 42, 0.15 );
	box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
	backdrop-filter: blur( 3.5px );
	-webkit-backdrop-filter: blur( 3.5px );
	border-radius: 10px;
	border: 1px solid rgba( 255, 255, 255, 0.18 );
	color:$textColorMain ;
	text-shadow: 2px 2px 8px $backgroundMain;
	text-align: center;
	}

    li {
        list-style: none;

        a {
            display: block;
            text-decoration: none;
            text-shadow: none;
            background: rgba( 56, 229, 42, 0.15 );
			box-shadow: 0 8px 32px 0 rgba( 31, 38, 135, 0.37 );
			backdrop-filter: blur( 3.5px );
			-webkit-backdrop-filter: blur( 3.5px );
			border-radius: 10px;
			border: 1px solid rgba( 255, 255, 255, 0.18 );
            	color:$textColorMain ;
            height: 30px;
            line-height: 30px;
            font-size: 2vmax;
            width: 10vmax;
            margin: 3px 0;
            padding:0 15px;
            

            &:hover {
                transition: 0.2s;
                background: $clover;
                color: $backgroundMain;
				box-shadow:5px 0px 25px #ffffbd73;
            }
        }
    }

}



.nav {

    @include nav();

	


}

p {
	margin-left: 4%;
	
	a{
		text-decoration: none;
		color: $textColorMain;
	}
	
}
	
	//
	//ul {
	//	display: flex;
	//	list-style: none;
	//	margin: 0;
	//	font-size: 2vw;
	//	padding: 0 35%;
	//	align-items: right;
	//	
	//	li {
	//	margin:0 7px;
	//	border-style: none solid solid solid;
	//	border-color:rgb(255, 255, 244);
  	//	border-width: 2px;
	//	border-radius:0 0 5px 5px;
	//	letter-spacing: 0.1vw;
	//	padding: 0 4px;
	//	
	//	&:hover{
	//		background-color:#39993b09;
	//		transition: 0.3sec;
	//		box-shadow:11px 12px 100px #39993b7a;
	//	}
	//		
	//	a{
	//		color: #39993A;
	//		text-decoration: none;
	//		background-color: transparent;
	//		&:hover{
	//			transition: 0.3sec;
	//			color: rgb(208, 231, 78);
	//		}
	//	}
	//}
	//}


</style>
