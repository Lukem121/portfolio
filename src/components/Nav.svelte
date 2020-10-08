<div class="flex-box">
    <a href="/"><span>Luke <span>Askew</span></span></a>
</div>

<style>
    .flex-box {
		display: none;
	}
    span {
		color: #202124;
		font-size: 3.5rem;
	}
	span span {
		color: #4af174;
	}
    @media only screen and (max-width: 600px) {
        .flex-box {
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            margin-top: 20px;
            cursor: pointer;
        }
		span {
			line-height: 90%;
		}
	}
</style>