<script>
    import 'iconify-icon';
    import { theme } from '../stores/theme.js';

    let logo = `<li class="w-1/3"><iconify-icon icon="streamline-cyber-color:cloud-flash" width="64" height="64"></iconify-icon></li>`;
    let buttonStyle = "px-4 py-2 rounded hover:bg-blue-700";
    let darkMode = `<li><iconify-icon icon="material-symbols:dark-mode-rounded" width="32" height="32"></iconify-icon></li>`;
    let lightMode = `<li><iconify-icon icon="material-symbols:light-mode-rounded" width="32" height="32"></iconify-icon></li>`
    let currentTheme = darkMode;

    function changeTheme(){
	if (currentTheme == darkMode) {
	    currentTheme = lightMode;
	    theme.set("text-black bg-white h-screen");
    	
	} else {

	    currentTheme = darkMode;
	    theme.set("text-white bg-stone-900 h-screen");
	}
    }


</script>
    
<div class="flex px-12 py-6">
    {@html logo} 
    <ul class="flex w-1/3">
	<li><button class={buttonStyle}>Services</button></li>
	<li><button class={buttonStyle}>Discord</button></li>
	<li><button class={buttonStyle}>Contact</button></li>
	<li><button class={buttonStyle}>About</button></li>
    </ul>
    <ul class="flex w-1/3 justify-end gap-5 items-center">
	<button onclick={changeTheme}>{@html currentTheme}</button>
	<li><button class={buttonStyle}>Login</button></li>
    </ul>
</div>
