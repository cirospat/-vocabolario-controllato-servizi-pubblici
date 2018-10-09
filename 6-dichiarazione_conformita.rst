
.. _h276951423965157734381d58f735032:

4. Dichiarazione di conformità
##############################

.. _h78f407310781d52704be11782d7b3d:

6.1. Requisiti del provider
***************************

Per conformarsi al profilo di applicazione del vocabolario del servizio pubblico principale (CPSV-AP), qualsiasi implementazione DEVE:

* Includere almeno tutte le proprietà obbligatorie di tutte le classi obbligatorie come indicato in " Elenco dettagliato delle classi e delle proprietà obbligatorie e facoltative ";

* Includere almeno tutte le proprietà obbligatorie di qualsiasi classe facoltativa utilizzata per descrivere il servizio pubblico, come indicato in " Elenco dettagliato di classi e proprietà obbligatorie e facoltative ";

* Non avere più di una istanza di quelle proprietà che hanno 1 come cardinalità massima come specificato in ciascuna sottosezione dalla Sezione 3.2 alla Sezione 3.18 ;

* Definisci ogni valore della proprietà in base al tipo specificato nella sezione 3 (vedi il diagramma UML in Figura 2 );

* Usa i termini (classi e proprietà) in modo coerente con la loro semantica come dichiarato nella Sezione 3 .

 

Un'implementazione conforme del profilo di applicazione del vocabolario del servizio pubblico principale può includere classi e proprietà da altri modelli di dati (vocabolari). Inoltre, un'implementazione conforme del profilo di applicazione del vocabolario del servizio pubblico principale può includere termini dai vocabolari controllati raccomandati per le proprietà corrispondenti, come elencato nella sezione 4 .

 

Il profilo di applicazione del vocabolario del servizio pubblico principale è neutro dal punto di vista tecnologico e un editore può utilizzare uno qualsiasi dei termini definiti in questo documento codificato in qualsiasi tecnologia, sebbene siano preferiti RDF e XML.

.. _h1823e441fb1934441c3e605e515114:

6.2. Requisiti del ricevitore
*****************************

Per conformarsi al profilo di applicazione del vocabolario del servizio pubblico principale, qualsiasi applicazione che riceve metadati DEVE essere in grado di:

* Informazioni sul processo per tutte le classi specificate nella Sezione 3 ;

* Informazioni di processo per tutte le proprietà specificate nella Sezione 3 .

* Informazioni sul processo per tutti i vocabolari controllati specificati nella Sezione 4 .

 

"Elaborazione" significa che i ricevitori devono accettare i dati in arrivo e fornire in modo trasparente questi dati alle applicazioni e ai servizi. Non implica né prescrive quali applicazioni e servizi possono finalmente fare con i dati (analizzare, convertire, memorizzare, rendere ricercabili, visualizzare agli utenti, ecc.). 


.. bottom of content
