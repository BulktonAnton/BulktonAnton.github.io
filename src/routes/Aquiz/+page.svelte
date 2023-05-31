<script>
   // Alla frågor och alternativ
let questions = [
    {
        q:"Är du aggresiv?",
        op: [
            {
               text:"A. Inte så ofta", personality: 1, choosen: false 
            },
            {
               text:"B. Ibland", personality: 2, choosen: false 
            },
            {
               text:"C. Aldig", personality: 3, choosen: false 
            },
            {
               text:"D. Alltid", personality: 4, choosen: false 
            },
            {
               text:"E. ♥Aggresivitet är fel♥", personality: 5, choosen: false 
            },
            {
               text:"F. Vet ej", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Är du dominant?",
        op: [
            {
               text:"A. 100%", personality: 1, choosen: false 
            },
            {
               text:"B. Njaaaa", personality: 2, choosen: false 
            },
            {
               text:"C. Vem vet", personality: 3, choosen: false 
            },
            {
               text:"D. Är det ens en fråga?", personality: 4, choosen: false 
            },
            {
               text:"E. Om det behövs", personality: 5, choosen: false 
            },
            {
               text:"F. Bryr mig inte", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Hur många är du vänn med?",
        op: [
            {
               text:"A. Få", personality: 1, choosen: false 
            },
            {
               text:"B. ALLA", personality: 2, choosen: false 
            },
            {
               text:"C. Dom flesta", personality: 3, choosen: false 
            },
            {
               text:"D. Inga", personality: 4, choosen: false 
            },
            {
               text:"E. 1", personality: 5, choosen: false 
            },
            {
               text:"F. Vänner är inte riktiga", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Är du diciplinerad?",
        op: [
            {
               text:"A. Till döden", personality: 1, choosen: false 
            },
            {
               text:"B. Jadu, bra fråga", personality: 2, choosen: false 
            },
            {
               text:"C. Ganska ofta", personality: 3, choosen: false 
            },
            {
               text:"D. Lista ut", personality: 4, choosen: false 
            },
            {
               text:"E. Jag tror det", personality: 5, choosen: false 
            },
            {
               text:"F. Ja...", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Är du Vacker?",
        op: [
            {
               text:"A. Vem Fuck bryr sig", personality: 1, choosen: false 
            },
            {
               text:"B. Otroligt", personality: 2, choosen: false 
            },
            {
               text:"C. Ganska", personality: 3, choosen: false 
            },
            {
               text:"D. Vackerhetism spelar ingen roll, slägga är vad som är viktigt!", personality: 4, choosen: false 
            },
            {
               text:"E. Mmmmhhhmm", personality: 5, choosen: false 
            },
            {
               text:"F. Nej.", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Vad är viktigt i Livet?",
        op: [
            {
               text:"A. Jag", personality: 1, choosen: false 
            },
            {
               text:"B. Alkohol", personality: 2, choosen: false 
            },
            {
               text:"C. Lycka och vänner", personality: 3, choosen: false 
            },
            {
               text:"D. Slägga och gym", personality: 4, choosen: false 
            },
            {
               text:"E. Kärlek", personality: 5, choosen: false 
            },
            {
               text:"F. Inget", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Hur lyckig är du?",
        op: [
            {
               text:"A. 7/10", personality: 1, choosen: false 
            },
            {
               text:"B. För lycklig", personality: 2, choosen: false 
            },
            {
               text:"C. 10/10", personality: 3, choosen: false 
            },
            {
               text:"D. Aldrig", personality: 4, choosen: false 
            },
            {
               text:"E. Självfallet", personality: 5, choosen: false 
            },
            {
               text:"F. Vad är lycka?", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Är du empatiskt?",
        op: [
            {
               text:"A. Varför skulle jag vara", personality: 1, choosen: false 
            },
            {
               text:"B. Jag är för empatiskt", personality: 2, choosen: false 
            },
            {
               text:"C. Såklart jag är", personality: 3, choosen: false 
            },
            {
               text:"D. Till vissa", personality: 4, choosen: false 
            },
            {
               text:"E. Till en person", personality: 5, choosen: false 
            },
            {
               text:"F. Jag är psykopat", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Hur ser din familjesituation ut??",
        op: [
            {
               text:"A. Ok.", personality: 1, choosen: false 
            },
            {
               text:"B. Bra, tror jag", personality: 2, choosen: false 
            },
            {
               text:"C. Den ser fantastik ut", personality: 3, choosen: false 
            },
            {
               text:"D. Filippa", personality: 4, choosen: false 
            },
            {
               text:"E. Mycket bra", personality: 5, choosen: false 
            },
            {
               text:"F. Vem behöver familj", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Vilken typ musik gillar du?",
        op: [
            {
               text:"A. Brazzilian Phonk", personality: 1, choosen: false 
            },
            {
               text:"B. All musik man blir glad av ", personality: 2, choosen: false 
            },
            {
               text:"C. Typ allt", personality: 3, choosen: false 
            },
            {
               text:"D. Brazzilian Phonk och Motiverande låtar", personality: 4, choosen: false 
            },
            {
               text:"E. Sommar Bangers", personality: 5, choosen: false 
            },
            {
               text:"F. Depprimerade musik", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Hur ser din politiska läggning ut?",
        op: [
            {
               text:"A. Höger!", personality: 1, choosen: false 
            },
            {
               text:"B. Mitten?", personality: 2, choosen: false 
            },
            {
               text:"C. Mat", personality: 3, choosen: false 
            },
            {
               text:"D. Politik är propaganda, Escape the Matrix!", personality: 4, choosen: false 
            },
            {
               text:"E. Extrem Feminist", personality: 5, choosen: false 
            },
            {
               text:"F. Diktatorismen", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Om det blev krig, vad hade du gjort?",
        op: [
            {
               text:"A. Krigat till döden", personality: 1, choosen: false 
            },
            {
               text:"B. Supit", personality: 2, choosen: false 
            },
            {
               text:"C. Hjälpt till", personality: 3, choosen: false 
            },
            {
               text:"D. Döda alla i min väg", personality: 4, choosen: false 
            },
            {
               text:"E. Blivit hippie", personality: 5, choosen: false 
            },
            {
               text:"F. En Stalin", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Har du fördommar om andra?",
        op: [
            {
               text:"A. Bryr mig inte om andra", personality: 1, choosen: false 
            },
            {
               text:"B. Absolut inte", personality: 2, choosen: false 
            },
            {
               text:"C. Tillfälle till tillfälle", personality: 3, choosen: false 
            },
            {
               text:"D. Sannorligen", personality: 4, choosen: false 
            },
            {
               text:"E. Beror på vad hon tycker", personality: 5, choosen: false 
            },
            {
               text:"F. Vem har inte det!", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Lyssnar och agerar du med dina känslor?",
        op: [
            {
               text:"A. Jag gör det jag måste göra, inte vad jag känner för att göra", personality: 1, choosen: false 
            },
            {
               text:"B. Ibland men jag har kontroll", personality: 2, choosen: false 
            },
            {
               text:"C. 40%", personality: 3, choosen: false 
            },
            {
               text:"D. Bara på agresiva sätt", personality: 4, choosen: false 
            },
            {
               text:"E. För det mesta", personality: 5, choosen: false 
            },
            {
               text:"F. Känslor är inte riktiga", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Vad är din dröm?",
        op: [
            {
               text:"A. Bli släggelit", personality: 1, choosen: false 
            },
            {
               text:"B. Unlimited alkohol", personality: 2, choosen: false 
            },
            {
               text:"C. Oändlig lycka", personality: 3, choosen: false 
            },
            {
               text:"D. Slå ner 5 pers", personality: 4, choosen: false 
            },
            {
               text:"E. Gifta mig", personality: 5, choosen: false 
            },
            {
               text:"F. Att alla dör", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Hade du överlevt en zombie acopolyctiksts?",
        op: [
            {
               text:"A. Enkelt", personality: 1, choosen: false 
            },
            {
               text:"B. Jag hade börjat köra dancebattle med en zombie, så nej", personality: 2, choosen: false 
            },
            {
               text:"C. Kanske", personality: 3, choosen: false 
            },
            {
               text:"D. Folk hade inte vart rädda för zombies, dom hade vart rädd för mig", personality: 4, choosen: false 
            },
            {
               text:"E. Bara min kärleks överlevnad är viktig", personality: 5, choosen: false 
            },
            {
               text:"F. vet ej", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Vad tycker du om killar som gråter ofta?",
        op: [
            {
               text:"A. Stör mig inte", personality: 1, choosen: false 
            },
            {
               text:"B. När min alkohol är slut gråter jag", personality: 2, choosen: false 
            },
            {
               text:"C. Jag tycker de gör rätt, jag hade försökt få dom att må bättre", personality: 3, choosen: false 
            },
            {
               text:"D. Klena", personality: 4, choosen: false 
            },
            {
               text:"E. Tycker det är fint att man visar sina känslor", personality: 5, choosen: false 
            },
            {
               text:"F. Avrättas", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Din släkt = Brooke. Lösning är du blir kriminell, hade du blivit det?",
        op: [
            {
               text:"A. 100%, allt för familjen", personality: 1, choosen: false 
            },
            {
               text:"B. Beror på", personality: 2, choosen: false 
            },
            {
               text:"C. Jag tror det", personality: 3, choosen: false 
            },
            {
               text:"D. Jag kan blir kriminell frivilligt", personality: 4, choosen: false 
            },
            {
               text:"E. Aldig, brott är fel!(alfons)", personality: 5, choosen: false 
            },
            {
               text:"F. Jag är redan kriminell", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Är det viktigt att ha vänner?",
        op: [
            {
               text:"A. Vene", personality: 1, choosen: false 
            },
            {
               text:"B. Som dricker, ja", personality: 2, choosen: false 
            },
            {
               text:"C. Såklart", personality: 3, choosen: false 
            },
            {
               text:"D. Ibland", personality: 4, choosen: false 
            },
            {
               text:"E. Vänskap är viktigt så ja", personality: 5, choosen: false 
            },
            {
               text:"F. Ja, annars sticker man ut och kan inte genomföra framtida krigsbrott", personality: 6, choosen: false 
            }
        ]
    },
    {
        q:"Vilket alternativ beskriver dig bäst??",
        op: [
            {
               text:"A. Bossig, obrydd och bäst", personality: 1, choosen: false 
            },
            {
               text:"B. Alkolist", personality: 2, choosen: false 
            },
            {
               text:"C. Glad, rolig, positiv och en bra vän", personality: 3, choosen: false 
            },
            {
               text:"D. Arg och agressiv", personality: 4, choosen: false 
            },
            {
               text:"E. Snäll, simp, oskyldig och fin", personality: 5, choosen: false 
            },
            {
               text:"F. Känslolös, phykopat och sjuk i huvudet", personality: 6, choosen: false 
            }
        ]
    }
   ,

   
]
//Massvis med variablar, Namnet på variablarna beskriver vad de gör/ är till för
let currentanswer = {};
let answers = [];
let undertext ='Bra jobbat! Nu är det dags för det riktiga quizet:';
let importent_information = "KOM IHÅG ATT LÄSA IGENOM ALLLLLLLA ALTERNATIV, TACK😊"
let finalaswer = "Långt quiz va!";
let finalaswer2 = "Du har just spenderat några minuter på ett totalt värdelöst quiz!"
let finalaswer3 = "Men men här har du vilka av Antons personlighet du är!"
let qIndex = 0;
let personalityes = ["BOSSIG ANTON", "PÅVERKAD ANTON", "GLAD ANTON", "ARG ANTON", "FÖRÄLSKAD ANTON", "KÄNSLOLÖS ANTON", ""]
let personality_dicription_index=0
let buttom_personality_text="Beskrivning av Persoligheterna"
let result_index = 0
let next_personality_buttom = "Nästa personlighet"
let background_music_varibel = "backgroundmusic.mp3"

//Musik till olika personligheter
let personality_musics = [    
   {
        pers_musics: [
            {
               music1: "bossig.mp3"
            }
        ]
    },
    {
        pers_musics: [
            {
               music1: "paverkad.mp3"
            }
        ]
    },
    {
        pers_musics: [
            {
               music1: "glad.mp3"
            }
        ]
    },
    {
        pers_musics: [
            {
               music1: "arg.mp3"
            }
        ]
    },
    {
        pers_musics: [
            {
               music1: "foralskad.mp3"
            }
        ]
    },
    {
        pers_musics: [
            {
               music1: "kanslolos.mp3"
            }
        ]
    },

   ]

//Funktionen kollar så man svarat på fråga först
//Sedan läggs alternativ man valt in i en lista, qindex plusas på 
function nextquestion(){


      if(Object.keys(currentanswer).length==0){
         alert("Hörrebörre bubbu, Nu tar vi det lilla lunga här. Svara på frågan IDIOT! (SWISHA MIG, 070-765-25-79)")
         return;
      }
      else{
        qIndex = qIndex + 1;
        answers.push(currentanswer)
        currentanswer = {} 
        undertext = ""
        
   
        if(qIndex==20)
            calculate1()
      }
    }

    //Räknar ut hur många gånger man valt varje personlighet i procent
    let results = []
    function calculate1(){
      for(let i=1; i<7; i++)
         results.push(answers.filter(obj => {
               return obj.personality == i;
            }).length/20*100);
      
      results = results
      
    }

    //Beskrivning av personligheter
    let pers_discription_list = [
    {
        pers_header:"BOSSIG ANTON",
        pers_text: [
            {
               pers1:"Du är narcissist! Du tror du är bäst på allt och att inget kan stoppa dig. Det ända som spelar roll i livet är dig själv och din familj. Världen kretsar runt dig och ditt liv går framför alla andras enligt dig själv. Du är på toppen av näringskedjan och om du hade fått alternativ om att 100 barn dör eller du hade du valt att 100 barn dör 10 gånger om. Brazzilian Phonk är din bästa vän och du pratar inte med så många. Några positiva aspekter är att du tränar otroligt hårt och effektivt. (Mer positiva aspekter har ännu inte upptäckts)"
            }
        ]
    },
    {
        pers_header:"PÅVERKAD ANTON",
        pers_text: [
            {
               pers1:"Du är litte lullig! Glad kan man och säga att du är och du vill prata med allt och alla. Du är otroligt snäll och ser bara den positiva sidan på allt och alla. Du är bara agressiv om du har en plastblomma i handen och denna blomma använder du för att tramatisera folks huvud. Din rizzometer är på Topp och du kan få vilken brud som helst (gäller även på bulk). Du blir även otroligt trött och sover en hel del. Något negativt är att du har IQ av en igelkott och kan inte tänka, du kan även inte stå upp."
            }
        ]
    },
    {
        pers_header:"GlAD ANTON",
        pers_text: [
            {
               pers1:"Du är glad, saker är bra och du har en skön vibe runt dig. Om du är på väldigt bra humör rekommenderar jag starkt att spela poker. Glad musik och barnlåtar är din bästa vän och du gillar att umgås och prata med andra individer. Du är dock jävligt skum och gör ba allmänt konstiga saker. Du gillar även att retas och göra folk irriterade eftersom du finner lycka i att se andra arga (Tuva)."
            }
        ]
    },
    {
        pers_header:"ARG ANTON",
        pers_text: [
            {
               pers1:"Du är läskig, otroligt läskig! Du är aggresiv som fan och vill slå ner allt och alla. Du blir arg på minsta lilla sak som att nån står vid diskon när du ska diska. Slag i bord och utbrott är också vanliga fenomen. Du är dock en gud i gymmet och lyfter som aldig förr, du tänker på allt folk har sagt till dig och pushar dig själv ännu hårdare. Du pratar bara med vissa men är mest tyst och lyssnar på musik. Poker är något som du inte ska spela eftersom det gör dig skuldsatt och mer aggresiv. "
            }
        ]
    },
    {
        pers_header:"FÖRÄLSKAD ANTON",
        pers_text: [
            {
               pers1:"Du har intresse för någon, du hatar denna personliget när du inte är den men älskar den när du är den (om du förstår svenskan där). Allt är bra i livet och du går runt med ett litet leende hela tiden. Träningen rullar på bra och skolandagarna går fort. Du är inne på snap för ofta och du kollar varje minut om hon har skrivit något. Du är väldigt snäll mot alla och blir sällan på dåligt humör. Men olyckligtvis finns denna personlighet oftas i väldigt korta stunder eftersom du till 95% blir dissad. Dock efter du blivit dissad är du magnifikisk i gymmet. "
            }
        ]
    },
    {
        pers_header:"KÄNSLOLÖS ANTON",
        pers_text: [
            {
               pers1:"Du vill hem och äta! Du har aldig varit så här hungrig och trött, allt du vill är att åka hem och käka och sen sova. Du har tränat alldeles för länge (oftas i 4 timmar) och allt i livet är meningslöst. Konstanta funderingar på vad jag gör med litt liv och om det verkligen är såhär jag vill leva. Depprimerad musik är en standard och du pratar inte med någon. Mat är din älskade och du ser hallucinationer av hambörgare. Du ser även förjävlig ut och vill bara dö. (Något positiv har ej än upptäckts)"
            }
        ]
    },
    {
      pers_header:"",
        pers_text: [
            {
               pers1:""
            }
        ]
    }
    
   ]
function qIndex_plus(){
   qIndex++
}

//När man gått igenom och läst om alla personligheter flyttas man till slutsida
function result_index_plus(){
   result_index++
   if(result_index==6)
      location.href='http://localhost:5173/Finalpage'

}

</script>
<!--Själva huvuduizet och frågor och alternativ skrivs ut-->
<div class="quiz-container" id="quiz">
   {#if qIndex<20}
    <div class="quiz-header">
        <h1><u>Fråga {qIndex+1}</u></h1>
        <h2>{undertext} {qIndex+1}/20</h2>
        <h3>{questions[qIndex].q}</h3>
        <div class="optionD1">
        {#each questions[qIndex].op as option, i}
        <div >
            <input class="answer" type="radio" bind:group={currentanswer} value={option} name="answer" id="D1">
            <label for="D1">{option.text}</label>
        </div>
        {/each}
        </div>
        <div>
            <button id="submit" class="submitbuttom"  on:click={nextquestion}>Nästa fråga</button>
        </div>
        <h4>{importent_information}</h4>
        <img src="tackfoorallt.jpg" alt="Bild på anton" class="picture_anton_left">
        <img src="data:image/jpeg;base64,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" alt="Slägg skaparen" class="picture_dad">
        <embed src={background_music_varibel} loop="true" autostart="true" class="background_music">
      

    
    </div>
    <!--Man ser hur mycket av varje personlighet man är-->
    {:else if qIndex==20}
    <h1 class="endheader">{finalaswer}</h1>
    <h2 class="endheader2">{finalaswer2}</h2>
    <h3 class="endheader3">{finalaswer3}</h3>
    {#each results as result, i}
    <p class="resultsstyle">{result}%</p>
    {/each}
    {#each personalityes as personalitye, i}
    <p class="personalitytextstyle">{personalitye}</p>
    {/each}
    <!--Slutbilder för varje personlighet-->
    <img src="bossiganton.jpg" alt="bossiganton" class="boss_anton">
    <img src="påverkadanton.jpg" alt="påverkadanton" class="påverkad_anton">
    <img src="gladanton.jpg" alt="gladanton" class="glad_anton">
    <img src="arganton.gif" alt="arganton" class="arg_anton">
    <img src="förälskadanton.jpg" alt="förälskadanton" class="förälskad_anton">
    <img src="känslolösanton.jpg" alt="känslolösanton" class="känslolös_anton">
    <!--Knapp till persolighets beskrivning sidor-->
    <button class="to_personalitiys"  on:click={qIndex_plus}>{buttom_personality_text}</button>
    <embed src="detkannsperfekt.mp3" loop="true" autostart="true" class="music_perfekt">

      <!--Läsa om de olika personligheter-->
    {:else}
    <h1 class="persoality_header_styling"><u>{personalityes[result_index]}</u></h1>
    <h2 class="end_procentege_styling">{results[result_index]}%</h2>
    {#each pers_discription_list[result_index].pers_text as pers_tex, l}
    <h2 class="pers_text_style">{pers_tex.pers1}</h2>
    {/each}
    {#each personality_musics[result_index].pers_musics as pers_music, k}
    <embed src={pers_music.music1} loop="true" autostart="true" class="music">
    {/each}
    <button class="next_personality"  on:click={result_index_plus}>{next_personality_buttom}</button>
    {/if}

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
        text-align: center;
        color: rgb(250, 252, 251);
        font-family: copperplate;
        font-size: 37px;
        margin-top: -50px;
        margin-bottom: 7px;
    }
    h4 {
      margin-left: -900px;
      color:   black;
      font-family: Impact;
      font-size: 25px;
      margin-top: -615px;
      margin-bottom: 7px;
    }
    .answer {
      background-color: white;
      border-color: black;
    }
    .picture_anton_left{
      width: 270px;
      height: 270px;
      margin-top: 320px;
      margin-left: -1200px;

    }
    .picture_dad {
      margin-right: -1200px;
      margin-top: -270px;
      width: 270px;
      height: 270px;
    }
    .background_music{
      width: 1px;
      height: 1px; 
      margin-top: 1px; 
    }
    .optionD1 {
        color:rgb(16, 16, 164);
        font-size: 30px;
        font-family: impact;
        display: flex;
        flex-direction: column;
        align-items:start;
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
    margin-top: 25px;
    }
    .to_personalitiys{
    width: 310px;
    height: 70px;
    border-radius: 25px;
    position: center;
    border: 5px solid black; 
    color: white; 
    background-color: rgb(25, 140, 228);
    font-size: 20px;
    font-family: copperplate;
    align-items: center;
    margin-top: 22px;
    margin-left: 567px;
    }
    .music_perfekt{
      width: 1px;
      height: 1px; 
      margin-top: 1px; 
    }
   .endheader{
      text-align: center;
      color: white;
      font-family: copperplate;
      font-size: 60px;
      margin-top: 10px;
    }
    .endheader2{
      text-align: center;
      color: rgb(250, 252, 251);
      font-family: copperplate;
      font-size: 41px;
      margin-top: -70px;
    }
    .endheader3{
      text-align: center;
      color: rgb(250, 252, 251);
      font-family: copperplate;
      font-size: 37px;
      margin-top: -50px;
      margin-bottom: 7px;
    }
    .resultsstyle {
      display: inline-block;
      margin-right: 100px;
      margin-left: 99px;
      font-family: Impact;
      font-size: 30px;
      color: black;
}
   .personalitytextstyle{
      display: inline-block;
      margin-right: 74px;
      margin-left: 55px;
      margin-top: -20px;
      font-family: Impact;
      font-size: 20px;
      color: black;
   }
   .boss_anton{
      width: 200px;
      height: 200px;
      margin-left: -110px;
   }
   .påverkad_anton{
      width: 200px;
      height: 200px;
      margin-left: 40px;
   }
   .glad_anton{
      width: 200px;
      height: 200px;
      margin-left: 45px;
   }
   .arg_anton{
      width: 200px;
      height: 200px;
      margin-left: 20px;
   }
   .förälskad_anton{
      width: 200px;
      height: 200px;
      margin-left: 30px;
   }
   .känslolös_anton{
      width: 240px;
      height: 200px;
      margin-left: 50px;
   }
   .persoality_header_styling{
      text-align: center;
      font-family: Impact;
      font-size: 71px;
      margin-top: 10px;
      color:black;
   }
   .end_procentege_styling{
      text-align: center;
      font-family: copperplate;
      font-size: 55px;
      margin-top: -70px;
      color:black;
   }
   .pers_text_style{
      text-align: center;
      font-family: Franklin Gothic Medium;
      font-size: 30px;
      margin-top: -70px;
      color:white;
   }
   .next_personality{
      width: 290px;
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
      margin-top: 70px;
    }
    .music{
      width: 1px;
      height: 1px; 
      margin-top: -900px; 
      margin-left: 0px;
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