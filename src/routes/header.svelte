<script>
	import HomeImg from './images/home.png';
	import AboutImg from './images/about.png';
	import ServicesImg from './images/services.png';
	import ContactImg from './images/contact.png';
</script>

<div id="header">
	<a href="#home">HOME</a>
	<a href="#about">ABOUT ME</a>
	<a href="#services">SERVICES</a>
	<a href="#contact">CONTACT ME</a>
</div>

<div id="mobHead">
	<a href="#home"><img src={HomeImg} alt="Home" /></a>
	<a href="#about"><img src={AboutImg} alt="About me" /></a>
	<a href="#services"><img src={ServicesImg} alt="Facilities" /> </a>
	<a href="#contact"><img src={ContactImg} alt="Contact Me" /></a>
</div>
``

<style>
	@media only screen and (max-width: 50000px) {
		#mobHead {
			display: none;
		}
		#header {
			display: none;
		}
	}
	@media only screen and (max-width: 3000px) {
		img {
			user-select: none;
			-webkit-user-drag: none;
			-moz-user-select: none;
			-webkit-user-select: none;
		}

		*::selection {
			background-color: #ffffff;
			color: rgb(0, 0, 0);
		}

		#mobHead {
			display: none;
		}

		#header {
			width: 100%;
			height: 70px;
			display: flex;
			align-items: center;
			justify-content: space-evenly;
			background-color: #8348f8;
			position: sticky;
			top: 0
		}

		#header > a {
			text-decoration: none;
			color: white;
			font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
				Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
			font-weight: 500;
			font-size: 30px;
		}
	}

	@media only screen and (max-width: 1800px) {
		#header {
			height: 60px;
		}
		#header > a {
			font-size: 25px;
		}
	}

	@media only screen and (max-width: 1100px) {
		#header {
			height: 50px;
		}
		#header > a {
			font-size: 20px;
		}
	}

	@media only screen and (max-width: 600px) {
		#header {
			display: none;
		}

		#mobHead {
			width: 100%;
			height: 45px;
			display: flex;
			align-items: center;
			justify-content: space-evenly;
			background-color: #8348f8;
			position: fixed;
		}

		#mobHead > a {
			width: 35px;
			height: 35px;
		}

		#mobHead > a > img {
			width: 100%;
		}
	}

	@media only screen and (max-width: 275px) {
		#mobHead {
			display: none;
		}
	}
</style>
