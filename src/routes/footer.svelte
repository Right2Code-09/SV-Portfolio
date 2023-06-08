<script>
	import youtubeImg from './images/youtube.webp';
	import instagramImg from './images/instagram.webp';
	import githubImg from './images/github.webp';
	import gmailImg from './images/g-mail.png';
</script>

<div id="footer">
	<div id="ftU">
		<div id="copyright">
			<h2>No © copyright issues.</h2>
			<p>Feel free to copy. If you need any help, contact me!</p>
		</div>
		<div id="social">
			<p>You can find me everywhere</p>
			<div>
				<a target="_blank" href="https://www.youtube.com/@Right2Code-09"
					><img src={youtubeImg} alt="Youtube" /></a
				>
				<a target="_blank" href="https://www.instagram.com/right_2_code"
					><img src={instagramImg} alt="Instagra," /></a
				>
				<a target="_blank" href="https://github.com/Right2Code-09"
					><img src={githubImg} alt="Github" /></a
				>
				<a target="_blank" href="mailto:right2code09@gmail.com"><img src={gmailImg} alt="Mail" /></a
				>
			</div>
		</div>
	</div>
	<p id="createdBy">
		{'</>'} and Crafted by
		<a target="_blank" href="https://github.com/Right2Code-09">Harshit Patel</a>
	</p>
	<div id="ftD">
		<p>® All Rights Reserved</p>
	</div>
</div>

<style>
	@media only screen and (max-width: 50000px) {
		#footer {
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

		#footer {
			display: flex;
			flex-direction: column;
			align-items: center;
			width: 100%;
			height: 800px;
			background-color: #000000;
		}

		#ftU {
			width: 100%;
			height: 150px;
			border-top: 5px double rgb(63, 63, 63);
			border-bottom: 5px double rgb(63, 63, 63);
			display: flex;
			align-items: center;
		}
		#ftU > div {
			width: 100%;
		}

		#copyright {
			max-width: 100%;
			height: fit-content;
			display: flex;
			flex-direction: column;
			align-items: center;
		}

		h2 {
			font-size: 25px;
			color: rgb(221, 221, 221);
			font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu,
				Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
			letter-spacing: 1px;
			margin-bottom: 0%;
		}

		#copyright > p {
			color: white;
			font-size: 20px;
			font-family: 'Amatic SC', cursive;
			letter-spacing: 1px;
			margin-top: 0%;
		}

		#social {
			width: 100%;
			height: fit-content;
			display: flex;
			flex-direction: column;
			align-items: center;
		}

		#social > p {
			color: white;
			font-size: 25px;
			font-family: 'Amatic SC', cursive;
			margin-bottom: 0%;
		}

		#social > div > a > img {
			width: 50px;
		}

		#createdBy {
			color: white;
			font-family: 'Amatic SC', cursive;
			letter-spacing: 1px;
			font-size: 20px;
		}

		#createdBy > a {
			color: #8348f8;
			text-decoration: none;
		}

		#createdBy > a:hover {
			text-decoration: underline;
		}

		#ftD {
			width: 100%;
			height: fit-content;
			margin-top: auto;
			display: flex;
			align-items: center;
			justify-content: center;
			border-top: 5px double rgb(63, 63, 63);
		}

		#ftD > p {
			color: white;
			font-family: Verdana, Geneva, Tahoma, sans-serif;
		}
	}

	@media only screen and (max-width: 800px) {
		#ftU {
			flex-direction: column;
			height: max-content;
		}

		#footer {
			height: 700px;
		}
	}

	@media only screen and (max-width: 400px) {
		#footer {
			height: 500px;
		}

		h2 {
			font-size: 22px;
		}

		#copyright > p {
			font-size: 13px;
		}

		#social > div > a > img {
			width: 40px;
		}

		#social > p {
			font-size: 20px;
		}
	}

	@media only screen and (max-width: 275px) {
		#footer {
			display: none;
		}
	}
</style>
