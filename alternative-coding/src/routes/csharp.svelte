<script>
import Navbar from '$lib/navbar.svelte';
import {Tabs} from 'spaper';
import {Tab} from 'spaper';
import Prism from "$lib/prism.svelte";


let code_sample = `
# Example Class
Class Car {

}`


</script>
    
<Navbar></Navbar>
<div>


<Tabs>
    <Tab label="Classes">
      <Prism language="csharp" code="{code_sample}" header=""/>
    </Tab>
    <Tab label="Constructors">
        <Prism language="csharp" code="{code_sample}" header=""/>
      </Tab>
      <Tab label="Fields">
        <Prism language="csharp" code="{code_sample}" header=""/>
      </Tab>
      <Tab label="Getters & Setters">
        <Prism language="csharp" code="{code_sample}" header=""/>
      </Tab>
    <Tab label="Variables">
      B: Doggo ipsum very hand that feed shibe fluffer
      tungg boofers shooberino you are doin me a concern...
    </Tab>
    <Tab label="Operators">
      C: Doggo ipsum long doggo long woofer heckin you
      are doing me the shock boof maximum borkdrive...
    </Tab>
  </Tabs>
</div>


<style>
.center{
position: fixed;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);
}
</style>