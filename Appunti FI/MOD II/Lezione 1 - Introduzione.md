
# Contenuti del corso
> Si divide in 2 parti

- Calcolabilità
	1. Capire quali problemi possono essere risolti automaticamente 
		1. Strada facendo ci accorgeremo che esistono problemi che non hanno soluzioni
	2. Per farlo dobbiamo capire come risolvere un problmea automaticamente 
		2. Capire cosa significa risolvere un problema
		2. Capire cosa è un problema
- 
- Complessità
	1. Capire quali dei problemi che possono essere risolti, si possono risolvere veramente 
		1. Contraddizione!!
	2. Ce ne occuperemo più avanti 

# Problemi e istanze
- Cos'è un problema?
	- 'Quanto fa 5+2?' 
	- 'Quanto misura l'area di un rettangolo la cui base è lunga 28 cm e la cui altezza è lunga 12 cm?'

- Sbagliato!! Nell'esempio vengono illustrate due istanze di due problemi diversi 
- 
- I problemi di quelle istanze sono:
	1. Problema somma: dati due numeri naturali, n e k, calcolare il valore della somma di n + k
	2. Problema area: dato un rettangolo, la cui base è lunga b e la cui altezza è lunga h, calcolare l'area Adi quel rettangolo
	3. Chiara la distinzione? 
- 
- Un problema è la descrizione di un insieme di parametri, che chiameremo dati, collegati da un certo insieme di relazioni, associata alla richiesta di derivare da essi un altro insieme di parametri, che costituiscono la soluzione

- Un’istanza di un problema è un particolare insieme di valori associati ai dati

# Trovare la soluzione di un'istanza
- Per trovare la soluzione di talune istanze di taluni problemi posso sfruttare le caratteristiche di quelle istanze
	1. Se chiedi a un bambino quanto fa 2 + 5, quello può contare sulle dita
	2. Se hai bisogno di trovare sen , puoi disegnare la circonferenza goniometrica e vederlo 
- 
- D’altra parte, a volte non è così semplice
	1. Le dita non bastano per calcolare 49856739902+50672143559986
	2. E calcolare sen ... non è proprio una passeggiata 
- 
- Altre volte, è proprio impossibile
	1. per quanto tu sia bravo in matematica, un numero reale che corrisponda a , non c’è verso, non riuscirai mai a trovarlo
	2. Quando l’istanza di un problema non ha soluzione diciamo che essa è una istanza negativa 
	3. E cominciate a tenerla a mente questa cosa delle istanze negative, ché vi tornerà utile (eccome!)

# Risolvere un problema
- Risolvere un problema significa individuare un metodo che sappia trovare la soluzione di qualunque istanza positiva del problema
	1. e, in più, che sappia riconoscere se un’istanza è negativa
- 
- Ossia, significa trovare un procedimento che, data una qualunque istanza del problema, indichi la sequenza di azioni che devono essere eseguite per trovare la soluzione di quell’istanza
	1. o per poter concludere che, quell’istanza, una soluzione non ce l’ha
- 
- E qui sorgono un (bel) po’ di questioni:
	1. Innanzi tutto, cosa è un procedimento?
	2. E, poi, che cos’è una azione?
	3. E, infine, chi è supposto debba eseguire le azioni indicate?
- 
- Come stiamo per vedere, queste questioni sono fra loro interconnesse
- 
- Cos’è un procedimento?
	1. *Un procedimento è la descrizione di un insieme di azioni unita alla specifica dell’ordine con il quale le azioni devono essere eseguite*
- 
- E che cos’è una azione?
	1. Qualcosa che deve esser fatto, ovvio! Tuttavia...
	2. Anche “data un’istanza del problema, trova la soluzione di quell’istanza” è una azione
	3. Allora, dobbiamo dire che le azioni indicate in un procedimento, devono essere azioni semplici, azioni, cioè, che possono essere eseguite con facilità
- 
- ESEMPIO: data una funzione f: + e dati due numeri reali a e b, calcolare la misura dell’area della regione di piano compresa fra la funzione, l’asse x e le rette y=a e y=b
- 
- PROCEDIMENTO: 1) calcola la funzione primitiva F(x) di f(x) 2) calcola F(b) – F(a)
- 
- Un procedimento è la descrizione di un insieme di azioni unita alla specifica dell’ordine con il quale le azioni devono essere eseguite
	1. E, a ciascuna di quelle azioni, viene dato il nome di istruzione
- 
- E le istruzioni indicate in un procedimento, devono essere elementari, devono,
- cioè, essere azioni che possono essere eseguite con facilità
- 
- ESEMPIO: data una funzione f: + e dati due numeri reali a e b, calcolare la misura dell’area della regione di piano compresa fra la funzione, l’asse x e le rette y=a e y=b
- 
- PROCEDIMENTO: 1) calcola la funzione primitiva F(x) di f(x) 2) calcola F(b) – F(a)
- 
- Certo, quello indicato è un procedimento che risolve il problema nell’esempio

- Tuttavia, “calcola la funzione primitiva F(x) di f(x)” è davvero un’istruzione elementare?
	1. Per me (che sono una matematica) sì, per un bambino in prima elementare no...

- Cioè, che sia elementare o no, dipende da chi è supposto debba eseguire le azioni indicate

# Istruzione elementare 
- Dunque, se vogliamo svincolare la definizione di procedimento risolutivo di un problema da quello di esecutore delle azioni in esso indicate, è necessario, prima di tutto, chiarire formalmente cosa si intende con istruzione elementare

- Vediamo, a tal proposito, la soluzione individuata da Alan Turing a questa questione

- Turing, osservò che, indipendentemente dall’esecutore, qualunque istruzione, per potere essere definita elementare, deve avere le seguenti caratteristiche:
	1. Deve essere scelta in un insieme di “poche” istruzioni disponibili
	2. Deve scegliere l’azione da eseguire all’interno di un insieme di “poche” azioni possibili
	3. Deve poter essere eseguita ricordando una quantità limitata di dati, ossia, in termini più tecnici, utilizzando una quantità limitata di memoria.

- Osserviamo che le caratteristiche individuate da Turing indicano come istruzione elementare una operazione che possa essere eseguita... a mente!

- Chiariamo con un esempio

- Consideriamo il PROBLEMA SOMMA: dati due interi n e k, ci viene richiesto di calcolare il numero n + k

- Vogliamo progettare un procedimento che risolva questo problema


- 