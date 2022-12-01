<script>
  import Button, { Label } from "@smui/button";
  import { goto } from "$app/navigation";
  let _mom = new Date().getFullYear();
  let _url = "https://johnapps.de";
  const goToContact = function () {
    goto("/contact");
  };
</script>

<h1 class="head">Welcome home</h1>
<div style="text-align: center; margin: 1rem">
  <Button on:click={() => goToContact()} variant="raised">
    <Label>Go</Label>
  </Button>
  <p style="margin: 1rem;">
    <a href="/contact">Go to contact</a>
  </p>
</div>

<div class="foot">
  <span>&copy</span>&nbsp;<a href={_url} target="_blank" rel="noreferrer"
    >johnapps</a
  >&nbsp; <span>{_mom}</span>
</div>

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
