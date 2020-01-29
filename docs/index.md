# Introduzione

Metti intro del paper

<br/><br/>
La prima visualizzazione è costituita da un Sankey diagram, il quale mette in relazione la quantità di tweets raccolti il giorno successivo all'uscita di ciascun film, con la relativa quantità di tweets riconosciuti come positivi o negativi dal servizio di Sentiment Analysis di Google. 
<br/><br/>
<br/><br/>

<div style = 'display:flex; position:absolute; right:0; left:0;'>
      <div id = 'sankey1' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/views/SentimentAnalysisSankey/SentimentSankey?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center" align="center"></iframe>
      </div>
 </div>
<div style="height: 1050px;"> </div>

<br/><br/>
La seconda visualizzazione pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru....
<br/><br/>
<br/><br/>

<div style = 'display:flex; position:absolute; right:0; left:0; '>
      <div id = 'sankey2' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src=" https://public.tableau.com/views/Box-officebubblechart/Boxoffice?:showVizHome=no&:embed=true" width = '1300' height = '1050'  scrolling='no' style="text-align:center"></iframe>
      </div>
 </div>
 <div style="height: 1050px;"> </div>

<br/><br/>
La terza visualizzazione pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru pirupirupiru....
<br/><br/>
<br/><br/>

 <div style = 'display:flex; position:absolute; right:0; left:0; '>
      <div id = 'sankey3' style = 'margin:auto;'> 
           <iframe seamless frameborder="0" src="https://public.tableau.com/shared/QTTY92TXW?:showVizHome=no&:embed=true" width = '1300' height = '1000'  scrolling='no' style="text-align:center"></iframe>
      </div>
 </div>
<div style="height: 1000px;"> </div>

<br/><br/>

---


# Note metodologiche

## DATI UTILIZZATI
Questo report è stato sviluppato a partire da dati raccolti per tutto il mese di Maggio dalle API ufficiali di Trenitalia. La particolare natura e il complesso meccanismo di questi strumenti ha reso necessario l'impiego di un'architettura in grado di raccogliere i dati in tempo reale. Per approfondire si faccia riferimento a questo documento.
I dati sono stati inizialmente esportati dal database in formato json e successivamente convertiti in formato csv compatibile con il software utilizzato (PowerBI).

## PREPROCESSING
Durante una prima fase di preprocessing i dati grezzi sono stati "puliti" pirupirupiru

# Questionari
Per fare un check sulla qualità delle nostre infografiche sono stati effettuati tre tipologie di assessment: la valutazione qualitativa delle euristiche, il questionario psicometrico e lo user test.

## VALUTAZIONE QUALITATIVA DELLE EURISTICHE
Sono state intervistati tre utenti a cui è stato chiesto di interagire con le infografiche per qualche minuto e di commentare ad alta voce i diversi grafici.
Grazie a questo tipo di attività è stato possibile individuare i seguenti problemi delle infografiche:

Non risultava immediato rimuovere i numerosi filtri presenti nella prima infografica. Per questo motivo è stata inserita, tramite il pulsante freccia "back" la possibilità di tornare allo stato iniziale della visualizzazione, nonostante queste non fosse una funzione automatica di PowerBI, come spiegato precedentemente.
Sempre nella prima infografica, selezionando una stazione di partenza, vengono automaticamente visualizzate le stazioni di arrivo (capolinea) dei treni in questione. In alcuni casi, invece, gli utenti pensavano di poter vedere tutte le fermate intermedie del treno. Non è stato possibile, tuttavia, assecondare questi suggerimenti per vincoli legati allo schema relazionale dei dati stessi.
Nella flow map, oltre alle tratte, erano state inizialmente inserite anche le stazioni, colorate in base al ritardo medio accumulato, ma risultava troppo pesante come visualizzazione quindi si è scelto di rimuoverle.

## QUESTIONARIO PSICOMETRICO
Per poter valutare la nostra prima visualizzazione abbiamo sottoposto il questionario psicometrico Cabitza-Locoro a 32 utenti. E' stato chiesto loro di valutare le tre infografiche principali attraverso una scala da 1 (Pochissimo) a 6 (Moltissimo) relativamente agli attributi qualitativi “Utilità”, “Intuitività”, “Chiarezza”, “Informatività”, “Bellezza” e “Valutazione Generale”.
<br/><br/><br/><br/>

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
Analizzando i barchart, il risultato più rilevante è che, in generale, la prima infografica è stata di più difficile comprensione. Risulta esserci una percentuale significativa di risposte negative, soprattutto relativamente alla "Chiarezza" e "Intuitività" dell'infografica.
Per quanto riguarda le altre due infografiche, invece, si nota una significativa maggioranza di giudizi positivi sia rispetto alle risposte neutre che negative.

Per valutare la correlazione tra gli attributi qualitativi presenti nel questionario abbiamo ritenuto opportuno l’utilizzo di un correlogramma.
<br/><br/><br/><br/>

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

