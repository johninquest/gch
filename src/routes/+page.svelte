<!-- <h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p> -->
<h1 class="head">Welcome home</h1>

<div class="foot"><span>&copy</span>&nbsp;<a href={_url} target="_blank" rel="noreferrer">John Apps</a>&nbsp;{_mom}</div>

<script>
    let _mom = new Date().getFullYear();
    let _url = 'https://johnapps.de';
</script>

<style>
    .head {
        text-align: center; 
        margin-top: 6rem; 
        color: blue;
    }

    .foot {
        text-align: center;
        font-weight: bold;
        margin: 3rem auto 1rem auto;
        color: teal;
    }
    a {text-decoration: none; color: teal;}
</style>