<script>
    import serverImage from '../../assets/data-server.png';
    import Service from './service.svelte';
</script>
<div class="flex-col space-y-30">
    <div class="flex">
	<h1 class="pt-40 pl-10 pr-60 leading-snug text-5xl font-bold">Reliable Web Hosting Platform for Your Website</h1>
	<img class="" src={serverImage} alt="">
    </div>
    <div class="flex justify-center">
	<Service title="Web Hosting" description="Host your own website and email without the worry of DDoS"/>
	<Service title="Discord Bot Hosting" description="Host your own custom coded Discord bot, with basic Linux command."/>
	<Service title="Minecraft server" description="Play with your friends anywhere, whether on mobile or PC!"/>

    </div>
</div>
