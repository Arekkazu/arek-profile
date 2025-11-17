<script lang="ts">
	import '@sakun/system.css';
	import '../app.css';
	import { SiGithub, SiTwitch, SiYoutube, SiTiktok, SiRust, SiJavascript, SiTypescript, SiPython, SiExpress, SiReact, SiSvelte, SiFlask } from '@icons-pack/svelte-simple-icons';
	
  let { children } = $props();
</script>

<svelte:head></svelte:head>
<div class="flex justify-center">
	<div class="window mx-auto w-10/12">
		<div class="title-bar">
			<button aria-label="Close" class="close"></button>
			<button aria-label="Resize" class="resize"></button>
		</div>
		<div class="separator"></div>

		<div class="window-pane">
			<ul role="menu-bar" class="flex justify-center gap-4 md:gap-10">
				<li role="menu-item" tabindex="0" aria-haspopup="false">
					<a href="https://profile.arekkazu.top/"> Inicio</a>
				</li>
				<li role="menu-item" tabindex="0" aria-haspopup="false">
					<a href="https://arekkazu.top/">Apuntes</a>
				</li>
				<li class="hidden w-full justify-center md:flex">
					<img src="/images/layout/penguin.gif" class="ml-18 w-8" alt="Penguin Dance" />
				</li>
				<li role="menu-item" tabindex="0" aria-haspopup="false">
					<a target="_blank" href="https://github.com/arekkazu">Proyectos</a>
				</li>

				<!-- SOCIAL MEDIA ICONS -->
				<li tabindex="0" aria-haspopup="false" class="hidden md:block">
					<div class="flex gap-2 mt-2">
						<a target="_blank" href="https://github.com/arekkazu">
							<SiGithub />
						</a>

						<a target="_blank" href="https://www.twitch.tv/arekkazu">
							<SiTwitch color={'purple'} />
						</a>
						<a target="_blank" href="https://www.youtube.com/@arekkazu">
							<SiYoutube color={'red'} />
						</a>
            
						<a target="_blank" href="https://www.tiktok.com/@arekkazu">
							<SiTiktok />
						</a>
					</div>
				</li>
				<!------------------------------->
			</ul>
		</div>
	</div>
</div>

{@render children()}
