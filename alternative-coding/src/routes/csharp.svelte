<script>
import Navbar from '$lib/navbar.svelte';
import {Tabs} from 'spaper';
import {Tab} from 'spaper';
import Prism from "$lib/prism.svelte";


let classCode = `
# Example Class
Class Car {

}`

let constructorsCode = `
# Example Class with a constructor

Class Car {

    Public Car(){

    }

}

`


</script>
<Navbar></Navbar>
<Tabs>
<div class='table'>
    <div class='row'>
        <div class='cell'> 
           
            <Tab label="Classes">
                <div class='table'>
                    <div class='row'>
                        <div class='cell'> 
              <Prism language="csharp" code="{classCode}" header=""/>
            </div>
            <div class='cell'>.
                <img src="./static/Classes.png">
            </div>
        </div>
    </div>
            <div class="col">
               
            </Tab>
            <Tab label="Constructors">
                <Prism language="csharp" code="{constructorsCode}" header=""/>
              </Tab>
              <Tab label="Fields">
                <Prism language="csharp" code="{classCode}" header=""/>
              </Tab>
              <Tab label="Getters & Setters">
                <Prism language="csharp" code="{classCode}" header=""/>
              </Tab>
            <Tab label="Variables">
              B: Doggo ipsum very hand that feed shibe fluffer
              tungg boofers shooberino you are doin me a concern...
            </Tab>
            <Tab label="Operators">
              C: Doggo ipsum long doggo long woofer heckin you
              are doing me the shock boof maximum borkdrive...
            </Tab>
        </div>
    </div>
</div>
        <div class="col">
           
        </div>
    

    </Tabs>


<style>
* {
    box-sizing:border-box;
}
html, body {
    width:100%;
    height:100%;
    overflow:hidden;
    position:fixed;
    margin:0;
    padding:0;
}
.table {
    display:table;
    width:100%;
    height:100%;
    table-layout:fixed;
}
.row {
    display:table-row;
}
.cell {
    display:table-cell;
    border:1px solid grey;
}
.header {
    display:table-header-group;
    border:1px solid grey;
}
img{
    border-color: transparent;
    max-width: 80%;
    max-height: 80%;
    margin-left: 10%;
}
</style>