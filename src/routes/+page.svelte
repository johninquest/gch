<!-- <h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->
<h1 class="head">Welcome home</h1>

<div class="foot"><span>&copy</span>&nbsp;<a href={_url} target="_blank" rel="noreferrer">johnapps</a>&nbsp; <span>{_mom}</span> </div>

<script>
    let _mom = new Date().getFullYear();
    let _url = 'https://johnapps.de';
</script>

<style lang="scss">
    .head {
        text-align: center; 
        margin: 6rem auto 6rem auto; 
        color: var(--primary-color);
    }

    .foot {
        text-align: center;
        font-weight: bold;
        text-transform: uppercase;
        margin: 3rem auto 3rem auto;
        color: var(--txt-color); 
        a {
        text-decoration: none; 
        color: var(--txt-color);
        }
    }
   
</style>