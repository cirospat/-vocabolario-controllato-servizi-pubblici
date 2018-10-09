
.. _h79675c214249d425368162c2919705b:

3. Profilo di applicazione del Vocabolario del servizio pubblico principale (CPSV-AP)
#####################################################################################

La specifica del profilo di applicazione del vocabolario del servizio pubblico principale è rappresentata in un diagramma di classe UML . La Figura 2 mostra il profilo completo che include:

* Le classi e le proprietà che definiscono il servizio stesso: gli input necessari, i possibili output, l'autorità pubblica responsabile e gli eventi che determinano l'utilizzo del servizio;

* Le classi e le proprietà che descrivono il contesto in cui viene offerto il servizio. Ciò include la legislazione pertinente e le regole di funzionamento per il servizio; e

* L' interfaccia tra il servizio e i suoi utenti: come e quando è possibile accedervi. 


|REPLACE1|


Figura 2. Rappresentazione grafica delle relazioni tra le classi e le proprietà del profilo completo del profilo di vocabolario del servizio pubblico Core

.. _h31137ad3d47725f43656f601434:

3.1.  Classi obbligatorie e facoltative e proprietà di CPSV-AP
**************************************************************

Per indicare i requisiti minimi per conformarsi a CPSV-AP, le classi e le proprietà vengono classificate come obbligatorie o facoltative. Un'implementazione minima di CPSV-AP fornisce almeno informazioni sulle proprietà obbligatorie delle classi obbligatorie. Le classi facoltative possono comunque avere proprietà obbligatorie per le quali devono essere fornite informazioni quando la classe specifica viene utilizzata nella descrizione dei servizi pubblici e degli eventi aziendali.

 

I termini di classe obbligatoria, classe facoltativa, proprietà obbligatoria e proprietà facoltativa hanno il seguente significato:

 

* Classe obbligatoria : un ricevitore di dati DEVE essere in grado di elaborare le informazioni sulle istanze della classe; un mittente di dati DEVE fornire informazioni sulle istanze della classe.

* Classe opzionale : un ricevitore DEVE essere in grado di elaborare le informazioni sulle istanze della classe; un mittente può fornire le informazioni ma non è obbligato a farlo.

* Proprietà obbligatoria : un ricevitore DEVE essere in grado di elaborare le informazioni per quella proprietà; un mittente DEVE fornire le informazioni per quella proprietà. Nel caso in cui la classe corrispondente sia classificata come facoltativa, un ricevitore DEVE essere in grado di elaborare le informazioni per quella proprietà; un mittente DEVE fornire le informazioni per quella proprietà se utilizza la classe corrispondente.

* Proprietà opzionale : un ricevitore DEVE essere in grado di elaborare le informazioni per quella proprietà; un mittente può fornire le informazioni per quella proprietà se è disponibile.

 

Tutte le classi includono la proprietà obbligatoria dell'identificatore che nelle codifiche dei dati collegati / RDF saranno IRI. Laddove le entità non esistano indipendentemente dal servizio pubblico, è consentito che queste siano locali all'implementazione, vale a dire che i nodi vuoti sono esplicitamente consentiti. Gli IRI globali DEVONO essere assegnati al servizio pubblico stesso, alle organizzazioni pubbliche, agli eventi, ai risultati, agli agenti, alle prove e ai quadri formali.  

 

Il significato dei termini DEVE, NON DEVE, DOVREBBE e POTREBBE in questa sezione e nelle seguenti sezioni sono come definiti nella RFC 2119\ [#F1]_\  [11] .

 

Nel contesto indicato, il termine "elaborazione" indica che i ricevitori devono accettare i dati in arrivo e fornire in modo trasparente questi dati alle applicazioni e ai servizi. Non implica né prescrive quali applicazioni e servizi possono finalmente fare con i dati (analizzare, convertire, memorizzare, rendere ricercabili, visualizzare agli utenti, ecc.).

 

" Elenco dettagliato di classi e proprietà obbligatorie e facoltative " fornisce una panoramica delle classi classificate come obbligatorie o facoltative. Per ogni classe viene fornita una panoramica delle proprietà classificate come obbligatorie e per le quali l'utilizzo è facoltativo.

 

Inoltre, la proposta in " Elenco dettagliato di classi e proprietà obbligatorie e facoltative " è stata discussa con il gruppo di lavoro.

.. _h5b3a35697e604432331706750421f5a:

3.2. La classe di servizio pubblico
***********************************

Questa classe rappresenta lo stesso servizio pubblico, come descritto in un catalogo di servizi pubblici. Un servizio pubblico è un insieme obbligatorio o discrezionale di attività svolte o in grado di essere eseguite da o per conto di un'organizzazione pubblica, finanziate con fondi pubblici e derivanti da politiche pubbliche. I servizi possono essere a beneficio di un individuo, un'azienda o altra autorità pubblica o gruppi di uno di questi. Un servizio esiste indipendentemente dal fatto che sia usato o meno, e il termine "beneficio" può essere applicato nel senso di consentire l'adempimento di un obbligo. Come definito nella versione rivista del Quadro europeo di interoperabilità\ [#F2]_\ , un servizio pubblico europeo comprende qualsiasi servizio fornito da pubbliche amministrazioni in Europa, o da altre organizzazioni a loro nome, a imprese, cittadini o altre amministrazioni pubbliche.


+-----------------+------------+-------------------+
|\ |STYLE0|\      |\ |STYLE1|\ |\ |STYLE2|\        |
+-----------------+------------+-------------------+
|Servizio pubblico|Obbligatorio|CPsV: PublicService|
+-----------------+------------+-------------------+

 

Le seguenti sottosezioni definiscono le proprietà della classe Servizio pubblico.

.. _h292c697d81a147bf346c237585b29:

3.2.1. Identifier
-----------------

Questa proprietà rappresenta un identificatore formalmente emesso per il servizio pubblico.

 

+--------------+-------------------+------------+------------+
|\ |STYLE3|\   |\ |STYLE4|\        |\ |STYLE5|\ |\ |STYLE6|\ |
+--------------+-------------------+------------+------------+
|identificatore|DCT: identificatore|Testo [13]  |1..1        |
+--------------+-------------------+------------+------------+

.. _h56804f1e2c696b6e6d295727565137:

3.2.2. Nome
-----------

Questa proprietà rappresenta il nome ufficiale del servizio pubblico.

 

+------------+------------+------------+-------------+
|\ |STYLE7|\ |\ |STYLE8|\ |\ |STYLE9|\ |\ |STYLE10|\ |
+------------+------------+------------+-------------+
|nome        |DCT: titolo |Testo       |1..1         |
+------------+------------+------------+-------------+

.. _h7648d4465c342c69236680605028:

3.2.3. Descrizione
------------------

Questa proprietà rappresenta un testo libero Descrizione del servizio pubblico. La descrizione è probabilmente il testo che i potenziali utenti del servizio pubblico vedono in qualsiasi catalogo di servizi pubblici. Le amministrazioni pubbliche sono incoraggiate a includere un ragionevole livello di dettaglio nella descrizione, ad esempio includendo i requisiti di idoneità di base per il particolare servizio pubblico e le informazioni di contatto.

 

+-------------+----------------+-------------+-------------+
|\ |STYLE11|\ |\ |STYLE12|\    |\ |STYLE13|\ |\ |STYLE14|\ |
+-------------+----------------+-------------+-------------+
|descrizione  |DCT: Descrizione|Testo        |1..1         |
+-------------+----------------+-------------+-------------+

.. _h1859c39147e41103428513e412c3a22:

3.2.4. Parola chiave
--------------------

Questa proprietà rappresenta una parola chiave, un termine o una frase per descrivere il servizio pubblico.

 

+-------------+-------------------+-------------+-------------+
|\ |STYLE15|\ |\ |STYLE16|\       |\ |STYLE17|\ |\ |STYLE18|\ |
+-------------+-------------------+-------------+-------------+
|parola chiave|DCAT: parola chiave|Testo        |0..n         |
+-------------+-------------------+-------------+-------------+

.. _h787c45843771eb1b11d165f5c7a7b:

3.2.5. Settore
--------------

Questa proprietà rappresenta l'industria o il settore a cui un servizio pubblico si riferisce o è destinato. Ad esempio: ambiente, sicurezza, abitazioni. Si noti che un singolo servizio pubblico può riguardare più settori. I possibili valori per questa proprietà sono forniti come un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+-------------+-------------+-------------+-------------+
|\ |STYLE19|\ |\ |STYLE20|\ |\ |STYLE21|\ |\ |STYLE22|\ |
+-------------+-------------+-------------+-------------+
|settore      |cv: Settore  |Concetto     |0..n         |
+-------------+-------------+-------------+-------------+

.. _h29391930134259620177f6018161971:

3.2.6. Area tematica
--------------------

Questa proprietà rappresenta l'area tematica di un servizio pubblico come descritto in un vocabolario controllato, ad esempio protezione sociale, salute, ricreazione, cultura e religione, famiglia, affari economici in viaggio , tasse, personale, ambiente ... I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+-------------+----------------+-------------+-------------+
|\ |STYLE23|\ |\ |STYLE24|\    |\ |STYLE25|\ |\ |STYLE26|\ |
+-------------+----------------+-------------+-------------+
|Area tematica|cv: thematicArea|Concetto     |0..n         |
+-------------+----------------+-------------+-------------+

.. _h5d1611f69315ce551d3d5dd44177c:

3.2.7. genere
-------------

Questa proprietà rappresenta il tipo di un servizio pubblico come descritto in un vocabolario controllato. Per indicare il Tipo, ci riferiamo alle funzioni del governo per indicare lo scopo di un'attività governativa, a cui è destinato il servizio pubblico. I vocabolari controllati raccomandati sono elencati nella sezione 4 .


+-------------+-------------+-------------+-------------+
|\ |STYLE27|\ |\ |STYLE28|\ |\ |STYLE29|\ |\ |STYLE30|\ |
+-------------+-------------+-------------+-------------+
|genere       |DCT: Tipo    |Concetto     |0..n         |
+-------------+-------------+-------------+-------------+

.. _h405977427138297c726743a5e516579:

3.2.8. linguaggio
-----------------

Questa proprietà rappresenta la lingua / le lingue in cui è disponibile il servizio pubblico. Questa potrebbe essere una lingua o più lingue, ad esempio in paesi con più di una lingua ufficiale. I valori possibili per questa proprietà sono descritti in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+-------------+-------------+---------------------+-------------+
|\ |STYLE31|\ |\ |STYLE32|\ |\ |STYLE33|\         |\ |STYLE34|\ |
+-------------+-------------+---------------------+-------------+
|linguaggio   |DCT: lingua  |DCT: LinguisticSystem|0..n         |
+-------------+-------------+---------------------+-------------+

.. _hc4959f77f7246246229444f208056:

3.2.9. Stato
------------

Indica se un servizio pubblico è attivo, inattivo, in fase di sviluppo ecc. In base a un vocabolario controllato.

 

+-------------+-------------+-------------+-------------+
|\ |STYLE35|\ |\ |STYLE36|\ |\ |STYLE37|\ |\ |STYLE38|\ |
+-------------+-------------+-------------+-------------+
|stato        |ADMS: Stato  |Concetto     |0..1         |
+-------------+-------------+-------------+-------------+

.. _h05a2ec1755a2c653d64c2740453:

3.2.10. È raggruppato da
------------------------

Questa proprietà collega il servizio pubblico alla classe Event (sezione 3.2.25 ). Diversi servizi pubblici possono essere associati a un particolare evento e, allo stesso modo, lo stesso servizio pubblico può essere associato a diversi eventi.

 

+-------------+---------------+-------------+-------------+
|\ |STYLE39|\ |\ |STYLE40|\   |\ |STYLE41|\ |\ |STYLE42|\ |
+-------------+---------------+-------------+-------------+
|isGroupedBy  |cv: isGroupedBy|Evento       |0..n         |
+-------------+---------------+-------------+-------------+

.. _h677b6033434e234848265317631f29:

3.2.11. Richiede
----------------

Un servizio pubblico può richiedere, o in qualche modo utilizzare, l'output di uno o più altri servizi pubblici. In questo caso, affinché un servizio pubblico sia eseguito, un altro servizio pubblico deve essere eseguito in anticipo. La natura del requisito sarà descritta nella relativa regola o input.

 

+-------------+-------------+-----------------+-------------+
|\ |STYLE43|\ |\ |STYLE44|\ |\ |STYLE45|\     |\ |STYLE46|\ |
+-------------+-------------+-----------------+-------------+
|richiede     |DCT: richiede|Servizio pubblico|0..n         |
+-------------+-------------+-----------------+-------------+

.. _h4e26691e7549133d46544053b183b28:

3.2.12. Relazionato
-------------------

Questa proprietà rappresenta un servizio pubblico correlato alla particolare istanza della classe di servizio pubblico.

 

+-------------+--------------+-----------------+-------------+
|\ |STYLE47|\ |\ |STYLE48|\  |\ |STYLE49|\     |\ |STYLE50|\ |
+-------------+--------------+-----------------+-------------+
|relazionato  |DCT: relazione|Servizio pubblico|0..n         |
+-------------+--------------+-----------------+-------------+

.. _h3e5a6e6431794f731a7130522765786f:

3.2.13. Criterion
-----------------

Collega un servizio pubblico a una classe che descrive i criteri per la necessità o l'utilizzo del servizio, come la residenza in un dato luogo, il superamento di una certa età, ecc. La classe Criterion è definita nel vocabolario Core Criterion e Core Evidence Vocabulary\ [#F3]_\  [14] .

 

+-------------+----------------+---------------------+-------------+
|\ |STYLE51|\ |\ |STYLE52|\    |\ |STYLE53|\         |\ |STYLE54|\ |
+-------------+----------------+---------------------+-------------+
|hasCriterion |cv: hasCriterion|Criterio obbligatorio|0..n         |
+-------------+----------------+---------------------+-------------+

.. _h9522b443c5e5b1f6d2551296e325d55:

3.2.14. Ha autorità competente
------------------------------

La struttura, collega un servizio pubblico ad un ente pubblico, che è l'agente responsabile della consegna del Servizio Pubblico. Se la particolare organizzazione pubblica fornisce direttamente o esternalizza il servizio pubblico non è rilevante. L' Organizzazione pubblica che è l'autorità competente del servizio è quella che è in definitiva responsabile della gestione e della fornitura del servizio pubblico.

 

Il termine Autorità Competente è definito nella Direttiva sui Servizi (2006/123 / CE) nel modo seguente:

 

"Qualsiasi organismo o autorità che abbia un ruolo di supervisione o di regolamentazione in uno Stato membro in relazione alle attività di servizi, comprese, in particolare, le autorità amministrative, compresi i tribunali in quanto tali, gli organismi professionali e le associazioni professionali o altre organizzazioni professionali che, in l'esercizio della loro autonomia legale, regolano in modo collettivo l'accesso alle attività di servizio o il loro esercizio ".

 

+---------------------+-------------------------+-----------------------+-------------+
|\ |STYLE55|\         |\ |STYLE56|\             |\ |STYLE57|\           |\ |STYLE58|\ |
+---------------------+-------------------------+-----------------------+-------------+
|hasCompetentAuthority|cv: hasCompetentAuthority|Organizzazione pubblica|1..1         |
+---------------------+-------------------------+-----------------------+-------------+

.. _hf5c299283d596c4718287d5e2336b:

3.2.15. Ha la partecipazione
----------------------------

Il CPSV-AP definisce i due ruoli fondamentali dell'autorità competente e del fornitore di servizi, ma questo modello semplice può essere esteso, se necessario, utilizzando la proprietà Has Participation che collega alla classe di partecipazione (vedere la sezione 3.6).

 

+----------------+--------------------+--------------+-------------+
|\ |STYLE59|\    |\ |STYLE60|\        |\ |STYLE61|\  |\ |STYLE62|\ |
+----------------+--------------------+--------------+-------------+
|hasParticipation|cv: hasParticipation|Partecipazione|0..n         |
+----------------+--------------------+--------------+-------------+

.. _h694d3558702a57737a155e75034f7f:

3.2.16. Ha Input
----------------

La proprietà Has Input collega un servizio pubblico a una o più istanze della classe Evidence (vedere la sezione 3.9). Un servizio pubblico specifico può richiedere la presenza di determinati elementi di prova per essere consegnati. Se la prova richiesta per usufruire di un servizio varia a seconda del canale attraverso il quale è accessibile, allora l'Input deve essere al livello del Canale (sezione 3.12.4).

 

+-------------+--------------+-------------+-------------+
|\ |STYLE63|\ |\ |STYLE64|\  |\ |STYLE65|\ |\ |STYLE66|\ |
+-------------+--------------+-------------+-------------+
|hasInput     |CPsV: hasInput|Prova        |0..n         |
+-------------+--------------+-------------+-------------+

.. _h5a6c252912f50594fc3a7949413c27:

3.2.17. Ha una risorsa legale
-----------------------------

La proprietà Has Formal Framework collega un servizio pubblico a un framework formale. Indica il quadro formale (ad esempio la legislazione) a cui il servizio pubblico si riferisce, opera o ha la sua base legale.

 

+----------------+-------------------+--------------+-------------+
|\ |STYLE67|\    |\ |STYLE68|\       |\ |STYLE69|\  |\ |STYLE70|\ |
+----------------+-------------------+--------------+-------------+
|hasLegalResource|cv: hasLegalResouce|Risorsa legale|0..n         |
+----------------+-------------------+--------------+-------------+

.. _h742e20651039502f322da713b1a3b75:

3.2.18. Produce
---------------

La proprietà Produces collega un servizio pubblico a una o più istanze della classe Output (vedere la sezione 3.10), descrivendo il risultato effettivo dell'esecuzione di un determinato servizio pubblico. Le uscite possono essere qualsiasi risorsa, ad esempio un documento, un manufatto o qualsiasi altra cosa prodotta dall'esecuzione del servizio pubblico.

 

+-------------+-------------+-------------+-------------+
|\ |STYLE71|\ |\ |STYLE72|\ |\ |STYLE73|\ |\ |STYLE74|\ |
+-------------+-------------+-------------+-------------+
|produce      |CPsV: produce|Produzione   |0..n         |
+-------------+-------------+-------------+-------------+

.. _h1da4522f6078304927b3e79724928:

3.2.19. segue
-------------

La proprietà follows collega un servizio pubblico alla / e regola / e in base alla quale opera. La definizione della classe Rule è molto ampia. In un caso tipico, l'autorità competente che fornisce il servizio pubblico definirà anche le regole che implementeranno le proprie politiche. Il CPSV-AP è flessibile per consentire variazioni significative in tale scenario.

 

+-------------+-------------+-------------+-------------+
|\ |STYLE75|\ |\ |STYLE76|\ |\ |STYLE77|\ |\ |STYLE78|\ |
+-------------+-------------+-------------+-------------+
|segue        |CPsV: segue  |Regola       |0..n         |
+-------------+-------------+-------------+-------------+

.. _h23d584d2c6d2650b544b3f6f43627:

3.2.20.  Spaziale
-----------------

È probabile che un servizio pubblico sia disponibile solo all'interno di una determinata area, in genere l'area coperta da una particolare autorità pubblica.

 

Un uso comune della proprietà spaziale sarà la definizione delle unità territoriali amministrative, in genere un paese o una regione, in cui è disponibile un servizio pubblico. L'Ufficio delle pubblicazioni dell'Unione europea offre una serie di URI\ [#F4]_\  adatto a questo scopo, ad esempio Malta è identificata da \ |LINK1|\  ,

Fiandre occidentali da \ |LINK2|\   e così via.

 

NB: La limitazione spaziale non è intesa per essere utilizzata per descrivere l'ammissibilità o la velocità di funzionamento del servizio. Questi aspetti saranno coperti dalla classe Criterion.

 

+-------------+-------------+-------------+-------------+
|\ |STYLE79|\ |\ |STYLE80|\ |\ |STYLE81|\ |\ |STYLE82|\ |
+-------------+-------------+-------------+-------------+
|spaziale     |DCT: spaziale|Posizione    |0..n         |
+-------------+-------------+-------------+-------------+

.. _h2457406c8122828546f697f5c524173:

3.2.21. Ha un punto di contatto
-------------------------------

Un punto di contatto per il servizio è quasi sempre utile. Il valore di questa proprietà, le informazioni di contatto stesso, devono essere fornite utilizzando lo schema: ContactPoint. Si noti che le informazioni di contatto dovrebbero essere rilevanti per il servizio pubblico che potrebbe non essere lo stesso delle informazioni di contatto per l'autorità competente o qualsiasi partecipante.

 

+---------------+-------------------+-----------------+-------------+
|\ |STYLE83|\   |\ |STYLE84|\       |\ |STYLE85|\     |\ |STYLE86|\ |
+---------------+-------------------+-----------------+-------------+
|hasContactPoint|cv: hasContactPoint|Punto di contatto|0..n         |
+---------------+-------------------+-----------------+-------------+

.. _h21182924602a2a5a2019726622555c80:

3.2.22. Ha un canale      
--------------------------

Questa proprietà collega il Servizio pubblico a qualsiasi canale attraverso il quale un agente fornisce, utilizza o interagisce in altro modo con il servizio pubblico, come un servizio online, un numero di telefono o un ufficio. Vedi sezione 3.12.

 

+-------------+--------------+-------------+-------------+
|\ |STYLE87|\ |\ |STYLE88|\  |\ |STYLE89|\ |\ |STYLE90|\ |
+-------------+--------------+-------------+-------------+
|hasChannel   |cv: hasChannel|Canale       |0..n         |
+-------------+--------------+-------------+-------------+

.. _h373f1e414e445d2c3d641915101e5f26:

3.2.23. Tempo di elaborazione
-----------------------------

Il valore di questa proprietà è il tempo (stimato) necessario per l'esecuzione di un servizio pubblico. Le informazioni reali sono fornite utilizzando la sintassi ISO8601 per le durate. Alcuni esempi sono forniti di seguito:

+--------------+--------+
|Durata        |Sintassi|
+--------------+--------+
|5 anni        |P5Y     |
+--------------+--------+
|1 mese        |P1M     |
+--------------+--------+
|3 giorni      |P3D     |
+--------------+--------+
|2 giorni 4 ore|P2DT4H  |
+--------------+--------+

 

Le durate iniziano con una P maiuscola seguita dal numero e dal relativo designatore, formalmente: P [n] Y [n] M [n] DT [n] H [n] M [n] S, dove Y è per anni, M per mesi ecc. Si noti che i periodi e le ore sono separati da una T maiuscola che disambigura anche M come mese (P2M significa 2 mesi) o minuto (PT2M significa 2 minuti). Le durate possono anche essere definite come un numero di settimane, quindi P4W significa 4 settimane. Una spiegazione completa è fornita nella pagina di Wikipedia\ [#F5]_\  che fa riferimento allo standard ISO ufficiale

 

Questo approccio è coerente sia con schema.org che con il W3C OWL Time Ontology.

 

+---------------------+------------------+-------------+-------------+
|\ |STYLE91|\         |\ |STYLE92|\      |\ |STYLE93|\ |\ |STYLE94|\ |
+---------------------+------------------+-------------+-------------+
|tempo di elaborazione|cv: ProcessingTime|Testo        |0..1         |
+---------------------+------------------+-------------+-------------+

.. _h6812691461174d238116b5049602f5:

3.2.24. Ha un costo
-------------------

La proprietà Has Cost collega un servizio pubblico a una o più istanze della classe di costo (vedere la sezione 3.11). Indica i costi relativi all'esecuzione di un servizio pubblico per il cittadino o l'attività commerciale relativa all'esecuzione di un particolare servizio pubblico. Laddove il costo varia in base al canale attraverso il quale si accede al servizio, può essere collegato al canale utilizzando la relazione If Accessed Through (sezione 3.11.6).

 

+-------------+-------------+-------------+-------------+
|\ |STYLE95|\ |\ |STYLE96|\ |\ |STYLE97|\ |\ |STYLE98|\ |
+-------------+-------------+-------------+-------------+
|hasCost      |cv: hasCost  |Costo        |0..n         |
+-------------+-------------+-------------+-------------+

.. _h114b1d727425622a1c216d7a734e385a:

3.2.25. È Descritto a      
---------------------------

La proprietà È Descritto in Proprietà collega un servizio pubblico al / ai set di dati del servizio pubblico (vedere 3.6) in cui viene descritto (vedere la sezione 3.6).

 

+-------------+-----------------+---------------------------------+--------------+
|\ |STYLE99|\ |\ |STYLE100|\    |\ |STYLE101|\                    |\ |STYLE102|\ |
+-------------+-----------------+---------------------------------+--------------+
|isDescribedAt|cv: isDescribedAt|Set di dati del servizio pubblico|0..n          |
+-------------+-----------------+---------------------------------+--------------+

.. _h15114371b7813dc5f121a4a13613b:

3.2.26. È classificato da
-------------------------

La proprietà Is Classified By consente di classificare il servizio pubblico con qualsiasi concetto (sezione 3.19), diverso da quelli già previsti e definiti esplicitamente nel CPSV-AP (area tematica, settore, ...). È una proprietà generica che può essere ulteriormente specializzata per rendere esplicita la classificazione, ad esempio per classificare i servizi pubblici in base al livello di digitalizzazione, al tipo di pubblico ...

 

Il Concetto è a sua volta collegato a una Collezione (sezione 3.20), che raggruppa i diversi concetti in un vocabolario controllato.

 

+--------------+------------------+--------------+--------------+
|\ |STYLE103|\ |\ |STYLE104|\     |\ |STYLE105|\ |\ |STYLE106|\ |
+--------------+------------------+--------------+--------------+
|isClassifiedBy|cv: isClassifiedBy|Concetto      |0..n          |
+--------------+------------------+--------------+--------------+

.. _h383c25767e673f341973534b613b7c4:

3.3. The Event Class
********************

This class represents an event that can be of any type that triggers, makes use of, or in some way is related to, a Public Service. It is not expected to be used directly, rather, one or other of its subclasses should be used. The properties of the class are, of course, inherited by those subclasses.

The Event class is used as a hook either to a single related Public Service, such as diagnosis of illness being related to application for sickness benefit (section 3.3.5); or to a group of Public Services, such as all those related to the establishment of a new business (see section 3.2.10).


+--------------+--------------+---+--------------+
|\ |STYLE107|\ |\ |STYLE108|\ |   |\ |STYLE109|\ |
+--------------+--------------+---+--------------+
|Event         |dct:identifier|   |URI           |
+--------------+--------------+---+--------------+

.. _h7775845515a4467507e1c21456152a:

3.3.1. Identifier
-----------------

This property represents an Identifier for the Event.


+--------------+--------------+--------------+--------------+
|\ |STYLE110|\ |\ |STYLE111|\ |\ |STYLE112|\ |\ |STYLE113|\ |
+--------------+--------------+--------------+--------------+
|Event         |dct:identifier|Text\ [#F7]_\ |1..1          |
+--------------+--------------+--------------+--------------+

.. _h74251854102827545a342f615d5947:

3.3.2. Name
-----------

This property represents the Name (or title) of the Event.


+--------------+--------------+--------------+--------------+
|\ |STYLE114|\ |\ |STYLE115|\ |\ |STYLE116|\ |\ |STYLE117|\ |
+--------------+--------------+--------------+--------------+
|name          |dct:title     |Text          |1..1          |
+--------------+--------------+--------------+--------------+

.. _h66220797d733267f5277f31381318:

3.3.3. Description
------------------

This property represents a free text description of the Event. The description is likely to be the text that a business or citizen sees for that specific Event when looking for relevant Public Services. Public administrations are therefore encouraged to include a reasonable level of detail in the description.


+--------------+---------------+--------------+--------------+
|\ |STYLE118|\ |\ |STYLE119|\  |\ |STYLE120|\ |\ |STYLE121|\ |
+--------------+---------------+--------------+--------------+
|description   |dct:description|Text          |0..1          |
+--------------+---------------+--------------+--------------+

.. _h2c204c5856282c56255c4f04a583215:

3.3.4. Type
-----------

The type property links an Event to a controlled vocabulary of event types and it is the nature of those controlled vocabularies that is the major difference between a business event, such as creating the business in the first place and a life event, such as the birth of a child.


+--------------+--------------+--------------+--------------+
|\ |STYLE122|\ |\ |STYLE123|\ |\ |STYLE124|\ |\ |STYLE125|\ |
+--------------+--------------+--------------+--------------+
|type          |dct:type      |concept       |0..n          |
+--------------+--------------+--------------+--------------+

.. _h4e274e22678346d1f80441237d6736:

3.3.5. Related Service
----------------------

This property links an event directly to a public service that is related to it.


+--------------+--------------+--------------+--------------+
|\ |STYLE126|\ |\ |STYLE127|\ |\ |STYLE128|\ |\ |STYLE129|\ |
+--------------+--------------+--------------+--------------+
|relatedService|dct:relation  |Public Service|0..n          |
+--------------+--------------+--------------+--------------+

.. _h7267416b5564e43236276d52474c6a:

3.4. La classe di eventi aziendali
**********************************

Questa classe rappresenta un evento aziendale, che è specializzato in eventi. Un evento aziendale è una situazione specifica o un evento nel ciclo di vita di un'azienda che soddisfa uno o più bisogni o obblighi (legali) di tale attività in questo specifico momento. Un Evento Aziendale richiede una serie di servizi pubblici da consegnare e consumare in modo da soddisfare le necessità aziendali o gli obblighi associati. Gli eventi aziendali sono definiti nel contesto di un determinato membro Stato .

 

In altre parole, un evento aziendale raggruppa una serie di servizi pubblici che devono essere consegnati per completare quel particolare evento.

 

+----------------+--------------+-----------------+
|\ |STYLE130|\   |\ |STYLE131|\ |\ |STYLE132|\    |
+----------------+--------------+-----------------+
|Evento aziendale|Opzionale     |cv: BusinessEvent|
+----------------+--------------+-----------------+

.. _h35e12466a55475e26669131b677653:

3.5. The Life Event Class
*************************

La classe Life Event rappresenta un evento o una situazione importante   nella vita di un cittadino in cui possono essere richiesti servizi pubblici. Nota lo scopo: un individuo incontrerà un numero qualsiasi di "eventi" nel senso generale del termine. Nel contesto di CPSV-AP, la classe Life Event rappresenta solo un evento a cui è collegato un servizio pubblico. Ad esempio, una coppia fidanzata non è un Evento di vita CPSV-AP, lo sposarsi è, poiché solo quest'ultimo ha rilevanza per i servizi pubblici.

 

+-----------------+--------------+--------------+
|\ |STYLE133|\    |\ |STYLE134|\ |\ |STYLE135|\ |
+-----------------+--------------+--------------+
|Evento della vita|Opzionale     |cv: LifeEvent |
+-----------------+--------------+--------------+

.. _h1f2363a4d1a1924c573a5f365715e:

3.6. La classe del set di dati del servizio pubblico
****************************************************

Il set di dati del servizio pubblico, è una specializzazione della classe Dataset del Vocabolario del catalogo dati (DCAT)\ [#F8]_\  e eredita tutte le sue proprietà. La classe descrive i metadati di dove viene descritto il set di dati, ad esempio su un portale di servizio pubblico regionale e / o su un portale nazionale di eGovernment.

 

+---------------------------------+--------------+------------------------+
|\ |STYLE136|\                    |\ |STYLE137|\ |\ |STYLE138|\           |
+---------------------------------+--------------+------------------------+
|Set di dati del servizio pubblico|Opzionale     |cv: PublicServiceDataset|
+---------------------------------+--------------+------------------------+

 

Le proprietà descritte nelle seguenti sezioni definiscono le proprietà obbligatorie se la classe viene istanziata. Ci riferiamo a DCAT per la definizione delle altre proprietà ereditate.

.. _h2c233b4a441997618115c70323651:

3.6.1. Identifier
-----------------

Questa proprietà rappresenta un identificatore per il set di dati del servizio pubblico.

 

+--------------+-------------------+---------------+--------------+
|\ |STYLE139|\ |\ |STYLE140|\      |\ |STYLE141|\  |\ |STYLE142|\ |
+--------------+-------------------+---------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F9]_\ |1..1          |
+--------------+-------------------+---------------+--------------+

.. _h19303ad605f59767e1e1835311c775f:

3.6.2. Editore
--------------

Questa proprietà rappresenta l'editore del set di dati del servizio pubblico, ovvero un'entità (organizzazione) responsabile della creazione del set di dati del servizio pubblico disponibile.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE143|\ |\ |STYLE144|\ |\ |STYLE145|\ |\ |STYLE146|\ |
+--------------+--------------+--------------+--------------+
|editore       |DCT: editore  |Agente        |1..1          |
+--------------+--------------+--------------+--------------+

.. _h60275c6299691470a7013194511c:

3.6.3. Nome
-----------

Questa proprietà contiene un nome assegnato al set di dati del servizio pubblico. Questa proprietà può essere ripetuta per versioni in lingua parallela del nome.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE147|\ |\ |STYLE148|\ |\ |STYLE149|\ |\ |STYLE150|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..n          |
+--------------+--------------+--------------+--------------+

.. _h13407d497b5c7a1d42d7737b511727:

3.6.4. Pagina di destinazione
-----------------------------

Questa proprietà fa riferimento a una pagina Web che fornisce l'accesso al set di dati del servizio pubblico. È inteso per indicare una pagina di destinazione presso il fornitore di dati originale, non su una pagina di un sito di terzi, come un aggregatore.

 

+----------------------+-----------------+--------------+--------------+
|\ |STYLE151|\         |\ |STYLE152|\    |\ |STYLE153|\ |\ |STYLE154|\ |
+----------------------+-----------------+--------------+--------------+
|pagina di destinazione|DCAT: Landingpage|Documento     |1..n          |
+----------------------+-----------------+--------------+--------------+

 

 

.. _h7823527fd4930242a4a4b38e5e5777:

3.7. La classe di partecipazione
********************************

Il CPSV-AP riconosce un ruolo comune connesso ai servizi pubblici, ovvero l'autorità competente (sezione 3.2.14). Tuttavia, questa semplice struttura non consente di formulare dichiarazioni su tali partecipanti, come la data di inizio e di fine di un contratto, né supporta l'inclusione di altri ruoli. La classe di partecipazione supporta questa complessità aggiuntiva se richiesta, ad esempio, la descrizione di un utente del servizio o di un fornitore di servizi. Il modello è coerente con il CPOV che a sua volta si basa sull'ontologia dell'organizzazione W3C che supporta semplicemente i casi comuni, ma consente i casi complessi ove necessario. La classe di partecipazione può essere associata alla classe Membership dell'Organizzazione Ontologia che consente di applicare relazioni più complesse e metadati più ricchi a un ruolo occupato da un determinato agente.

 

+--------------+--------------+------------------+
|\ |STYLE155|\ |\ |STYLE156|\ |\ |STYLE157|\     |
+--------------+--------------+------------------+
|Partecipazione|Opzionale     |cv: Partecipazione|
+--------------+--------------+------------------+

 

\ |STYLE158|\            \ |STYLE159|\ 

Questa proprietà rappresenta un identificatore per la partecipazione.

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE160|\ |\ |STYLE161|\      |\ |STYLE162|\    |\ |STYLE163|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F10]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h13713867743c3f56716926a6a142738:

3.7.2. Descrizione
------------------

Una descrizione testuale libera della partecipazione.

 

+--------------+----------------+--------------+--------------+
|\ |STYLE164|\ |\ |STYLE165|\   |\ |STYLE166|\ |\ |STYLE167|\ |
+--------------+----------------+--------------+--------------+
|descrizione   |DCT: Descrizione|Testo         |1..1          |
+--------------+----------------+--------------+--------------+

.. _h201d203a3e74f1e41357264d2d4b4:

3.7.3. Ruolo
------------

Fornisce il ruolo svolto. Questo dovrebbe essere fornito usando un vocabolario controllato. Poiché questo è un meccanismo di estensione per CSPV-AP, il vocabolario controllato dovrebbe essere deciso per adattarsi alle implementazioni locali.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE168|\ |\ |STYLE169|\ |\ |STYLE170|\ |\ |STYLE171|\ |
+--------------+--------------+--------------+--------------+
|ruolo         |cv: ruolo     |Concetto      |1..n          |
+--------------+--------------+--------------+--------------+

 

.. _h4a207bb71171c7c366a7710621f201c:

3.8. La classe di requisiti per il criterio
*******************************************

Non tutti i servizi pubblici sono necessari o utilizzabili da tutti. Ad esempio, il servizio di visto gestito da paesi europei non è necessario per i cittadini europei, ma è richiesto da alcuni cittadini di altri paesi, oppure i servizi pubblici che offrono sussidi di disoccupazione e le sovvenzioni si rivolgono a specifici gruppi sociali. Il CPSV riutilizza il Vocabolario del Core Criterion e del Core Evidence\ [#F11]_\  per questa classe. CCCEV fornisce ulteriori dettagli ma la classe Requisito criterio ha tre proprietà obbligatorie.

 

+---------------------+--------------+------------------------+
|\ |STYLE172|\        |\ |STYLE173|\ |\ |STYLE174|\           |
+---------------------+--------------+------------------------+
|Criterio obbligatorio|Opzionale     |cv: CriterionRequirement|
+---------------------+--------------+------------------------+

 

.. _h45793a60115d7a285856a4a4638531a:

3.8.1. Identifier
-----------------

Questa proprietà rappresenta un identificatore per il criterio di criterio .

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE175|\ |\ |STYLE176|\      |\ |STYLE177|\    |\ |STYLE178|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F12]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h6c4a3e56324b2d76582c7c8322f7572:

3.8.2. Nome
-----------

Questa proprietà rappresenta il nome ufficiale del criterio di criterio .

 

+--------------+--------------+--------------+--------------+
|\ |STYLE179|\ |\ |STYLE180|\ |\ |STYLE181|\ |\ |STYLE182|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..1          |
+--------------+--------------+--------------+--------------+

.. _h29386738243b495b6c1f7a116b54207:

3.8.3. genere
-------------

Questa proprietà rappresenta il tipo di criterio richiesto come descritto in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE183|\ |\ |STYLE184|\ |\ |STYLE185|\ |\ |STYLE186|\ |
+--------------+--------------+--------------+--------------+
|genere        |DCT: Tipo     |Concetto      |0..n          |
+--------------+--------------+--------------+--------------+

 

.. _h697a48716c5e4c577a633146235f96f:

3.9. La classe di prova
***********************

La classe Evidence è definita nel vocabolario Core Criterion e Core Evidence (CCCEV) come qualsiasi risorsa in grado di documentare o supportare una risposta di criterio. Contiene informazioni che dimostrano che un requisito di criterio esiste o è vero, in particolare sono utilizzate evidenze per dimostrare che un criterio specifico è soddisfatto.

 

Sebbene la formulazione della definizione sia diversa, la semantica corrisponde esattamente alla classe Input di CPSV che sostituisce.

 

Le prove possono essere qualsiasi risorsa - documento, artefatto - qualsiasi cosa necessaria per l'esecuzione del servizio pubblico. Nel contesto dei servizi pubblici, la prova è solitamente documenti amministrativi o moduli di domanda compilati. Un servizio pubblico specifico può richiedere la presenza di determinate prove o combinazioni di prove per essere consegnato.

 

In alcuni casi, l'output di un servizio sarà Evidence per un altro servizio. Tali relazioni dovrebbero essere descritte nelle regole associate.

 

+--------------+--------------+--------------+
|\ |STYLE187|\ |\ |STYLE188|\ |\ |STYLE189|\ |
+--------------+--------------+--------------+
|Prova         |Opzionale     |cv: Evidence  |
+--------------+--------------+--------------+

.. _h69272261e55e17434b502b686b5814:

3.9.1. Identifier
-----------------

Questa proprietà rappresenta un identificatore per il pezzo di prova.

 

+--------------+-------------------+----------------+--------------+
|\ |STYLE190|\ |\ |STYLE191|\      |\ |STYLE192|\   |\ |STYLE193|\ |
+--------------+-------------------+----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F13]_\ |1..1          |
+--------------+-------------------+----------------+--------------+

.. _h531136505057514e2d7c70145c504b4d:

3.9.2. Nome
-----------

Questa proprietà rappresenta il nome ufficiale del pezzo di prova.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE194|\ |\ |STYLE195|\ |\ |STYLE196|\ |\ |STYLE197|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..1          |
+--------------+--------------+--------------+--------------+

.. _h79c2919343762457347e6d323ac73:

3.9.3. Descrizione
------------------

Questa proprietà rappresenta un testo libero Descrizione dell'elemento di prova.

 

+--------------+----------------+--------------+--------------+
|\ |STYLE198|\ |\ |STYLE199|\   |\ |STYLE200|\ |\ |STYLE201|\ |
+--------------+----------------+--------------+--------------+
|descrizione   |DCT: Descrizione|Testo         |0..1          |
+--------------+----------------+--------------+--------------+

.. _h7c552a3131263954182e782f62706c2a:

3.9.4. genere
-------------

Questa proprietà rappresenta il tipo di Evidenza come descritto in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+--------------+--------------+--------------+--------------+
|\ |STYLE202|\ |\ |STYLE203|\ |\ |STYLE204|\ |\ |STYLE205|\ |
+--------------+--------------+--------------+--------------+
|genere        |DCT: Tipo     |Concetto      |0..1          |
+--------------+--------------+--------------+--------------+

.. _h465127f6a647e32656b40523043168:

3.9.5. Documentazione correlata
-------------------------------

Questa proprietà rappresenta la documentazione che contiene informazioni relative all'Evidenza, ad esempio un modello particolare per un documento amministrativo, un'applicazione o una guida sulla formattazione dell'input.

 

+-----------------------+--------------+--------------+--------------+
|\ |STYLE206|\          |\ |STYLE207|\ |\ |STYLE208|\ |\ |STYLE209|\ |
+-----------------------+--------------+--------------+--------------+
|Documentazionecorrelata|foaf: Pagina  |Documento     |0..n          |
+-----------------------+--------------+--------------+--------------+

.. _h347b0dc7b325e622810f653f443f:

3.9.6. Linguaggio
-----------------

Indica la / e lingua / e in cui deve essere fornita la prova.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE210|\ |\ |STYLE211|\ |\ |STYLE212|\ |\ |STYLE213|\ |
+--------------+--------------+--------------+--------------+
|linguaggio    |DCT: lingua   |Concetto      |0..n          |
+--------------+--------------+--------------+--------------+

.. _h67104b5d7b20372542555d4a50417c4d:

3.10. La classe di output
*************************

I risultati possono essere qualsiasi risorsa - documento, artefatto - qualsiasi cosa prodotta dal servizio pubblico. Nel contesto di un servizio pubblico, l'output fornisce un documento ufficiale o altro artefatto dell'autorità competente ( organizzazione pubblica ) che consente / autorizza / autorizza un agente a (fare) qualcosa.

 

In alcuni casi, l'output di un servizio pubblico sarà utilizzato come prova per soddisfare un requisito di criterio di un altro servizio pubblico. Tali relazioni dovrebbero essere descritte nelle regole associate.

 

+--------------+--------------+--------------+
|\ |STYLE214|\ |\ |STYLE215|\ |\ |STYLE216|\ |
+--------------+--------------+--------------+
|Produzione    |Opzionale     |cv: Uscita    |
+--------------+--------------+--------------+

 

.. _h716639403252431c1b3541f444f341f:

3.10.1. Identifier
------------------

Questa proprietà rappresenta un identificatore per l'output.

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE217|\ |\ |STYLE218|\      |\ |STYLE219|\    |\ |STYLE220|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F14]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h5e2a40692d14651511eb7e4581580:

3.10.2. Nome
------------

Questa proprietà rappresenta il nome ufficiale dell'output.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE221|\ |\ |STYLE222|\ |\ |STYLE223|\ |\ |STYLE224|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..1          |
+--------------+--------------+--------------+--------------+

.. _h5c6d4e7651101e455675430157373:

3.10.3. Descrizione
-------------------

Questa proprietà rappresenta un testo libero Descrizione dell'output.

 

+--------------+----------------+--------------+--------------+
|\ |STYLE225|\ |\ |STYLE226|\   |\ |STYLE227|\ |\ |STYLE228|\ |
+--------------+----------------+--------------+--------------+
|descrizione   |DCT: Descrizione|Testo         |0..1          |
+--------------+----------------+--------------+--------------+

.. _h2e5207c11521e74214344327f206657:

3.10.4. Tipo
------------

Questa proprietà rappresenta il tipo di Output definito in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+--------------+--------------+--------------+--------------+
|\ |STYLE229|\ |\ |STYLE230|\ |\ |STYLE231|\ |\ |STYLE232|\ |
+--------------+--------------+--------------+--------------+
|tipo          |DCT: Tipo     |Concetto      |0..n          |
+--------------+--------------+--------------+--------------+

.. _h7048535b3d155645263b73c3c457a5:

3.11.   La classe di costo
**************************

La classe di costo rappresenta tutti i costi relativi all'esecuzione di un servizio pubblico che l'agente che consuma deve pagare.

 

+--------------+--------------+--------------+
|\ |STYLE233|\ |\ |STYLE234|\ |\ |STYLE235|\ |
+--------------+--------------+--------------+
|Costo         |Opzionale     |cv: Costo     |
+--------------+--------------+--------------+

 

.. _h727f443376557d38268052619522b4a:

3.11.1. Identifier
------------------

Questa proprietà rappresenta un identificatore per il costo.

+--------------+-------------------+-----------------+--------------+
|\ |STYLE236|\ |\ |STYLE237|\      |\ |STYLE238|\    |\ |STYLE239|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F15]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h535645645b675c494956a5f5f355466:

3.11.2. Valore
--------------

Questa proprietà rappresenta un valore numerico che indica l'importo del costo.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE240|\ |\ |STYLE241|\ |\ |STYLE242|\ |\ |STYLE243|\ |
+--------------+--------------+--------------+--------------+
|valore        |cv: Valore    |Numero        |0..1          |
+--------------+--------------+--------------+--------------+

.. _h35224b74766f3763e757d542be4e5c:

3.11.3. Moneta
--------------

Questa proprietà rappresenta la valuta in cui il costo deve essere pagato e il valore del costo è espresso. I valori possibili per questa proprietà sono descritti in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4 .

 

+--------------+--------------+--------------+--------------+
|\ |STYLE244|\ |\ |STYLE245|\ |\ |STYLE246|\ |\ |STYLE247|\ |
+--------------+--------------+--------------+--------------+
|moneta        |cv: Valuta    |Concetto      |0..1          |
+--------------+--------------+--------------+--------------+

.. _h6f7a5740436014741a15c791845507a:

3.11.4.           Descrizione
-----------------------------

Questa proprietà rappresenta una descrizione di testo libera del costo.

 

+--------------+----------------+--------------+--------------+
|\ |STYLE248|\ |\ |STYLE249|\   |\ |STYLE250|\ |\ |STYLE251|\ |
+--------------+----------------+--------------+--------------+
|descrizione   |DCT: Descrizione|Testo         |0..1          |
+--------------+----------------+--------------+--------------+

.. _h1d30462f305820271d51373d472c3c1a:

3.11.5. È definito da
---------------------

Questa proprietà l inchiostra la classe di costo con una o più istanze della classe Organizzazione pubblica (sezione 3.16). Questa proprietà indica quale Organizzazione pubblica è l'autorità competente per la definizione dei costi associati alla consegna di un particolare servizio pubblico.

 

+--------------+---------------+------------------+--------------+
|\ |STYLE252|\ |\ |STYLE253|\  |\ |STYLE254|\     |\ |STYLE255|\ |
+--------------+---------------+------------------+--------------+
|isDefinedBy   |cv: isDefinedBy|PublicOrganisation|0..n          |
+--------------+---------------+------------------+--------------+

.. _h5325564b7a1d7987e6e4c3b6617454a:

3.11.6. Se accessibile
----------------------

Dove il costo varia a seconda del canale utilizzato, ad esempio, se l'accesso avviene tramite un servizio online cf. accesso in una posizione fisica, il costo può essere collegato al canale utilizzando la proprietà If Accessed Through.

 

+-----------------+---------------------+--------------+--------------+
|\ |STYLE256|\    |\ |STYLE257|\        |\ |STYLE258|\ |\ |STYLE259|\ |
+-----------------+---------------------+--------------+--------------+
|ifAccessedThrough|cv: ifAccessedThrough|Canale        |0..1          |
+-----------------+---------------------+--------------+--------------+

 

.. _h2a2b3684da150562e6495073113a:

3.12. La classe del canale
**************************

La classe Channel rappresenta il mezzo attraverso il quale un agente fornisce, utilizza o interagisce in un altro modo con un servizio pubblico. Esempi tipici includono servizi online, telefono, centri di accoglienza ecc.

 

+--------------+--------------+--------------+
|\ |STYLE260|\ |\ |STYLE261|\ |\ |STYLE262|\ |
+--------------+--------------+--------------+
|Canale        |Opzionale     |cv: Canale    |
+--------------+--------------+--------------+

 

.. _h2223c6472141b2079301d633a50537f:

3.12.1. Identifier
------------------

Questa proprietà rappresenta un identificatore per il canale.

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE263|\ |\ |STYLE264|\      |\ |STYLE265|\    |\ |STYLE266|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo \ |LINK3|\ |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h4245fd163f3e2f624c4d6e521820a:

3.12.2. Posseduto da
--------------------

Questa proprietà esegue l'inchiostrazione della classe Channel con una o più istanze della classe Agent (sezione 3.15). Questa proprietà indica il proprietario di un canale specifico attraverso il quale viene consegnato un servizio pubblico. Si noti che l'organizzazione pubblica è una sottoclasse di agente in modo che se il proprietario è l'organizzazione pubblica , la proprietà OwnBy può collegarsi ad essa.

 

+--------------+--------------+-----------------------+--------------+
|\ |STYLE267|\ |\ |STYLE268|\ |\ |STYLE269|\          |\ |STYLE270|\ |
+--------------+--------------+-----------------------+--------------+
|posseduto da  |cv: ownedBy   |Organizzazione pubblica|0..n          |
+--------------+--------------+-----------------------+--------------+

.. _h674d3d6f31272a7d251b797446471020:

3.12.3. Genere
--------------

Questa proprietà rappresenta il tipo di canale definito in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE271|\ |\ |STYLE272|\ |\ |STYLE273|\ |\ |STYLE274|\ |
+--------------+--------------+--------------+--------------+
|genere        |DCT: Tipo     |Concetto      |0..1          |
+--------------+--------------+--------------+--------------+

.. _h6a7a2931571a4f3a491f47537e451449:

3.12.4. Ha Input
----------------

Nella maggior parte dei casi, le prove richieste per utilizzare un servizio pubblico saranno indipendenti dal canale attraverso il quale si accede al servizio. La proprietà Has Input dovrebbe essere normalmente utilizzata per collegare un servizio pubblico direttamente a uno o più elementi di Evidence (vedere la sezione 3.9). Tuttavia, laddove il tipo di Evidenza richiesto varia in base al canale utilizzato per accedere al Servizio Pubblico, la proprietà Has Input può essere utilizzata a livello di Canale.Ad esempio, potrebbe essere richiesta una firma digitale per un canale online, mentre potrebbe essere richiesta una firma fisica per una fornitura di servizi faccia a faccia.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE275|\ |\ |STYLE276|\ |\ |STYLE277|\ |\ |STYLE278|\ |
+--------------+--------------+--------------+--------------+
|hasInput      |CPsV: hasInput|Prova         |0..n          |
+--------------+--------------+--------------+--------------+

.. _h227873159736262125e51591a544942:

3.12.5. Orari di apertura
-------------------------

Questa proprietà rappresenta i normali orari di apertura di un canale. Il valore dovrebbe seguire il formato flessibile definito per la proprietà degli orari di apertura di schema.org\ [#F16]_\ . Seguendo questa struttura, i giorni della settimana sono rappresentati da due codici lettera (Mo, Tu, We, Th, Fr, Sa, Su). Le liste devono essere separate da una virgola (ad esempio: Mo, We, Fr) e periodi separati da un trattino (ad esempio: Mo-Fr).

 

Se è opportuno aggiungere ore di apertura, questo segue il giorno quindi se un servizio telefonico è disponibile dalle 08:00 alle 20:00 dal lunedì al sabato e dalle 08:00 alle 18:00 la domenica che sarà codificata come Mo-Sa 08: 00-20: 00, Su 08: 00-18: 00.

 

+-----------------+--------------------+--------------+--------------+
|\ |STYLE279|\    |\ |STYLE280|\       |\ |STYLE281|\ |\ |STYLE282|\ |
+-----------------+--------------------+--------------+--------------+
|orari di apertura|Schema: openingHours|Testo         |0..n          |
+-----------------+--------------------+--------------+--------------+

 

.. _h217e4e34775e634a261d168321b5b79:

3.12.6. Restrizione di disponibilità
------------------------------------

Questa proprietà collega un canale a informazioni su quando il canale non è disponibile, ignorando le informazioni generali sull'orario di apertura ( 3.12.5). I dettagli sono forniti utilizzando la classe Specificazione ore di apertura (sezione 3.13).

 

+-----------------------+----------------------+------------------------------------+--------------+
|\ |STYLE283|\          |\ |STYLE284|\         |\ |STYLE285|\                       |\ |STYLE286|\ |
+-----------------------+----------------------+------------------------------------+--------------+
|availabilityRestriction|schema: hoursAvailable|Specificazione delle ore di apertura|0..1          |
+-----------------------+----------------------+------------------------------------+--------------+

 

.. _h2e1e4f582339a4e6d5d2c37651f2842:

3.13. La classe di specificazione delle ore di apertura
*******************************************************

Il CPSV-AP utilizza la proprietà openingHours di schema.org (sezione 3.12.5 ) per fornire dettagli sulle operazioni regolari. La specifica delle ore di apertura\ [#F17]_\ . La classe può essere utilizzata per fornire dettagli su circostanze eccezionali, come la chiusura nei giorni festivi, che è codificata (in Turtle), quindi:

ex: PublicHolidayClosed a schema: OpeningHoursSpecification;

schema: dayOfWeek <http://schema.org/PublicHoliday>.

 

Si noti che lo schema di proprietà: opens non viene utilizzato, quindi il punto di contatto è chiuso. È possibile indicare chiusure più specifiche includendo lo schema: validFrom e schema: proprietà validThrough, ad esempio:

 

ex: ChristmasClosed a schema: OpeningHoursSpecification;

schema: validFrom "2016-12-24T012: 00Z";

schema: validThrough "2017-01-02T09: 00Z".

 

+-----------------+--------------+---------------------------------+
|\ |STYLE287|\    |\ |STYLE288|\ |\ |STYLE289|\                    |
+-----------------+--------------+---------------------------------+
|orari di apertura|Opzionale     |schema: OpeningHoursSpecification|
+-----------------+--------------+---------------------------------+

.. _h178141d7b4d1d5b6f6921717d75e:

3.14. La classe regola
**********************

La classe Rule rappresenta un documento che definisce le regole, le linee guida o le procedure specifiche seguite dal Servizio pubblico. Comprende i termini di servizio, licenza e requisiti di autenticazione del servizio pubblico.

 

Le istanze della classe Rule sono espressioni FRBR, cioè un'espressione concreta come un documento, del concetto più astratto delle regole stesse. Il CPSV-AP non prevede istanze della classe Rule come regole di business leggibili dalla macchina.

 

La modellazione dettagliata delle regole relative ai servizi pubblici non rientra negli obiettivi di CPSV-AP.

 

+--------------+--------------+--------------+
|\ |STYLE290|\ |\ |STYLE291|\ |\ |STYLE292|\ |
+--------------+--------------+--------------+
|Regola        |Opzionale     |CPsV: Regola  |
+--------------+--------------+--------------+

 

.. _h655a2e12481d3a6365045265753f4c:

3.14.1.  Identifier
-------------------

Questa proprietà rappresenta un identificatore per la regola.

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE293|\ |\ |STYLE294|\      |\ |STYLE295|\    |\ |STYLE296|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F18]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

 

.. _h522243f715634286c355c5f461e11:

3.14.2. Descrizione
-------------------

Questa proprietà rappresenta un testo libero Descrizione della regola.

 

+--------------+----------------+--------------+--------------+
|\ |STYLE297|\ |\ |STYLE298|\   |\ |STYLE299|\ |\ |STYLE300|\ |
+--------------+----------------+--------------+--------------+
|descrizione   |DCT: Descrizione|Testo         |1..1          |
+--------------+----------------+--------------+--------------+

.. _h304c2f2f6e637f615312b631b1a6029:

3.14.3. Linguaggio
------------------

Questa proprietà rappresenta la lingua / le lingue in cui è disponibile la regola. Potrebbe trattarsi di una o più lingue, ad esempio in paesi con più di una lingua ufficiale. I valori possibili per questa proprietà sono descritti in un vocabolario controllato. I vocabolari controllati raccomandati sono elencati nella sezione 4.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE301|\ |\ |STYLE302|\ |\ |STYLE303|\ |\ |STYLE304|\ |
+--------------+--------------+--------------+--------------+
|linguaggio    |DCT: lingua   |Concetto      |0..n          |
+--------------+--------------+--------------+--------------+

.. _h4a1e69793d147340a7539761674196:

3.14.4. Nome
------------

Questa proprietà rappresenta il nome della regola.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE305|\ |\ |STYLE306|\ |\ |STYLE307|\ |\ |STYLE308|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..1          |
+--------------+--------------+--------------+--------------+

.. _h644634173252ce125f2d7f1512e1f:

3.14.5. Implementa
------------------

La proprietà Implementa collega una Regola alla legislazione o ai documenti politici pertinenti, ovvero la Risorsa Legale in base alla quale vengono definite le Regole (vedere la sezione 3.16).

 

+--------------+--------------+-----------------+--------------+
|\ |STYLE309|\ |\ |STYLE310|\ |\ |STYLE311|\    |\ |STYLE312|\ |
+--------------+--------------+-----------------+--------------+
|attrezzi      |CPsV: attrezzi|Servizio pubblico|0..n          |
+--------------+--------------+-----------------+--------------+

 

.. _h75261d2612653e6d493b276a19601a47:

3.15. La classe dell'agente
***************************

La classe Agent è qualsiasi risorsa che agisce o ha il potere di agire. Questo include persone, organizzazioni e gruppi. La classe Public Organization , definita nel Vocabolario Core Public Organization , è una sottoclasse notevole di Agent.

 

+--------------+--------------+--------------+
|\ |STYLE313|\ |\ |STYLE314|\ |\ |STYLE315|\ |
+--------------+--------------+--------------+
|Agente        |Opzionale     |DCT: Agente   |
+--------------+--------------+--------------+

 

.. _h624fb7673769554056353f1224303d:

3.15.1. Nome
------------

Questa proprietà rappresenta il nome dell'agente.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE316|\ |\ |STYLE317|\ |\ |STYLE318|\ |\ |STYLE319|\ |
+--------------+--------------+--------------+--------------+
|nome          |DCT: titolo   |Testo         |1..1          |
+--------------+--------------+--------------+--------------+

.. _h447b5f32321d3b551e5447b7e31047:

3.15.2. Identifier
------------------

Questa proprietà rappresenta un identificatore per l'agente.

 

+--------------+-------------------+-----------------+--------------+
|\ |STYLE320|\ |\ |STYLE321|\      |\ |STYLE322|\    |\ |STYLE323|\ |
+--------------+-------------------+-----------------+--------------+
|identificatore|DCT: identificatore|Testo\ [#F19]_\  |1..1          |
+--------------+-------------------+-----------------+--------------+

.. _h4d7576676f7e3d7c36151756e5a3ff:

3.15.3. Gioca il ruolo
----------------------

Questa proprietà collega un agente alla classe di partecipazione. La classe di partecipazione è definita nella sezione 3.6 e facilita la descrizione dettagliata di come un agente partecipa o interagisce con un servizio pubblico e può includere vincoli temporali e spaziali su tale partecipazione.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE324|\ |\ |STYLE325|\ |\ |STYLE326|\ |\ |STYLE327|\ |
+--------------+--------------+--------------+--------------+
|playsRole     |cv: playsRole |Partecipazione|0..n          |
+--------------+--------------+--------------+--------------+

.. _h3d7c504f101624575b2051334ce224d:

3.15.4.  Ha un indirizzo
------------------------

Questa proprietà rappresenta un n indirizzo relativo a un agente. L'affermazione della relazione di indirizzo implica che l'agente abbia un indirizzo.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE328|\ |\ |STYLE329|\ |\ |STYLE330|\ |\ |STYLE331|\ |
+--------------+--------------+--------------+--------------+
|hasAddress    |cv: hasAddress|Indirizzo     |0..1          |
+--------------+--------------+--------------+--------------+

 

.. _h6f3f6a76f485d195e4a32635f671c1d:

3.16. La classe di risorse legali
*********************************

Questa classe rappresenta la legislazione, la politica o le politiche che si celano dietro le Regole che regolano il servizio.

 

La definizione e le proprietà della classe di risorse legali nel CPSV-AP sono allineate con l'ontologia inclusa in "Conclusioni del Consiglio che invitano l'introduzione dell'identificatore della legislazione europea (ELI)"\ [#F20]_\ .

 

Per descrivere gli attributi di una risorsa legale (etichette, etichette preferite, etichette alternative, definizione ...) ci riferiamo all'ontologia ELI.

 

+--------------+--------------+------------------+
|\ |STYLE332|\ |\ |STYLE333|\ |\ |STYLE334|\     |
+--------------+--------------+------------------+
|Risorsa legale|Opzionale     |eli: LegalResource|
+--------------+--------------+------------------+

.. _h514f13716c367534297f4622485a27f:

3.16.1. Relazionato
-------------------

Questa proprietà rappresenta un'altra istanza della classe di risorse legali correlata alla particolare risorsa legale descritta.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE335|\ |\ |STYLE336|\ |\ |STYLE337|\ |\ |STYLE338|\ |
+--------------+--------------+--------------+--------------+
|Relazionato   |DCT: relazione|Risorsa legale|0..n          |
+--------------+--------------+--------------+--------------+

 

.. _h441c404b67e1c747872b213b2316:

3.17. La classe di organizzazione pubblica
******************************************

Il CPSV-AP riutilizza il Vocabolario Core Public Organization\ [#F21]_\  che definisce il concetto di organizzazione pubblica e proprietà e relazioni associate. Si basa in gran parte sull'ontologia dell'organizzazione W3C

 

+-----------------------+--------------+----------------------+
|\ |STYLE339|\          |\ |STYLE340|\ |\ |STYLE341|\         |
+-----------------------+--------------+----------------------+
|Organizzazione pubblica|Obbligatorio  |cv: PublicOrganisation|
+-----------------------+--------------+----------------------+

 

All'interno di CPSV-AP sono obbligatorie le seguenti proprietà:

* etichetta preferita

* spaziale

Il valore di quest'ultimo dovrebbe essere un URI delle Unità territoriali amministrative\ [#F23]_\  Elenco delle autorità denominate gestite dal registro dei metadati dell'Ufficio delle pubblicazioni.

 

+--------------+---------------+--------------+--------------+
|\ |STYLE342|\ |\ |STYLE343|\  |\ |STYLE344|\ |\ |STYLE345|\ |
+--------------+---------------+--------------+--------------+
|preferredLabel|skos: prefLabel|Testo         |1..1          |
+--------------+---------------+--------------+--------------+
|spaziale      |DCT: spaziale  |Concetto      |1..1          |
+--------------+---------------+--------------+--------------+

 

.. _h6f292043b16592a6767397b21492443:

3.18. La classe del punto di contatto
*************************************

Questa classe rappresenta le informazioni di contatto per un servizio pubblico, canale, organizzazione pubblica , ecc. È definita nel vocabolario Core Public Organization e viene fornita come schema: Contact Point . Come il canale, un punto di contatto può avere orari di apertura regolari (sezione 3.12.5) che vengono quindi sostituiti, ad esempio, dalle festività pubbliche, utilizzando la classe di specifica Orari di apertura (sezione 3.13).

 

+-----------------+--------------+--------------------+
|\ |STYLE346|\    |\ |STYLE347|\ |\ |STYLE348|\       |
+-----------------+--------------+--------------------+
|Punto di contatto|Opzionale     |schema: ContactPoint|
+-----------------+--------------+--------------------+

 

.. _h61447126c1e6f4466115919716d60:

3.19. La classe di conformità
*****************************

Questa classe rappresenta qualsiasi concetto che possa essere utilizzato per classificare il servizio pubblico e che si riferisce al servizio pubblico attraverso la proprietà è classificato da (sezione 3.2.26). Questa classe è stata aggiunta in CPSV-AP per integrare la necessità di aggiungere altri metodi di classificazione del servizio pubblico, che non sono stati definiti in modo esplicito in CPSV-AP.

 

In questo contesto, il CPSV-AP riutilizza il Concetto\ [#F24]_\  classe come definita nel sistema di organizzazione della conoscenza semplice SKOS

 

Il Concetto può o non può appartenere a (membro) una certa Collezione (sezione 3.20).

 

+--------------+--------------+--------------+
|\ |STYLE349|\ |\ |STYLE350|\ |\ |STYLE351|\ |
+--------------+--------------+--------------+
|Concetto      |Opzionale     |SKOS: Concetto|
+--------------+--------------+--------------+

 

.. _h7f57314f7675a7646397e6983b2159:

3.20. La classe di raccolta
***************************

Questa classe rappresenta la Collezione a cui appartiene un Concetto (sezione 3.19 ). Raggruppare concetti diversi definisce un vocabolario controllato.

 

In questo contesto, il CPSV-AP riutilizza la Collezione\ [#F26]_\  classe come definita nel sistema di organizzazione della conoscenza semplice SKOS

 

 

+--------------+--------------+----------------+
|\ |STYLE352|\ |\ |STYLE353|\ |\ |STYLE354|\   |
+--------------+--------------+----------------+
|Collezione    |Opzionale     |SKOS: Collection|
+--------------+--------------+----------------+

 

.. _h7d5d155847c7d2ce4a36186437a7d:

3.20.1. Membro
--------------

La proprietà Member , come definita in SKOS, consente di indicare i concetti (sezione 3.19) che fanno parte di una raccolta.

 

+--------------+--------------+--------------+--------------+
|\ |STYLE355|\ |\ |STYLE356|\ |\ |STYLE357|\ |\ |STYLE358|\ |
+--------------+--------------+--------------+--------------+
|Membro        |SKOS: membro  |Concetto      |0..n          |
+--------------+--------------+--------------+--------------+

 


.. bottom of content


.. |STYLE0| replace:: **Nome della classe**

.. |STYLE1| replace:: **Obbligatorio / facoltativo**

.. |STYLE2| replace:: **URI**

.. |STYLE3| replace:: **Proprietà**

.. |STYLE4| replace:: **URI**

.. |STYLE5| replace:: **Gamma**

.. |STYLE6| replace:: **Cardinalità**

.. |STYLE7| replace:: **Proprietà**

.. |STYLE8| replace:: **URI**

.. |STYLE9| replace:: **Gamma**

.. |STYLE10| replace:: **Cardinalità**

.. |STYLE11| replace:: **Proprietà**

.. |STYLE12| replace:: **URI**

.. |STYLE13| replace:: **Gamma**

.. |STYLE14| replace:: **Cardinalità**

.. |STYLE15| replace:: **Proprietà**

.. |STYLE16| replace:: **URI**

.. |STYLE17| replace:: **Gamma**

.. |STYLE18| replace:: **Cardinalità**

.. |STYLE19| replace:: **Proprietà**

.. |STYLE20| replace:: **URI**

.. |STYLE21| replace:: **Gamma**

.. |STYLE22| replace:: **Cardinalità**

.. |STYLE23| replace:: **Proprietà**

.. |STYLE24| replace:: **URI**

.. |STYLE25| replace:: **Gamma**

.. |STYLE26| replace:: **Cardinalità**

.. |STYLE27| replace:: **Proprietà**

.. |STYLE28| replace:: **URI**

.. |STYLE29| replace:: **Gamma**

.. |STYLE30| replace:: **Cardinalità**

.. |STYLE31| replace:: **Proprietà**

.. |STYLE32| replace:: **URI**

.. |STYLE33| replace:: **Gamma**

.. |STYLE34| replace:: **Cardinalità**

.. |STYLE35| replace:: **Proprietà**

.. |STYLE36| replace:: **URI**

.. |STYLE37| replace:: **Gamma**

.. |STYLE38| replace:: **Cardinalità**

.. |STYLE39| replace:: **Proprietà**

.. |STYLE40| replace:: **URI**

.. |STYLE41| replace:: **Gamma**

.. |STYLE42| replace:: **Cardinalità**

.. |STYLE43| replace:: **Proprietà**

.. |STYLE44| replace:: **URI**

.. |STYLE45| replace:: **Gamma**

.. |STYLE46| replace:: **Cardinalità**

.. |STYLE47| replace:: **Proprietà**

.. |STYLE48| replace:: **URI**

.. |STYLE49| replace:: **Gamma**

.. |STYLE50| replace:: **Cardinalità**

.. |STYLE51| replace:: **Proprietà**

.. |STYLE52| replace:: **URI**

.. |STYLE53| replace:: **Gamma**

.. |STYLE54| replace:: **Cardinalità**

.. |STYLE55| replace:: **Proprietà**

.. |STYLE56| replace:: **URI**

.. |STYLE57| replace:: **Gamma**

.. |STYLE58| replace:: **Cardinalità**

.. |STYLE59| replace:: **Proprietà**

.. |STYLE60| replace:: **URI**

.. |STYLE61| replace:: **Gamma**

.. |STYLE62| replace:: **Cardinalità**

.. |STYLE63| replace:: **Proprietà**

.. |STYLE64| replace:: **URI**

.. |STYLE65| replace:: **Gamma**

.. |STYLE66| replace:: **Cardinalità**

.. |STYLE67| replace:: **Proprietà**

.. |STYLE68| replace:: **URI**

.. |STYLE69| replace:: **Gamma**

.. |STYLE70| replace:: **Cardinalità**

.. |STYLE71| replace:: **Proprietà**

.. |STYLE72| replace:: **URI**

.. |STYLE73| replace:: **Gamma**

.. |STYLE74| replace:: **Cardinalità**

.. |STYLE75| replace:: **Proprietà**

.. |STYLE76| replace:: **URI**

.. |STYLE77| replace:: **Gamma**

.. |STYLE78| replace:: **Cardinalità**

.. |STYLE79| replace:: **Proprietà**

.. |STYLE80| replace:: **URI**

.. |STYLE81| replace:: **Gamma**

.. |STYLE82| replace:: **Cardinalità**

.. |STYLE83| replace:: **Proprietà**

.. |STYLE84| replace:: **URI**

.. |STYLE85| replace:: **Gamma**

.. |STYLE86| replace:: **Cardinalità**

.. |STYLE87| replace:: **Proprietà**

.. |STYLE88| replace:: **URI**

.. |STYLE89| replace:: **Gamma**

.. |STYLE90| replace:: **Cardinalità**

.. |STYLE91| replace:: **Proprietà**

.. |STYLE92| replace:: **URI**

.. |STYLE93| replace:: **Gamma**

.. |STYLE94| replace:: **Cardinalità**

.. |STYLE95| replace:: **Proprietà**

.. |STYLE96| replace:: **URI**

.. |STYLE97| replace:: **Gamma**

.. |STYLE98| replace:: **Cardinalità**

.. |STYLE99| replace:: **Proprietà**

.. |STYLE100| replace:: **URI**

.. |STYLE101| replace:: **Gamma**

.. |STYLE102| replace:: **Cardinalità**

.. |STYLE103| replace:: **Proprietà**

.. |STYLE104| replace:: **URI**

.. |STYLE105| replace:: **Gamma**

.. |STYLE106| replace:: **Cardinalità**

.. |STYLE107| replace:: **Proprietà**

.. |STYLE108| replace:: **Mandatory/Optional**

.. |STYLE109| replace:: **URI**

.. |STYLE110| replace:: **Proprietà**

.. |STYLE111| replace:: **URI**

.. |STYLE112| replace:: **Gamma**

.. |STYLE113| replace:: **Cardinalità**

.. |STYLE114| replace:: **Proprietà**

.. |STYLE115| replace:: **URI**

.. |STYLE116| replace:: **Gamma**

.. |STYLE117| replace:: **Cardinalità**

.. |STYLE118| replace:: **Proprietà**

.. |STYLE119| replace:: **URI**

.. |STYLE120| replace:: **Gamma**

.. |STYLE121| replace:: **Cardinalità**

.. |STYLE122| replace:: **Proprietà**

.. |STYLE123| replace:: **URI**

.. |STYLE124| replace:: **Gamma**

.. |STYLE125| replace:: **Cardinalità**

.. |STYLE126| replace:: **Proprietà**

.. |STYLE127| replace:: **URI**

.. |STYLE128| replace:: **Gamma**

.. |STYLE129| replace:: **Cardinalità**

.. |STYLE130| replace:: **Nome della classe**

.. |STYLE131| replace:: **Obbligatorio / facoltativo**

.. |STYLE132| replace:: **URI**

.. |STYLE133| replace:: **Nome della classe**

.. |STYLE134| replace:: **Obbligatorio / facoltativo**

.. |STYLE135| replace:: **URI**

.. |STYLE136| replace:: **Nome della classe**

.. |STYLE137| replace:: **Obbligatorio / facoltativo**

.. |STYLE138| replace:: **URI**

.. |STYLE139| replace:: **Proprietà**

.. |STYLE140| replace:: **URI**

.. |STYLE141| replace:: **Gamma**

.. |STYLE142| replace:: **Cardinalità**

.. |STYLE143| replace:: **Proprietà**

.. |STYLE144| replace:: **URI**

.. |STYLE145| replace:: **Gamma**

.. |STYLE146| replace:: **Cardinalità**

.. |STYLE147| replace:: **Proprietà**

.. |STYLE148| replace:: **URI**

.. |STYLE149| replace:: **Gamma**

.. |STYLE150| replace:: **Cardinalità**

.. |STYLE151| replace:: **Proprietà**

.. |STYLE152| replace:: **URI**

.. |STYLE153| replace:: **Gamma**

.. |STYLE154| replace:: **Cardinalità**

.. |STYLE155| replace:: **Nome della classe**

.. |STYLE156| replace:: **Obbligatorio / facoltativo**

.. |STYLE157| replace:: **URI**

.. |STYLE158| replace:: *3.7.1.*

.. |STYLE159| replace:: *Identifier*

.. |STYLE160| replace:: **Proprietà**

.. |STYLE161| replace:: **URI**

.. |STYLE162| replace:: **Gamma**

.. |STYLE163| replace:: **Cardinalità**

.. |STYLE164| replace:: **Proprietà**

.. |STYLE165| replace:: **URI**

.. |STYLE166| replace:: **Gamma**

.. |STYLE167| replace:: **Cardinalità**

.. |STYLE168| replace:: **Proprietà**

.. |STYLE169| replace:: **URI**

.. |STYLE170| replace:: **Gamma**

.. |STYLE171| replace:: **Cardinalità**

.. |STYLE172| replace:: **Nome della classe**

.. |STYLE173| replace:: **Obbligatorio / facoltativo**

.. |STYLE174| replace:: **URI**

.. |STYLE175| replace:: **Proprietà**

.. |STYLE176| replace:: **URI**

.. |STYLE177| replace:: **Gamma**

.. |STYLE178| replace:: **Cardinalità**

.. |STYLE179| replace:: **Proprietà**

.. |STYLE180| replace:: **URI**

.. |STYLE181| replace:: **Gamma**

.. |STYLE182| replace:: **Cardinalità**

.. |STYLE183| replace:: **Proprietà**

.. |STYLE184| replace:: **URI**

.. |STYLE185| replace:: **Gamma**

.. |STYLE186| replace:: **Cardinalità**

.. |STYLE187| replace:: **Nome della classe**

.. |STYLE188| replace:: **Obbligatorio / facoltativo**

.. |STYLE189| replace:: **URI**

.. |STYLE190| replace:: **Proprietà**

.. |STYLE191| replace:: **URI**

.. |STYLE192| replace:: **Gamma**

.. |STYLE193| replace:: **Cardinalità**

.. |STYLE194| replace:: **Proprietà**

.. |STYLE195| replace:: **URI**

.. |STYLE196| replace:: **Gamma**

.. |STYLE197| replace:: **Cardinalità**

.. |STYLE198| replace:: **Proprietà**

.. |STYLE199| replace:: **URI**

.. |STYLE200| replace:: **Gamma**

.. |STYLE201| replace:: **Cardinalità**

.. |STYLE202| replace:: **Proprietà**

.. |STYLE203| replace:: **URI**

.. |STYLE204| replace:: **Gamma**

.. |STYLE205| replace:: **Cardinalità**

.. |STYLE206| replace:: **Proprietà**

.. |STYLE207| replace:: **URI**

.. |STYLE208| replace:: **Gamma**

.. |STYLE209| replace:: **Cardinalità**

.. |STYLE210| replace:: **Proprietà**

.. |STYLE211| replace:: **URI**

.. |STYLE212| replace:: **Gamma**

.. |STYLE213| replace:: **Cardinalità**

.. |STYLE214| replace:: **Nome della classe**

.. |STYLE215| replace:: **Obbligatorio / facoltativo**

.. |STYLE216| replace:: **URI**

.. |STYLE217| replace:: **Proprietà**

.. |STYLE218| replace:: **URI**

.. |STYLE219| replace:: **Gamma**

.. |STYLE220| replace:: **Cardinalità**

.. |STYLE221| replace:: **Proprietà**

.. |STYLE222| replace:: **URI**

.. |STYLE223| replace:: **Gamma**

.. |STYLE224| replace:: **Cardinalità**

.. |STYLE225| replace:: **Proprietà**

.. |STYLE226| replace:: **URI**

.. |STYLE227| replace:: **Gamma**

.. |STYLE228| replace:: **Cardinalità**

.. |STYLE229| replace:: **Proprietà**

.. |STYLE230| replace:: **URI**

.. |STYLE231| replace:: **Gamma**

.. |STYLE232| replace:: **Cardinalità**

.. |STYLE233| replace:: **Nome della classe**

.. |STYLE234| replace:: **Obbligatorio / facoltativo**

.. |STYLE235| replace:: **URI**

.. |STYLE236| replace:: **Proprietà**

.. |STYLE237| replace:: **URI**

.. |STYLE238| replace:: **Gamma**

.. |STYLE239| replace:: **Cardinalità**

.. |STYLE240| replace:: **Proprietà**

.. |STYLE241| replace:: **URI**

.. |STYLE242| replace:: **Gamma**

.. |STYLE243| replace:: **Cardinalità**

.. |STYLE244| replace:: **Proprietà**

.. |STYLE245| replace:: **URI**

.. |STYLE246| replace:: **Gamma**

.. |STYLE247| replace:: **Cardinalità**

.. |STYLE248| replace:: **Proprietà**

.. |STYLE249| replace:: **URI**

.. |STYLE250| replace:: **Gamma**

.. |STYLE251| replace:: **Cardinalità**

.. |STYLE252| replace:: **Proprietà**

.. |STYLE253| replace:: **URI**

.. |STYLE254| replace:: **Gamma**

.. |STYLE255| replace:: **Cardinalità**

.. |STYLE256| replace:: **Proprietà**

.. |STYLE257| replace:: **URI**

.. |STYLE258| replace:: **Gamma**

.. |STYLE259| replace:: **Cardinalità**

.. |STYLE260| replace:: **Nome della classe**

.. |STYLE261| replace:: **Obbligatorio / facoltativo**

.. |STYLE262| replace:: **URI**

.. |STYLE263| replace:: **Proprietà**

.. |STYLE264| replace:: **URI**

.. |STYLE265| replace:: **Gamma**

.. |STYLE266| replace:: **Cardinalità**

.. |STYLE267| replace:: **Proprietà**

.. |STYLE268| replace:: **URI**

.. |STYLE269| replace:: **Gamma**

.. |STYLE270| replace:: **Cardinalità**

.. |STYLE271| replace:: **Proprietà**

.. |STYLE272| replace:: **URI**

.. |STYLE273| replace:: **Gamma**

.. |STYLE274| replace:: **Cardinalità**

.. |STYLE275| replace:: **Proprietà**

.. |STYLE276| replace:: **URI**

.. |STYLE277| replace:: **Gamma**

.. |STYLE278| replace:: **Cardinalità**

.. |STYLE279| replace:: **Proprietà**

.. |STYLE280| replace:: **URI**

.. |STYLE281| replace:: **Gamma**

.. |STYLE282| replace:: **Cardinalità**

.. |STYLE283| replace:: **Proprietà**

.. |STYLE284| replace:: **URI**

.. |STYLE285| replace:: **Gamma**

.. |STYLE286| replace:: **Cardinalità**

.. |STYLE287| replace:: **Nome della classe**

.. |STYLE288| replace:: **Obbligatorio / facoltativo**

.. |STYLE289| replace:: **URI**

.. |STYLE290| replace:: **Nome della classe**

.. |STYLE291| replace:: **Obbligatorio / facoltativo**

.. |STYLE292| replace:: **URI**

.. |STYLE293| replace:: **Proprietà**

.. |STYLE294| replace:: **URI**

.. |STYLE295| replace:: **Gamma**

.. |STYLE296| replace:: **Cardinalità**

.. |STYLE297| replace:: **Proprietà**

.. |STYLE298| replace:: **URI**

.. |STYLE299| replace:: **Gamma**

.. |STYLE300| replace:: **Cardinalità**

.. |STYLE301| replace:: **Proprietà**

.. |STYLE302| replace:: **URI**

.. |STYLE303| replace:: **Gamma**

.. |STYLE304| replace:: **Cardinalità**

.. |STYLE305| replace:: **Proprietà**

.. |STYLE306| replace:: **URI**

.. |STYLE307| replace:: **Gamma**

.. |STYLE308| replace:: **Cardinalità**

.. |STYLE309| replace:: **Proprietà**

.. |STYLE310| replace:: **URI**

.. |STYLE311| replace:: **Gamma**

.. |STYLE312| replace:: **Cardinalità**

.. |STYLE313| replace:: **Nome della classe**

.. |STYLE314| replace:: **Obbligatorio / facoltativo**

.. |STYLE315| replace:: **URI**

.. |STYLE316| replace:: **Proprietà**

.. |STYLE317| replace:: **URI**

.. |STYLE318| replace:: **Gamma**

.. |STYLE319| replace:: **Cardinalità**

.. |STYLE320| replace:: **Proprietà**

.. |STYLE321| replace:: **URI**

.. |STYLE322| replace:: **Gamma**

.. |STYLE323| replace:: **Cardinalità**

.. |STYLE324| replace:: **Proprietà**

.. |STYLE325| replace:: **URI**

.. |STYLE326| replace:: **Gamma**

.. |STYLE327| replace:: **Cardinalità**

.. |STYLE328| replace:: **Proprietà**

.. |STYLE329| replace:: **URI**

.. |STYLE330| replace:: **Gamma**

.. |STYLE331| replace:: **Cardinalità**

.. |STYLE332| replace:: **Nome della classe**

.. |STYLE333| replace:: **Obbligatorio / facoltativo**

.. |STYLE334| replace:: **URI**

.. |STYLE335| replace:: **Proprietà**

.. |STYLE336| replace:: **URI**

.. |STYLE337| replace:: **Gamma**

.. |STYLE338| replace:: **Cardinalità**

.. |STYLE339| replace:: **Nome della classe**

.. |STYLE340| replace:: **Obbligatorio / facoltativo**

.. |STYLE341| replace:: **URI**

.. |STYLE342| replace:: **Proprietà**

.. |STYLE343| replace:: **URI**

.. |STYLE344| replace:: **Gamma**

.. |STYLE345| replace:: **Cardinalità**

.. |STYLE346| replace:: **Nome della classe**

.. |STYLE347| replace:: **Obbligatorio / facoltativo**

.. |STYLE348| replace:: **URI**

.. |STYLE349| replace:: **Nome della classe**

.. |STYLE350| replace:: **Obbligatorio / facoltativo**

.. |STYLE351| replace:: **URI**

.. |STYLE352| replace:: **Nome della classe**

.. |STYLE353| replace:: **Obbligatorio / facoltativo**

.. |STYLE354| replace:: **URI**

.. |STYLE355| replace:: **Proprietà**

.. |STYLE356| replace:: **URI**

.. |STYLE357| replace:: **Gamma**

.. |STYLE358| replace:: **Cardinalità**


.. |REPLACE1| raw:: html

    <img src="https://raw.githubusercontent.com/cirospat/-vocabolario-controllato-servizi-pubblici/master/static/CPSV-AP_Specification%20v2.2.png" />

.. |LINK1| raw:: html

    <a href="http://publications.europa.eu/resource/authority/atu/MLT" target="_blank">http://publications.europa.eu/resource/authority/atu/MLT</a>

.. |LINK2| raw:: html

    <a href="http://publications.europa.eu/resource/authority/atu/BEL_PR_WVL" target="_blank">http://publications.europa.eu/resource/authority/atu/BEL_PR_WVL</a>

.. |LINK3| raw:: html

    <a href="https://translate.googleusercontent.com/translate_f#_ftn9" target="_blank">[9]</a>



.. rubric:: Footnotes

.. [#f1]   `https://www.ietf.org/rfc/rfc2119.txt <https://www.ietf.org/rfc/rfc2119.txt>`__  
.. [#f2]   `http://ec.europa.eu/isa/documents/isa_annex_ii_eif_en.pdf <http://ec.europa.eu/isa/documents/isa_annex_ii_eif_en.pdf>`__  
.. [#f3]   `https://joinup.ec.europa.eu/asset/criterion_evidence_cv/description <https://joinup.ec.europa.eu/asset/criterion_evidence_cv/description>`__  
.. [#f4]   `http://publications.europa.eu/resource/authority/atu/ <http://publications.europa.eu/resource/authority/atu/>`__  
.. [#f5]   `https://en.wikipedia.org/wiki/ISO_8601#Durations <https://en.wikipedia.org/wiki/ISO_8601#Durations>`__  
.. [#f6]   `http://www.iso.org/iso/catalogue_detail?csnumber=40874 <http://www.iso.org/iso/catalogue_detail?csnumber=40874>`__  
.. [#f7]  This property should be a URI if it is modelled in RDF.
.. [#f8]   `https://www.w3.org/TR/vocab-dcat/#class-dataset <https://www.w3.org/TR/vocab-dcat/#class-dataset>`__  
.. [#f9]  Questa proprietà dovrebbe essere un URI se è modellato in RDF.
.. [#f10]  This property should be a URI if it is modelled in RDF.
.. [#f11]   `https://joinup.ec.europa.eu/asset/criterion_evidence_cv/description <https://joinup.ec.europa.eu/asset/criterion_evidence_cv/description>`__  
.. [#f12]  This property should be a URI if it is modelled in RDF.
.. [#f13]  This property should be a URI if it is modelled in RDF.
.. [#f14]  This property should be a URI if it is modelled in RDF.
.. [#f15]  This property should be a URI if it is modelled in RDF.
.. [#f16]   `http://schema.org/openingHours <http://schema.org/openingHours>`__ 
.. [#f17]   `http://schema.org/OpeningHoursSpecification <http://schema.org/OpeningHoursSpecification>`__  
.. [#f18]  This property should be a URI if it is modelled in RDF.
.. [#f19]  This property should be a URI if it is modelled in RDF.
.. [#f20]   `http://publications.europa.eu/mdr/eli/ <http://publications.europa.eu/mdr/eli/>`__  
.. [#f21]   `https://joinup.ec.europa.eu/asset/cpov/asset_release/all <https://joinup.ec.europa.eu/asset/cpov/asset_release/all>`__  
.. [#f22]   `http://www.w3.org/TR/vocab-org/ <http://www.w3.org/TR/vocab-org/>`__  
.. [#f23]   `http://publications.europa.eu/mdr/authority/atu/ <http://publications.europa.eu/mdr/authority/atu/>`__  
.. [#f24]   `https://www.w3.org/TR/skos-reference/#concepts <https://www.w3.org/TR/skos-reference/#concepts>`__  
.. [#f25]   `https://www.w3.org/TR/skos-reference/ <https://www.w3.org/TR/skos-reference/>`__  
.. [#f26]   `https://www.w3.org/TR/skos-reference/#concepts <https://www.w3.org/TR/skos-reference/#concepts>`__  
.. [#f27]   `https://www.w3.org/TR/skos-reference/ <https://www.w3.org/TR/skos-reference/>`__  
