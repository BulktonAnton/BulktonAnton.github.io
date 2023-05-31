<script>
    function gobacktoquiz(){
        location.href='http://localhost:5173/Aquiz'
    }

let finalsound="finalsound.mp3"
let finalmusic="finalmusic.mp3"
</script>

<div class="quiz-container" id="quiz">
    <div class="quiz-header">
        <h1><u>Härligt quiz va!</u></h1>
        <h2>070-765-25-79</h2>
        <h3>↑STÖD ETT BARN SOM BEHÖVER HJÄLP!↑</h3>
        <button id="submit" class="submitbuttom" on:click={gobacktoquiz}>Tillbaka till quizet</button>
        <img src="ackliglinus.jpg" alt="Äcklig Linus" class="linus">
        <img src="criggewii.jpg" alt="Fetto" class="crigge">


        <embed src={finalsound} loop="true" autostart="true" class="finalmusic_sound" >
        <embed src={finalmusic} loop="true" autostart="true" class="finalmusic_music">

    </div>
</div>

<style>
    h1 {
        text-align: center;
        color: Black;
        font-family: Impact;
        font-size: 120px;
        margin-top: 10px;
    }
    h2 {
        text-align: center;
        color: rgb(250, 252, 251);
        font-family: copperplate;
        font-size: 100px;
        margin-top: -60px;
    }
    h3 {
        text-align: center;
        color: rgb(250, 252, 251);
        font-family: copperplate;
        font-size: 40px;
        margin-top: -40px;
        font-size: 35px;
    }
    .finalmusic_music {
    width: 1px;
      height: 1px; 
      margin-top: 1px; 
    }
    .finalmusic_sound {
        width: 1px;
      height: 1px; 
      margin-top: 1px; 
    }
    .linus {
    width: 300px;
    height: 500px; 
    margin-top: -410px; 
    margin-left: -1170px;
    }
    .crigge {
    width: 300px;
    height: 500px; 
    margin-top: -500px; 
    margin-left: 1170px;
    }
    
    .submitbuttom {
        width: 300px;
        text-align: center;
        border-radius: 25px;
        border: 5px solid black; 
        color: white; 
        background-color: rgb(25, 140, 228);
        font-size: 30px;
        font-family: copperplate;
        align-items: center;
        margin-bottom: -60px;
        margin-top: 70px;
    }

    .quiz-container {
        background-color: rgb(104, 187, 196);
        box-shadow: 0 0 15px 5px;
        width: 1500px;
        height: 650px;
        margin: auto;
    }
    .quiz-header{
        display: flex;
        flex-direction: column;
        align-items:center;
    }

    </style>