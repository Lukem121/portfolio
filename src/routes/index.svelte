<script>
	import TransitionWrapper from '../components/TransitionWrapper.svelte';
</script>

<svelte:head>
	<title>Luke Askew - Welcome</title>
</svelte:head>

<TransitionWrapper>
	<div class="flex-box">
		<div class="content">
			<span>Luke <span>Askew</span></span>
			<div class="links-wrapper">
				<div class="links">
					<a href="https://www.linkedin.com/in/luke-askew/"><i
						class="fab fa-linkedin" />
						Linkedin</a>
					<a href="https://github.com/Lukem121"><i
						class="fab fa-github-square" />
						GitHub</a>
					<a href="https://www.instagram.com/lukem121/"><i
						class="fab fa-instagram-square" />
						Instagram</a>
				</div>
				<div class="buttons">
					<a href="/#">Resume</a>
					<a href="/projects">Projects</a>
				</div>
			</div>
		</div>
	</div>
</TransitionWrapper>

<style>
	.flex-box {
		display: flex;
		align-items: center;
		justify-content: center;
		text-align: center;
		height: 100vh;
	}

	.content span {
		color: #202124;
		font-size: 6.5rem;
	}
	.content span span {
		color: #4af174;
	}

	.links-wrapper {
		margin-top: -30px;
	}

	.links {
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 0 100px;
		cursor: pointer;
	}
	.buttons {
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.buttons a {
		cursor: pointer;
		padding: 0 20px;
		margin: 12px;
		border: 1px solid #d8d8d8;
		font-size: 1.5rem;
	}

	@media only screen and (max-width: 600px) {
		.content span {
			line-height: 90%;
		}
		.links-wrapper {
			margin-top: 10px;
		}
		.links {
			padding: 0 50px;
		}
	}
</style>