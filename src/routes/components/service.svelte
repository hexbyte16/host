<script>
    import 'iconify-icon';
    let { title, description } = $props();
</script>

<div class="rounded-xl space-y-3 m-5 py-5 px-10 bg-[#24242F] hover:bg-blue-700">
    <h1 class="font-bold">{title}</h1>
    <p>{description}</p>
    <iconify-icon icon="emojione-monotone:right-arrow" width="45" height="45"></iconify-icon>


</div>



