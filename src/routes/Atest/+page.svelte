<script>
    function gotoquiz(){
        if(document.getElementById("c1").checked)
            location.href='./Aquiz'
        else
            alert("Hur lyckas du ha fel på första frågan, otroligt pinsamt! Eftersom du hade fel är du skydig mig en swish på 10kr (070-765-25-79)")
    }
</script>
<div class="quiz-container" id="quiz">
    <div class="quiz-header">
        <h1><u>Test fråga</u></h1>
        <h2 id="question1">För att få genomföra quizet måste du först svara rätt på en testfråga. Hur många kladdkakor äter Anton under Bulkningssäsong? </h2>
        <form class="options">
            <div>
                    <input class="answer" type="radio" name="answer" id="a1">
                    <label for="a1" id="optionA1" class="optionA1">A. För många</label>
            </div>
            <div>
                    <input class="answer" type="radio" name="answer" id="b1">
                    <label for="b1" id="optionB1" class="optionB1">B. 23</label>
            </div>
            <div>
                    <input class="answer" type="radio" name="answer" id="c1">
                    <label for="c1" id="optionC1" class="optionC1">C. Inte nog många</label>
            </div>
            <div>
                    <input class="answer" type="radio" name="answer" id="D1">
                    <label for="D1" id="optionD1" class="optionD1">D. Lagom</label>
            </div>
        </form>


        <button id="submit" class="submitbuttom" on:click={gotoquiz}>Till quizet😊</button>
        <h3><u>HA IGÅNG LJUD UNDER QUIZET!!!</u></h3>
        <h4><u>Ljud PÅ!</u></h4>
    </div>
</div>


<style>
h1 {
    text-align: center;
    color: white;
    font-family: copperplate;
    font-size: 75px;
    margin-top: 10px;
}
h2 {
    text-align: center;
    color: rgb(250, 252, 251);
    font-family: copperplate;
    font-size: 40px;
    margin-top: -70px;
}
h3 {
    font-size: 35px;
    font-family: impact;
    color:black;
    margin-left: -770px;
    margin-top: 20px;
}
h4 {
    font-size: 80px;
    font-family: impact;
    color:black;
    margin-left: 720px;
    margin-top: -340px;
}

.submitbuttom {
    width: 220px;
    text-align: center;
    border-radius: 25px;
    position: center;
    border: 5px solid black; 
    color: white; 
    background-color: rgb(25, 140, 228);
    font-size: 30px;
    font-family: copperplate;
    align-items: center;
    margin: auto;
}
.answer{
    background-color: white;
    border-color: black;
}
.optionA1 {
    color:rgb(16, 16, 164);
    font-size: 30px;
    font-family: impact;
    margin: 5px;
    margin-top: -500px;
}
.optionB1 {
    color:rgb(16, 16, 164);
    font-size: 30px;
    font-family: impact;
    margin: 5px;
}
.optionC1 {
    color:rgb(16, 16, 164);
    font-size: 30px;
    font-family: impact;
    margin: 5px;
}
.optionD1 {
    color:rgb(16, 16, 164);
    font-size: 30px;
    font-family: impact;
    margin: 5px;
}
.quiz-container {
    background-color: rgb(104, 187, 196);
    box-shadow: 0 0 15px 5px;
    width: 1200px;
    height: 650px;
    margin: auto;
}
.quiz-header{
    display: flex;
    flex-direction: column;
    align-items:center;
}
.options {
    display: flex;
    flex-direction: column;
    align-items:start;
    margin: 5px;
}
</style>