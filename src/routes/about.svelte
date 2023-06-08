<script>
	import profile2 from './images/profile2.png';
</script>

<div id="about">
	<h1>About Me</h1>
	<div id="aboutD">
		<img src={profile2} alt="ImageOfHarshit" />
		<p>
			My experience as a Web Developer and content creator is approximately 2 years. Currently, I'm
			a Front-End Developer, but I'm aspiring to become a Full-Stack Developer. 💻 Teaching others
			online for free is something I ❤️ to do. An example is YouTube. I have made 50+ projects to
			improve my skills and learn about new errors!! Stackoverflow, LinkedIn, Medium, YouTube and
			Instagram are just a few online platforms where I am found. To further gain knowledge and
			experience, I seek out new opportunities and challenges. As a result of solving other people's
			problems, I gain more experience and learn more. 🕵️‍♂️ Join me and ask me your questions. 🙋
		</p>
	</div>
</div>

<style>
	@media only screen and (max-width: 50000px) {
		#about {
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

		#about {
			width: 100%;
			height: max-content;
			border-top: 1px solid rgb(63, 63, 63);
			display: flex;
			flex-direction: column;
			align-items: center;
			gap: 50px;
			scroll-margin-top: 60px;
		}

		h1 {
			width: fit-content;
			height: fit-content;
			color: white;
			letter-spacing: 2px;
			font-family: 'Alegreya Sans SC', sans-serif;
			font-size: 48px;
			font-weight: 100;
			border-bottom: 5px solid #8348f8;
		}

		#aboutD {
			max-width: fit-content;
			height: fit-content;
			display: flex;
			align-items: center;
			gap: 50px;
		}

		#aboutD > img {
			width: 300px;
		}

		#aboutD > p {
			text-align: center;
			max-width: 800px;
			color: #ffffff;
			font-size: 25px;
			line-height: 50px;
			font-family: 'Amatic SC', cursive;
			letter-spacing: 1.2px;
			word-spacing: 3px;
		}
	}

	@media only screen and (max-width: 1200px) {
		#aboutD > p {
			max-width: 600px;
		}
	}

	@media only screen and (max-width: 1000px) {
		#aboutD {
			flex-direction: column;
		}

		#aboutD > p {
			max-width: 700px;
		}

		#aboutD > img {
			width: 275px;
		}
	}

	@media only screen and (max-width: 800px) {
		#aboutD > p {
			max-width: 550px;
		}
	}

	@media only screen and (max-width: 600px) {
		#about {
			gap: 30px;
		}

		#aboutD {
			gap: 30px;
		}

		#aboutD > p {
			max-width: 450px;
		}

		#aboutD > img {
			width: 225px;
		}
	}

	@media only screen and (max-width: 500px) {
		h1 {
			font-size: 40px;
		}

		#aboutD > p {
			max-width: 400px;
			line-height: 45px;
			font-size: 23px;
		}
	}

	@media only screen and (max-width: 400px) {
		#about {
			gap: 15px;
		}

		#aboutD {
			gap: 15px;
		}

		#aboutD > p {
			max-width: 300px;
			font-size: 21px;
			line-height: 35px;
		}
	}

	@media only screen and (max-width: 320px) {
		#aboutD > p {
			max-width: 250px;
			font-size: 18px;
			line-height: 30px;
		}
	}

	@media only screen and (max-width: 275px) {
		#about {
			display: none;
		}
	}
</style>
