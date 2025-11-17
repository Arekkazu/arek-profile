<script>
	import {
		SiRust,
		SiJavascript,
		SiTypescript,
		SiPython,
		SiReact,
		SiSvelte,
		SiFlask,
		SiExpress,
		SiLinux,
		SiGnubash
	} from '@icons-pack/svelte-simple-icons';
	const skills = [
		{ name: 'Rust', icon: SiRust, color: '#DEA584' },
		{ name: 'JavaScript', icon: SiJavascript, color: '#F7DF1E' },
		{ name: 'TypeScript', icon: SiTypescript, color: '#3178C6' },
		{ name: 'Python', icon: SiPython, color: '#3776AB' },
		{ name: 'Express', icon: SiExpress, color: '#000000' },
		{ name: 'React', icon: SiReact, color: '#61DAFB' },
		{ name: 'Svelte', icon: SiSvelte, color: '#FF3E00' },
		{ name: 'Flask', icon: SiFlask, color: '#000000' },
		{ name: 'Linux', icon: SiLinux, color: '#000000' },
		{ name: 'Bash', icon: SiGnubash, color: '#000000' }
	];

	$inspect(skills);
</script>

<div class="grid justify-center">
	<img class=" mt-20 h-60 w-60 rounded-full bg-black/45" src="/images/arekkazu.png" alt="Avatar" />

	<h2 class="title text-center">Arekkazu :D</h2>
</div>

<div class="mx-auto mt-10 mb-10 grid w-11/12 grid-cols-1 gap-4 md:w-2/3 md:grid-cols-2">
	<div class="standard-dialog center scale-down">
		<div class="title-bar">
			<button aria-label="Close" class="close"></button>
			<h1 class="title">Sobre mi</h1>
			<button aria-label="Resize" class="resize"></button>
		</div>
		<p class="mt-4 text-lg">
			Soy Alexander, también conocido como Arekkazu, estudiante de ingeniería de software y
			apasionado por la programación, especialmente en el área de Backend. Aun así, no me limito a
			una sola especialidad: me interesa entender cómo funcionan las demás áreas y cómo se aplican
			dentro del desarrollo moderno.
		</p>

		<p class="mt-4 text-lg">
			Cuando construyo software, busco que sea pulido, eficiente y fácil de mantener. Para mí, la
			ingeniería no es solo resolver un problema, sino comprender por qué la solución es la adecuada
			y cómo puede evolucionar.
		</p>
	</div>

	<div class="standard-dialog center scale-down">
		<div class="title-bar">
			<button aria-label="Close" class="close"></button>
			<h1 class="title">Tecnologias que uso</h1>
			<button aria-label="Resize" class="resize"></button>
		</div>
		<div class="mt-4 flex flex-wrap gap-3">
			{#each skills as skill}
				<div class="flex items-center gap-2 rounded-md bg-slate-800/60 px-2 py-1">
					<skill.icon color={skill.color} />
					<span class="text-sm text-black">{skill.name}</span>
				</div>
			{/each}
		</div>
	</div>
</div>
