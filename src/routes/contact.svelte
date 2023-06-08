<script>
	import youtubeImg from './images/youtube.webp';
	import instagramImg from './images/instagram.webp';
	import stackoverflowImg from './images/stackoverflow.webp';
	import linkedinImg from './images/linkedin.webp';
	import githubImg from './images/github.webp';
	import mediumImg from './images/medium.jpeg';
	import codepenImg from './images/codepen.webp';
	import dribbbleImg from './images/dribbble.webp';
	import clickHereImg from './images/clickhere.webp';
</script>

<div id="contact">
	<div id="cntL">
		<h1>CONTACT ME</h1>
		<a href="mailto:right2code09@gmail.com">right2code09@gmail.com</a>
		<img src={clickHereImg} alt="clickIcon" />
	</div>
	<div id="cntR">
		<h2>SOCIAL</h2>
		<div class="SoIcn">
			<a target="_blank" href="https://www.youtube.com/@Right2Code-09"
				><img src={youtubeImg} alt="youtube" />
			</a>

			<a target="_blank" href="https://www.instagram.com/right_2_code"
				><img src={instagramImg} alt="instagram" />
			</a>

			<a target="_blank" href="https://github.com/Right2Code-09"
				><img src={githubImg} alt="github" />
			</a>

			<a target="_blank" href="https://stackoverflow.com/users/21973458/right-2-code"
				><img src={stackoverflowImg} alt="stackoverflow" />
			</a>
		</div>
		<div id="SoIcn2" class="SoIcn">
			<a target="_blank" href="https://www.linkedin.com/in/right-2-code-aa59a1278">
				<img src={linkedinImg} alt="linkedin" />
			</a>

			<a target="_blank" href="https://medium.com/@right2code09"
				><img src={mediumImg} alt="medium" /></a
			>
			<a target="_blank" href="https://codepen.io/Right-2-Code"
				><img src={codepenImg} alt="codepen" /></a
			>
			<a target="_blank" href="https://dribbble.com/right2code"
				><img src={dribbbleImg} alt="dribble" /></a
			>
		</div>
	</div>
</div>

<style>
	@media only screen and (max-width: 50000px) {
		#contact {
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
		#contact {
			width: 100%;
			height: max-content;
			border-top: 1px solid rgb(63, 63, 63);
			display: flex;
			scroll-margin-top: 60px;
		}

		#cntL {
			width: 50%;
			display: flex;
			flex-direction: column;
			align-items: center;
			border-right: 1px solid rgb(63, 63, 63);
		}

		#cntL > a {
			color: rgb(223, 223, 223);
			font-family: 'Amatic SC', cursive;
			font-weight: 600;
			letter-spacing: 2px;
			font-size: 50px;
			margin-top: 50px;
		}

		#cntL > a:hover {
			color: #8348f8;
			transition: 0.3s;
		}

		#cntL > img {
			width: 100px;
			margin-top: 10px;
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

		#cntR {
			width: 50%;
			display: flex;
			flex-direction: column;
			align-items: center;
			gap: 20px;
		}

		h2 {
			width: fit-content;
			height: fit-content;
			font-size: 35px;
			font-family: 'Alegreya Sans SC', sans-serif;
			letter-spacing: 2px;
			color: white;
			font-weight: 100;
			border-bottom: 5px solid #8348f8;
		}

		.SoIcn {
			width: 400px;
			height: max-content;
			border-radius: 11px;
			display: flex;
			align-items: center;
			justify-content: space-evenly;
		}

		.SoIcn > a > img {
			width: 60px;
			border-radius: 50%;
		}

		.SoIcn > a:hover {
			transform: scale(130%) rotate(360deg);
			transition: 0.3s;
		}

		#SoIcn2 > a:hover {
			transform: scale(130%) rotate(-360deg);
			transition: 0.3s;
		}

		#SoIcn2 {
			margin-bottom: 20px;
		}
	}

	@media only screen and (max-width: 1100px) {
		#cntL > a {
			font-size: 35px;
			margin-top: 10px;
		}

		.SoIcn > a > img {
			width: 50px;
		}
	}

	@media only screen and (max-width: 900px) {
		h1 {
			font-size: 30px;
		}

		h2 {
			font-size: 30px;
		}

		#cntL > a {
			font-size: 35px;
			margin-top: 10px;
		}

		#cntL > img {
			width: 50px;
		}

		#cntR {
			gap: 5px;
		}

		.SoIcn {
			width: 250px;
		}

		.SoIcn > a > img {
			width: 50px;
		}

		.SoIcn > a:hover {
			transform: none;
			transition: none;
		}

		#SoIcn2 > a:hover {
			transform: none;
			transition: none;
		}
	}

	@media only screen and (max-width: 700px) {
		#contact {
			flex-direction: column;
			align-items: center;
		}

		#cntL {
			border-right: none;
			border-bottom: 1px solid rgb(63, 63, 63);
			width: 100%;
		}
	}

	@media only screen and (max-width: 350px) {
		h1 {
			font-size: 25px;
		}

		h2 {
			font-size: 25px;
		}

		#cntL > a {
			font-size: 25px;
		}

		.SoIcn > a > img {
			width: 40px;
		}
	}

	@media only screen and (max-width: 275px) {
		#contact {
			display: none;
		}
	}
</style>
