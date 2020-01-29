# INTRODUZIONE

L’industria cinematografica più importante al mondo ha sede a Los Angeles, dove Hollywood vanta un giro di affari di miliardi di dollari.
Nell’era della grande rivoluzione digitale e sociale che stiamo vivendo, si può dire che l’ascesa dei social network impatti anche su un business così colossale? 

Abbiamo tentato di rispondere a questa domanda svolgendo una sentiment analysis sui tweet raccolti in tempo reale il giorno seguente all’uscita nelle sale di alcuni film statunitensi e verificando se ci fosse una correlazione tra questi risultati e gli incassi al botteghino ottenuti dagli stessi film nei sette giorni successivi.

---

La prima visualizzazione è costituita da un Sankey diagram, il quale mette in relazione la quantità di tweets raccolti il giorno successivo all'uscita di ciascun film, mettendoli in relazione con la relativa quantità di tweets riconosciuti come positivi o negativi dal servizio di Sentiment Analysis di Google. 
Il grafico è interattivo e permette all'utente di evidenziare i risultati di un particolare film, cliccando sul titolo o sull'immagine di copertina relativa.
<br/><br/>


<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/SentimentAnalysisSankey/SentimentSankey?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<br/><br/>
La seconda visualizzazione consiste in un diagramma a bolle, in cui ogni bolla varia in colore e dimensione in base al risultato ottenuto al botteghino nei 7 giorni successivi alla relativa raccolta dei tweets. Quanto più una bolla è grande e di colore tendente al rosso, tanto maggiore sarà l'incasso di quel film. Cliccando sulle stesse si possono visualizzare la copertina, l'incasso in milioni di dollari e i generi a cui appartiene il film (secondo il catalogo di IMDb).
<br/><br/>


<div style = 'display:flex; position:absolute; right:0; left:0; '>
      <div id = 'sankey2' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src=" https://public.tableau.com/views/Box-officebubblechart/Boxoffice?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center"></iframe>
      </div>
 </div>
 <div style="height: 1050px;"> </div>

<br/><br/>
La terza visualizzazione infine prescinde dal film (usa i dati originari per calcolare una matrice di correlazione secondo Spearman) per mostrare se e quanto l'incasso, la magnitudo media dei tweet e il sentiment medio degli stessi presentino correlazione tra di essi.
In statistica, una correlazione è una relazione tra due variabili tale che a ciascun valore della prima corrisponda un valore della seconda, seguendo una certa regolarità.

Per mostrarla si è scelto di rappresentarla in una matrice di correlazione, in cui per ogni coppia di variabili si mostra un cerchio, la cui area e il cui colore varia in base al valore dell'indice di correlazione. Quanto più è grande il cerchio, tanto maggiore è il valore dell'indice. Il colore varia da verde (correlazione positiva) a rosso (correlazione negativa). Il valore, selezionabile tramite click con il mouse, viene inoltre stampato a lato della matrice stessa.

Poichè non tutti gli utenti erano familiari con il concetto statistico in questione, abbiamo preferito aggiungere una breve spiegazione munita di esempi nella nuvolettà a destra del titolo: "Che cos'è la correlazione?"
<br/><br/>

 <div style = 'display:flex; position:absolute; right:0; left:0; '>
      <div id = 'sankey3' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/shared/QTTY92TXW?:showVizHome=no&:embed=true" width = '1300' height = '1000'  scrolling='no' style="text-align:center"></iframe>
      </div>
 </div>
<div style="height: 1000px;"> </div>

## CONCLUSIONE
Conclusione 

---

# NOTE METODOLOGICHE

## DATI UTILIZZATI
Queste visualizzazioni sono state sviluppate a partire dai dati raccolti tramite il processo accuratamente spiegato in <a href="LINK REPORT">questo report</a>, usando un modulo python appositamente creato per lo scopo e un'architettura in grado di raccogliere i dati in tempo reale da Twitter.
I dati sono stati poi convertiti in formato csv per essere utilizzati con il software usato (Tableau Desktop).

## PULIZIA DEI DATI
Per data cleaning si intende il processo di preparazione dei dati su cui si dovranno condurre le analisi. I tweet sono stati puliti eliminando i metadati, conctractions, URL e e-mail, righe vuote, tabs e punteggiatura ed applicando i processi di stemming e lemmatization. Lo stemming serve a ridurre le parole alle loro “radici”, mentre la lemmatization è il processo di riduzione di una forma flessa di una parola alla sua forma canonica, detta lemma (o forma base). Questo al fine di ottenere risultati più affidabili e non sfalsati da retweet o tweet pubblicitari. 

# QUALITY ASSESSMENTS
Per fare una verifica della qualità delle nostre visualizzazioni sono stati effettuati tre tipologie di assessment: 
* una valutazione qualitativa delle euristiche
* un questionario psicometrico 
* uno user test.

## VALUTAZIONE QUALITATIVA DELLE EURISTICHE
Si sono intervistati 4 utenti, a cui è stato chiesto di interagire e di giocare con le infografiche da noi sviluppate e di "pensare" ad alta voce. In questo modo è stato possibile individuare le seguenti criticità:
* La terza visualizzazione non risultava chiara e comprensibile agli utenti che non avevano familiarità con tale concetto statistico. Per questo motivo si è scelto di inserire una "nuvoletta" che fornisse definizione ed esempi al passare del mouse.
* 2
* 3

## QUESTIONARIO PSICOMETRICO
Per poter valutare le nostre visualizzazioni abbiamo sottoposto un questionario psicometrico secondo il modello Cabitza-Locoro a 60 utenti. Ad essi stato chiesto di valutare ciascuna delle nostre tre visualizzazioni tramite una scala da 1 (Poco) a 6 (Molto) i seguenti attributi qualitativi:
* Chiarezza
* Utilità
* Bellezza
* Intuitività
* Informatività
* Totale
<br/><br/>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_questionario_fig1/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_questionario_fig2/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_questionario_fig3/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<br/><br/>
Analizzando i risultati, il risultato più rilevante è che, in generale, la terza infografica è stata di più difficile comprensione. Questo è un dato che ci attendevamo, vista la difficoltà del concetto statistico per coloro che non ne sono stati precedentemente esposti. Ci riteniamo comunque soddisfatti di un tale risultato nonostante la difficoltà del concetto visualizzato.
Per quanto riguarda le altre due infografiche, invece, si nota una significativa maggioranza di giudizi positivi, specialmente per la seconda infografica.

Per valutare la correlazione tra gli attributi qualitativi presenti nel questionario abbiamo ritenuto opportuno l’utilizzo di una matrice di correlazione, visualizzata come nella nostra infografica numero 3, a cui abbiamo affiancato uno scatter plot. Quest'ultimo rappresenta, per ciascuna valutazione, il valore complessivo assegnato dall'utente e il valore calcolato a partire dalle sue risposte, tramite il procedimento spiegatoci dal professor Cabitza. 
<br/><br/>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/Scatterecorrelazione_questionario_fig1/Correlazione?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/Scatterecorrelazione_questionario__fig2/Correlazione?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/Scatterecorrelazione_questionario__fig3/Correlazione?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<br/><br/>
Nel triangolo superiore sono presenti dei corrplot, che si differenziano tra loro per forma e colore. Questi ultimi indicano la forza della correlazione, che varia da -1 a 1. Più la forma è simile ad un ellisse, maggiore è la correlazione, che a seconda dell’inclinazione verso l’alto o il basso può essere rispettivamente positiva o negativa. Più la forma è simile ad un cerchio, invece, più tale attributo si avvicina allo 0. Il blu corrisponde a valori positivi mentre il rosso a quelli negativi; in questo caso tutte le correlazioni presenti sono positive. Si può notare in tutte e tre le infografiche la coppia di attributi "Chiara" e "Intuitiva" risultano avere la correlazione più alta, mediamente pari all'87%.

## TEST UTENTE
Per ottenere un feedback sull’efficienza generale e sull'usabilità del report è stato chiesto a 16 utenti di svolgere 3 task differenti (uno per ogni infografica), registrando la correttezza delle risposte e il tempo impiegato, misurandolo in secondi. Si è scelto in questo caso di focalizzare l'attenzione sulla tipologia di utente che si interagisce con l'infografica; per questo motivo è stato chiesto agli utenti di auto-definirsi "esperti" o "non esperti" di dati in base al campo di studio/lavoro. Questo ha permesso di verificare se ci fossero differenze significative tra i due gruppi.
Per valutare la differenza dei tempi di risposta e la relativa distribuzione, è stato ritenuto opportuno l’utilizzo di violin plot riportati di seguito.
<br/><br/><br/><br/>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_task_fig1/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_task_fig2/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/violin_task_fig3/Template?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<br/><br/>
È possibile notare che, per tutti e tre i task, i tempi di risposta di chi si ritiene non esperto di dati, sono maggiori rispetto a chi, invece, si ritiene esperto.
In particolare, la differenza tra i tempi di esecuzione medi tra gli utenti esperti e non risulta essere di 23,7 secondi per il task 1, di 11,6 secondi per il task 2 e di 17,1 secondi per il task riferito all'ultima infografica.
Per valutare la significatività di queste quantità sono stati effettuati test t da cui è emerso, appunto, che tale differenza tra i tempi medi di esecuzione è statisticamente significativa per tutti e tre i task. (p value Task1= 0.000174, p-value Task2= 8.324e-05, p-value Task3 = 0.00359)
<br/><br/>
<br/><br/>

