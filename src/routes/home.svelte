<script>
	import profile1 from './images/profile1.jpg';
</script>

<div id="home">
	<div id="homeU">
		<img src={profile1} alt="ImageOfHarshit" />
		<h1>Harshit Patel</h1>
		<p>Front-End Developer</p>
	</div>
	<div id="homeD">
		<p>
			Hello, I'm Harshit. My journey of coding started before 2 years, and has become my passion.
			Here, you'll discover everything about me. discover more about my journey below.
		</p>
	</div>
</div>

<style>
	@media only screen and (max-width: 50000px) {
		#home {
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
			background-color: #8348f8;
			color: white;
		}

		#home {
			width: 100%;
			height: max-content;
			display: flex;
			flex-direction: column;
			margin-top: 25px;
			scroll-margin-top: 75px;
		}

		#homeU {
			width: fit-content;
			height: fit-content;
			margin: 0 auto 0 auto;
		}

		#homeU > img {
			width: 300px;
			border-radius: 50%;
		}

		h1 {
			width: fit-content;
			height: fit-content;
			margin: 30px auto 0 auto;
			font-family: 'Satisfy', cursive;
			letter-spacing: 1.5px;
			word-spacing: 5px;
			font-size: 45px;
			font-weight: 100;
			color: white;
		}

		#homeU > p {
			padding-right: 3px;
			height: fit-content;
			width: fit-content;
			margin: -10px auto 0 auto; /* top right bottom left */
			color: rgb(255, 255, 255);
			font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
				Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
			font-weight: 100;
			font-size: 15px;
			overflow: hidden;
			border-right: 0.15em solid orange;
			white-space: nowrap;
			animation: typing 5s steps(30, end), blink-caret 0.5s step-end infinite;
		}

		/* The typing effect */
		@keyframes typing {
			from {
				width: 0;
			}
			to {
				width: 47%;
			}
		}

		/* The typewriter cursor effect */
		@keyframes blink-caret {
			from,
			to {
				border-color: transparent;
			}
			50% {
				border-color: orange;
			}
		}

		#homeD {
			max-width: 800px;
			height: fit-content;
			margin: 50px auto 0 auto; /* up-bottom, right-left*/
		}

		#homeD > p {
			text-align: center;
			line-height: 60px;
			color: white;
			font-size: 40px;
			font-weight: 100;
			font-family: 'Amatic SC', cursive;
			letter-spacing: 1px;
			word-spacing: 3px;
		}
	}

	@media only screen and (max-width: 1000px) {
		#homeU > img {
			width: 250px;
		}
	}

	@media only screen and (max-width: 800px) {
		h1 {
			font-size: 40px;
		}

		#homeD > p {
			font-size: 35px;
			max-width: 600px;
		}
	}

	@media only screen and (max-width: 600px) {
		#homeU > img {
			width: 225px;
		}

		h1 {
			font-size: 35px;
		}

		#homeU > p {
			font-size: 13px;
		}

		#homeD > p {
			font-size: 30px;
			max-width: 400px;
		}
	}

	@media only screen and (max-width: 400px) {
		#homeD > p {
			max-width: 300px;
		}
	}

	@media only screen and (max-width: 350px) {
		#homeD > p {
			font-size: 22px;
			max-width: 250px;
			line-height: 50px;
		}
	}

	@media only screen and (max-width: 275px) {
		#home {
			display: none;
		}
	}
</style>
