<script>

    function nextpage() {
        location.href='./Atest'
    }

</script>


<div class="content">
    <h1>Vilken Av Antons Personligheter Är Du!?</h1>
    <p>⬇Klicka här nedan för att starta quizet⬇</p>
    <div>
        <button on:click={nextpage} type="button" class="buttonstart">Till Quizet</button>
    </div>
</div>
<div  class="startbackground">
</div>
<img src="gustav.jpg" alt="Gustav" class="gustav">
<img src="hans.jpg" alt="hans" class="hans">
<img src="joel.jpg" alt="joel" class="joel">
<img src="helge.jpg" alt="helge" class="helge">
<h3 class="pictures_discription">🤝↑Några Inperationsrika Herrar↑🤝</h3>



<style>
.startbackground{
    width: 100vw;
    height: 100vh;
    background-size: cover;
    background-position: center;
}

.content {
    width: 100%;
    position: absolute;
    top: 30%;
    transform: translateY(-50%);
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;

}
.content h1 {
    color: black;
    font-family: copperplate;
    font-size: 82px;
    margin-top: 110px;
    margin-bottom: -40px;
}
.content p {
    color: white;
    font-size: 30px;
    margin-top: 80px;
    font-weight: 100;
    line-height: 25px;
    font-family: Impact;
}
.buttonstart{
    width: 200px;
    text-align: center;
    border-radius: 25px;
    position: center;
    border: 5px solid black; 
    color: white; 
    background-color: rgb(180, 163, 163);
    font-size: 30px;
    font-family: copperplate;
    margin-top: 30px;
}
.pictures_discription {
    font-family: Lucida Handwriting;
    color:white;
    display: flex;
    flex-direction: column;
    align-items: center;
    font-size: 70px;
}
.gustav{
    width: 320px;
    height: 320px;
    margin-top: -390px;
    margin-left: 15px;
}
.joel{
    width: 320px;
    height: 320px;
    margin-top: -390px;
    margin-left: 45px;
}
.hans{
    width: 320px;
    height: 320px;
    margin-top: -390px;
    margin-left: 45px;
}
.helge{
    width: 320px;
    height: 320px;
    margin-top: -390px;
    margin-left: 45px;
}

</style>