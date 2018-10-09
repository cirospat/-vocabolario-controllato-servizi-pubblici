
.. _h37562677d2d265b121d315261695617:

4.0 Vocabolari controllati consigliati
######################################

Al fine di facilitare lo scambio di informazioni sui servizi pubblici raggruppati in eventi aziendali o eventi della vita, i vocabolari controllati hanno lo scopo di armonizzare i valori possibili per determinate proprietà. Ciò migliora l'interoperabilità delle descrizioni e facilita l'integrazione di informazioni provenienti da fonti diverse. Per quanto riguarda il modello di dominio CPSV-AP descritto nella sezione 3, le organizzazioni pubbliche possono mappare i valori dei vocabolari controllati che usano per descrivere i servizi pubblici nella loro SM, ai valori specifici dei vocabolari controllati suggeriti di seguito.

 

È importante ricordare che i vocabolari controllati raccomandati in CPSV-AP non sono obbligatori. Pertanto, possono essere utilizzati altri vocabolari controllati che sono più adatti o adattati al contesto nazionale. Possono anche essere estesi dagli Stati membri per soddisfare le loro esigenze specifiche. In particolare, questo può essere utile per i vocabolari controllati raccomandati di cui sono stati definiti solo i valori di alto livello. Ad esempio, per la proprietà " Area tematica " della classe "Evento aziendale", un MS può estendere questo particolare vocabolario controllato aggiungendo ulteriori eventi o fornendo ulteriori livelli di granularità.

 

Dove possibile, la Tabella 1 fornisce un suggerimento per i vocabolari controllati per le proprietà incluse nel CPSV-AP. Per elaborare la panoramica, i vocabolari controllati che sono stati sviluppati nel contesto di iniziative europee o di altre iniziative sovranazionali (ad esempio EL, Named Authority Lists, Eurovoc, NACE, COFOG ...) e che sono già stati utilizzati in più applicazioni, sono massimizzati essere riutilizzato. Inoltre, al fine di allinearsi con i Vocabolari Core esistenti, i vocabolari controllati già utilizzati vengono riutilizzati al massimo in questo profilo dell'applicazione. Inoltre, vengono presi in considerazione i vocabolari controllati esistenti negli Stati membri.

 

In particolare per la lista 1\ |STYLE0|\  e 2\ |STYLE1|\  livello eventi aziendali, 1 \ |STYLE2|\  livello di eventi della vita e livello di tipi di output, il vocabolario controllato suggerito è basato su un'analisi effettuata. Per questo, i dati sono stati raccolti dalla letteratura e dai portali di servizio pubblico esistenti e questi dati sono stati confrontati, interpretati e analizzati al fine di elaborare una proposta. Questa proposta è stata discussa in una riunione del gruppo di lavoro e il feedback ricevuto è stato elaborato in versioni modificate che sono state aggiunte a questa specifica come vocabolari controllati raccomandati per:

* Tipo di evento aziendale;

* Tipo di evento di vita; e

* Tipo di uscita

 

\ |STYLE3|\ 

+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Classe                 |Proprietà                |Vocabolario controllato                                                                                 |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Evento                 |Genere                   |Evento aziendale                                                                                        |
|                       |                         |                                                                                                        |
|                       |                         |Evento della vita                                                                                       |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Evento aziendale       |genere\ [#F1]_\          |Iniziare affari                                                                                         |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione di un'azienda                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Richiede una licenza, un permesso o un certificato per avviare o continuare un'attività               |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione della proprietà intellettuale                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione di un ramo                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* Inizia una nuova attività                                                                             |
|                       |                         |                                                                                                        |
|                       |                         |* Finanziamento di un'azienda                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Assumere un dipendente                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |Avvio di attività transfrontaliere                                                                      |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione di un'attività transfrontaliera                                                         |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione di un ramo                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |Facendo affari                                                                                          |
|                       |                         |                                                                                                        |
|                       |                         |* Finanziamento di un'azienda                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Richiede una licenza, un permesso o un certificato per avviare o continuare un'attività               |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione della proprietà intellettuale                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Assumere un dipendente                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |* Partecipare agli appalti pubblici                                                                     |
|                       |                         |                                                                                                        |
|                       |                         |* Notifica e segnalazione alle autorità                                                                 |
|                       |                         |                                                                                                        |
|                       |                         |* Inizia una nuova attività                                                                             |
|                       |                         |                                                                                                        |
|                       |                         |* Registrazione di un ramo                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* Avere problemi nel pagare i creditori                                                                 |
|                       |                         |                                                                                                        |
|                       |                         |Concludere affari                                                                                       |
|                       |                         |                                                                                                        |
|                       |                         |* Ristrutturazione di un'azienda                                                                        |
|                       |                         |                                                                                                        |
|                       |                         |* Scioglimento di una società                                                                           |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Evento della vita      |Genere\ [#F2]_\          |* Avere un figlio                                                                                       |
|                       |                         |                                                                                                        |
|                       |                         |* Diventare un custode (sociale)                                                                        |
|                       |                         |                                                                                                        |
|                       |                         |* Iniziare l'educazione                                                                                 |
|                       |                         |                                                                                                        |
|                       |                         |* Alla ricerca di un nuovo lavoro                                                                       |
|                       |                         |                                                                                                        |
|                       |                         |* Perdere / lasciare un lavoro                                                                          |
|                       |                         |                                                                                                        |
|                       |                         |* Alla ricerca di un posto dove vivere                                                                  |
|                       |                         |                                                                                                        |
|                       |                         |* Modifica dello stato della relazione                                                                  |
|                       |                         |                                                                                                        |
|                       |                         |* Guidare un veicolo                                                                                    |
|                       |                         |                                                                                                        |
|                       |                         |* Viaggiare all'estero                                                                                  |
|                       |                         |                                                                                                        |
|                       |                         |* Trasferimenti da / verso il paese                                                                     |
|                       |                         |                                                                                                        |
|                       |                         |* Andare al servizio militare                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Di fronte a un problema di emergenza / salute                                                         |
|                       |                         |                                                                                                        |
|                       |                         |* Di fronte a un crimine                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |* La pensione                                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* Morte di un parente                                                                                   |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Servizio pubblico      |Genere                   |Tassonomia COFOG\ [#F3]_\                                                                               |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Area tematica            |TBC                                                                                                     |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Linguaggio               |Elenco delle autorità denominate nelle lingue dell'Ufficio delle pubblicazioni europee (NAL)\ [#F4]_\   |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Settore                  |Elenco dei codici NACE\ [#F5]_\                                                                         |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Spaziale                 |MDR Continents Elenco delle autorità denominate\ [#F6]_\  , Elenco delle autorità con nome Paesi MDR    |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Stato                    |Vocabolario di stato ADMS\ [#F10]_\                                                                     |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Partecipazione         |Ruolo                    |TBC                                                                                                     |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Criterion Requirement  |genere                   |TBC                                                                                                     |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Prova                  |genere                   |TBC                                                                                                     |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |linguaggio               |Elenco delle autorità denominate nelle lingue dell'Ufficio delle pubblicazioni europee (NAL)\ [#F11]_\  |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Produzione             |genere\ [#F12]_\         |* Dichiarazione                                                                                         |
|                       |                         |                                                                                                        |
|                       |                         |* Oggetto fisico                                                                                        |
|                       |                         |                                                                                                        |
|                       |                         |* Codice                                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |* Obbligo finanziario                                                                                   |
|                       |                         |                                                                                                        |
|                       |                         |* Beneficio finanziario                                                                                 |
|                       |                         |                                                                                                        |
|                       |                         |* Riconoscimento                                                                                        |
|                       |                         |                                                                                                        |
|                       |                         |* Permesso                                                                                              |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Costo                  |Moneta                   |Elenco delle autorità nominate dall'Ufficio delle pubblicazioni europee (NAL)\ [#F13]_\                 |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Canale                 |genere                   |* E-mail                                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |* Homepage                                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* Fax                                                                                                   |
|                       |                         |                                                                                                        |
|                       |                         |* Assistente                                                                                            |
|                       |                         |                                                                                                        |
|                       |                         |* Telefono                                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* App per dispositivi mobili                                                                            |
|                       |                         |                                                                                                        |
|                       |                         |* Tv digitale                                                                                           |
|                       |                         |                                                                                                        |
|                       |                         |* posta                                                                                                 |
|                       |                         |                                                                                                        |
|                       |                         |* Servizio di assistenza                                                                                |
|                       |                         |                                                                                                        |
|                       |                         |* Posizione del cliente                                                                                 |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Regola                 |linguaggio               |Elenco delle autorità denominate nelle lingue dell'Ufficio delle pubblicazioni europee (NAL)\ [#F14]_\  |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Quadro formale         |linguaggio               |Elenco delle autorità denominate nelle lingue dell'Ufficio delle pubblicazioni europee (NAL)\ [#F15]_\  |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Stato                    |* Identificatore della legislazione europea\ [#F16]_\ :                                                 |
|                       |                         |                                                                                                        |
|                       |                         |* vigente                                                                                               |
|                       |                         |                                                                                                        |
|                       |                         |* non in vigore                                                                                         |
|                       |                         |                                                                                                        |
|                       |                         |* parzialmente applicabile                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* implicitamente revocato                                                                               |
|                       |                         |                                                                                                        |
|                       |                         |* esplicitamente revocato                                                                               |
|                       |                         |                                                                                                        |
|                       |                         |* abrogato                                                                                              |
|                       |                         |                                                                                                        |
|                       |                         |* scaduto                                                                                               |
|                       |                         |                                                                                                        |
|                       |                         |* sospeso                                                                                               |
|                       |                         |                                                                                                        |
|                       |                         |* altro                                                                                                 |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Soggetto                 |Domini Eurovoc\ [#F17]_\                                                                                |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |Applicazione territoriale|Tassonomia NUTS\ [#F18]_\                                                                               |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|                       |genere                   |Tipi di risorse Named Authority Lists (NAL)\ [#F19]_\                                                   |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+
|Organizzazione pubblica|Spaziale                 |MDR Continents Elenco delle autorità denominate\ [#F20]_\  , Elenco delle autorità con nome Paesi MDR   |
+-----------------------+-------------------------+--------------------------------------------------------------------------------------------------------+


.. bottom of content


.. |STYLE0| replace:: :sup:`°`

.. |STYLE1| replace:: :sup:`°`

.. |STYLE2| replace:: :sup:`st`

.. |STYLE3| replace:: **Tabella 1 : vocabolari controllati da CPSV-AP**


.. rubric:: Footnotes

.. [#f1]  Il 2° livello di eventi aziendali potrebbero presentare domanda di diverse 1 \ :sup:`st`\ eventi aziendali di livello, portando a una relazione molti-a-molti mapping tra 1 \ :sup:`°`\ e 2 \ :sup:`nd`\ eventi aziendali di livello. Una descrizione per ogni 2 \ :sup:`°`\ evento di business di livello è stato inserito nella “ Descrizione del 2 \ :sup:`nd`\ eventi aziendali di livello”.
.. [#f2]  La lista attualmente include solo un 1 \ :sup:`°`\ livello per eventi della vita. Una descrizione per ogni evento della vita di \ :sup:`primo`\ livello è stata inclusa in " Descrizione degli eventi di 1 ° livello ".
.. [#f3]  http://unstats.un.org/unsd/cr/registry/regcst.asp?Cl=4
.. [#f4]  http://publications.europa.eu/mdr/authority/language/index.html
.. [#f5]  http://ec.europa.eu/competition/mergers/cases/index/nace_all.html
.. [#f6]  http://publications.europa.eu/mdr/authority/continent/index.html
.. [#f7]  http://publications.europa.eu/mdr/authority/country/
.. [#f8]  http://publications.europa.eu/mdr/authority/place/index.html
.. [#f9]  http://sws.geonames.org/
.. [#f10]  http://purl.org/adms/status/
.. [#f11]  http://publications.europa.eu/mdr/authority/language/index.html
.. [#f12]  Una descrizione per ciascun tipo di output è stata inclusa in " Descrizione dei tipi di output ".
.. [#f13]  http://publications.europa.eu/mdr/authority/currency/index.html
.. [#f14]  http://publications.europa.eu/mdr/authority/language/index.html
.. [#f15]   http://publications.europa.eu/mdr/authority/language/index.html
.. [#f16]  http://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX:52012XG1026(01)
.. [#f17]  http://eurovoc.europa.eu/drupal/?q=download/subject_oriented&cl=en
.. [#f18]   `http://ec.europa.eu/eurostat/ramon/nomenclatures/index.cfm?TargetUrl=LST_NOM_DTL&StrNom=NUTS_22&StrLanguageCode=EN&IntPcKey=&StrLayoutCode=HIERARCHIC <http://ec.europa.eu/eurostat/ramon/nomenclatures/index.cfm?TargetUrl=LST_NOM_DTL&StrNom=NUTS_22&StrLanguageCode=EN&IntPcKey=&StrLayoutCode=HIERARCHIC>`__ 
.. [#f19]  http://publications.europa.eu/mdr/authority/resource-type/index.html
.. [#f20]  http://publications.europa.eu/mdr/authority/continent/index.html
.. [#f21]  http://publications.europa.eu/mdr/authority/country/
.. [#f22]  http://publications.europa.eu/mdr/authority/place/index.html
.. [#f23]  http://sws.geonames.org/
