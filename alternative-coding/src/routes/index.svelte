<script>
import { Button } from 'spaper';
import Navbar from '$lib/navbar.svelte';
</script>

<Navbar></Navbar>

<div class="center">
<h1>Altocode currently supports the folowing languages:</h1>
<Button href="/csharp" size="large" type="secondary">C#</Button>
</div>

<style>
.center {
position: fixed;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
}
</style>