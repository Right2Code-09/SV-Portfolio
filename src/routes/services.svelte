<script>
	import service1 from './images/service1.webp';
	import service2 from './images/service2.webp';
	import service3 from './images/service3.png';
</script>

<div id="services">
	<h1>SERVICES FOR YOU 👇</h1>
	<div id="facD">
		<a href="#contact">
			<img src={service1} alt="UI/UX_logo" />
			<p class="txtB">UI/UX designing.</p>
			<p class="txtS">47+ Projects.</p>
		</a>
		<a href="#contact">
			<img src={service2} alt="Front-End_logo" />
			<p class="txtB">Front-Ent Development.</p>
			<p class="txtS">25+ projects</p>
		</a>
		<a id="service3" href="#contact">
			<img src={service3} alt="social_logo" />
			<p class="txtB">Social Media Designing.</p>
			<p class="txtS">19+ Projects</p>
		</a>
	</div>
</div>

<style>
	@media only screen and (max-width: 50000px) {
		#services {
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

		#services {
			width: 100%;
			height: max-content;
			display: flex;
			flex-direction: column;
			align-items: center;
			border-top: 1px solid rgb(63, 63, 63);
			scroll-margin-top: 50px;
		}

		h1 {
			width: fit-content;
			height: fit-content;
			color: white;
			letter-spacing: 2px;
			font-family: 'Alegreya Sans SC', sans-serif;
			font-size: 40px;
			font-weight: 100;
			border-bottom: 5px solid #8348f8;
		}

		#facD {
			width: 100%;
			height: 500px;
			display: flex;
			align-items: center;
			justify-content: center;
			gap: 150px;
		}

		#facD > a {
			width: 300px;
			height: 400px;
			background-color: rgb(25, 25, 25);
			border-radius: 11px;
			display: flex;
			flex-direction: column;
			align-items: flex-start;
			justify-content: center;
			padding: 5px;
			text-decoration: none;
		}

		#facD > a:hover {
			transform: scale(103%);
			transition: 0.3s;
			-webkit-box-shadow: 11px 11px 10px -15px rgb(150, 150, 150);
			-moz-box-shadow: 11px 11px 10px -15px rgb(150, 150, 150);
			box-shadow: 11px 11px 10px -15px rgb(150, 150, 150);
		}

		#facD > a > img {
			width: 60px;
			margin-left: 15px;
		}

		.txtB {
			color: rgb(224, 224, 224);
			font-size: 30px;
			font-family: 'Amatic SC', cursive;
			letter-spacing: 2px;
			margin: 100px 0 0 20px;
		}

		.txtS {
			color: rgb(173, 173, 173);
			margin: 10px 0 0 20px;
			font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
				Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
			font-size: 15px;
		}
	}
	@media only screen and (max-width: 1300px) {
		#facD {
			gap: 60px;
		}
	}

	@media only screen and (max-width: 1100px) {
		h1 {
			font-size: 35px;
		}
		#facD {
			gap: 30px;
		}

		#facD > a {
			width: 250px;
			height: 350px;
		}
	}

	@media only screen and (max-width: 900px) {
		h1 {
			font-size: 30px;
		}

		#facD {
			height: 350px;
		}

		#facD > a {
			width: 200px;
			height: 250px;
		}

		#facD > a:hover {
			transform: none;
			box-shadow: none;
			transition: none;
		}

		.txtB {
			margin-top: 60px;
		}
	}

	@media only screen and (max-width: 750px) {
		#facD {
			height: 250px;
			gap: 15px;
		}

		#facD > a {
			width: 150px;
			height: 180px;
		}

		#facD > a > img {
			width: 50px;
		}

		.txtB {
			margin: 20px 0 0 10px;
			font-size: 25px;
		}

		.txtS {
			margin: 5px 0 0 10px;
		}
	}

	@media only screen and (max-width: 550px) {
		#facD {
			flex-direction: column;
			height: fit-content;
		}

		#facD > a {
			width: 300px;
			display: flex;
			align-items: center;
		}

		#service3 {
			margin-bottom: 10px;
		}
	}

	@media only screen and (max-width: 350px) {
		h1 {
			font-size: 22px;
		}

		#facD > a {
			width: 230px;
		}

		.txtB {
			font-size: 22px;
		}
	}

	@media only screen and (max-width: 275px) {
		#services {
			display: none;
		}
	}
</style>
