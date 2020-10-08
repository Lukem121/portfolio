<script>
    import TransitionWrapper from '../components/TransitionWrapper.svelte';
    import Nav from '../components/Nav.svelte';
    import projects from './_projects.js';
</script>

<svelte:head>
	<title>Luke Askew - Projects</title>
</svelte:head>


<TransitionWrapper>
    <Nav />
    <div class="flex-box">
        {#each projects as project}
            <div class="card">
                <img src="{project.img}" alt="Avatar">
                <div class="container">
                    <h2><b>{project.title}</b></h2>
                    <p>{project.description}</p>
                    <div class="buttons">
                        <a href="{project.demo}">Demo</a>
                        <a href="{project.code}">Code</a>
                    </div>
                </div>
            </div>
        {/each}
    </div>
</TransitionWrapper>

<style>
    .flex-box {
        display: flex;
        flex-wrap: wrap;
		align-items: center;
		justify-content: center;
		text-align: center;
		height: 100vh;
	}
    .card {
        box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
        transition: 0.3s;
        border-radius: 5px;
        margin: 20px;
        width: 80%;
    }
    .card:hover {
        box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
    }
    .container {
        padding: 2px 16px;
    }
    img {
        width: 100%;
        border-radius: 5px 5px 0 0;
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

    @media only screen and (min-width: 600px) {
        .card {
            min-width: 245px;
            max-width: 20%;
        }
    }
</style>