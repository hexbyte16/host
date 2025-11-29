<script>
    import Home from './home.svelte'
    import { theme } from './stores/theme.js';
</script>

<div class = {$theme}>
    <Home/>

</div>

