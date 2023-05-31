<script>
    let name = '';
    let tasks = [];


    function addTask() {
        tasks = [{todo:name, done:false},...tasks];
    }
    function linethrough() {
        textdecoration = line-through;
    }
    //function playSound(audioName) {
        //let audio = new Audio(audioName);
        //audio.loop = true;
        //audio.play();
    //}
    //playSound("fortnite-dance.mp3")
</script>

<div class = "background">
    <h1>To-Do-Tren</h1>

    <input type="text" class="item-description" placeholder="dagens Uppgifter" bind:value={name}>
    <button on:click={addTask}>
        Lägg till uppgift
    </button>
    <audio controls autoplay>
        <source src="FORTNITE DEFAULT DANCE BASS BOOSTED.wav">
    </audio>
    <fieldset>
        {#each tasks as task}

            <label class:container={task.done}  ><input type="checkbox" class="item-completed" bind:checked={task.done} on:click={linethrough} />{task.todo }</label>
        {/each}
    </fieldset>
</div>

<style>
button {
    background-color: purple;
    border: 4px;
    border-color: greenyellow;
}



.background{
    width: 60vw;
    height: 100vh;
    margin: 0;
    background-repeat: no-repeat;
    background-size: 100vw 100vh;
    background-image: url(https://media.tenor.com/5VmCkmnx7rQAAAAC/fortnite-default-skin.gif);

}
input {
    background-color: green;
    color: white;
    border: 4px solid; 
    border-color:  purple;
}
h1 {
    color: white;
}
::placeholder {
    color: white;
}
.container {
  display: block;
  font-size: 25px;;
  color: white;
  text-decoration: line-through;
  padding: 0;
  margin: 0px;
}
.item-completed:checked + .item-description {
    background: #dddddd;
    text-decoration: line-through;
}



</style>

<!--göra så det stryks över om man trycker en gång-->
<!--göra så det försvinner om man trycker två gånger-->
