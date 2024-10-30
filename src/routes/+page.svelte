<main class="m-auto ">
	<div class="scene relative grid h-svh grid-cols-1 grid-rows-1">
		<img alt="bg" class=" camera-focus bg h-[70%]" src="Background.png" />
		<img alt="tree right" class="tree-r right-[-25%] top-[-18%]" src="Layer 2.png" />
		<img alt="tree left" class="tree-l left-[-6%] top-[0%]" src="Layer 2 copy.png" />
		<img alt="text" class=" floating-text top-[70%]" src="House Starks.png" />
		<img alt="date" class="floating-text top-[84%] left-[20%]" src="02.10.2024.png" />
		<img alt="text" class="floating-text top-[20%]" src="Over The Gard.png" />
	</div>
</main>

<style>
	.bg {
		background-size: cover;
		background-position: 50% 100%;
	}
	.scene {
		display: grid;
		justify-items: center;
		overflow: hidden;
	}

	img {
		border: 1px solid #00ffff00;
		position: relative;
		grid-column-start: 1;
		grid-row-start: 1;
	}

	.tree-l {
		animation: sway 33s ease-in-out infinite;
		transform-origin: bottom center;
	}

	.tree-r {
		animation: sway 23s ease-in-out infinite;
		transform-origin: bottom center;
	}

	@keyframes sway {
		0% {
			transform: rotate(0deg);
		}
		25% {
			transform: rotate(2deg);
		}
		50% {
			transform: rotate(0deg);
		}
		75% {
			transform: rotate(-2deg);
		}
		100% {
			transform: rotate(0deg);
		}
	}

	.camera-focus {
		animation: focus-drift 38s ease-in-out infinite;
	}

	@keyframes focus-drift {
		0% {
			transform: translate(0, 0);
		}
		25% {
			transform: translate(5px, -3px);
		}
		50% {
			transform: translate(-5px, 4px);
		}
		75% {
			transform: translate(3px, -2px);
		}
		100% {
			transform: translate(0, 0);
		}
	}


.floating-text {
      animation: float 13s ease-in-out infinite;
        display: inline-block;
  }

  @keyframes float {
    0% {
      transform: translateY(0);
      }
    50% {
      transform: translateY(-10px);
      }
    100% {
      transform: translateY(0);
      }
  }
</style>
