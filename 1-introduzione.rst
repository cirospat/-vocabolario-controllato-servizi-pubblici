
.. _h4258373d4d6f5e28414207f3f56354:

1. Introduzione
***************

L'originale CPSV-AP è stato preparato nel contesto dell'Azione 2016.29 - Accesso alle risorse informative degli Stati membri a livello europeo - Catalogo dei servizi\ [#F1]_\  del programma Interoperabilità della Commissione europea delle amministrazioni pubbliche \ |LINK1|\  [Commissione europea. Interoperabilità per le pubbliche amministrazioni europee (ISA)]. Il CPSV-AP è stato visto come un primo passo per la creazione di un modello per la descrizione di servizi pubblici relativi a eventi aziendali e di vita, per facilitare l'organizzazione di cataloghi di servizi orientati alle imprese e ai cittadini.

 

Questo documento definisce un aggiornamento della versione 2.1 del profilo applicativo del vocabolario del servizio pubblico principale (\ |LINK2|\ ). L'aggiornamento è motivato dall’esperienza di implementazione della versione 2.1 del CPSV-AP da parte di diversi SM e stakeholder e dalle conseguenti richieste ricevute in \ |LINK3|\  o durante \ |LINK4|\  e durante il seminario organizzato a \ |LINK5|\  .

.. _h5325917564305c2c564cf654158:

1.1. Portata e obiettivi
========================

Dalla pubblicazione del CPSV-AP, diversi Stati membri e progetti europei hanno iniziato a utilizzare ed estendere il modello dati in base alle proprie esigenze. L'utilizzo di questo modello dati in contesti nazionali o regionali ha portato all'identificazione di potenziali aree di miglioramento ed estensione. Grazie al feedback ricevuto, la versione 2.2 ha aggiornato la precendente versione delle specifiche allineandola con ELI, aggiornandola classificazione dei servizi pubblici e le proprietà corrispondenti e correggendo alcuni bug.

 

Questo lavoro tiene anche conto delle implementazioni di CPSV-AP da parte di entità diverse, cercando di mantenere le specifiche il più stabili possibile.

 

.. _h5b4f8381629b5696c14362a697c49:

1.2. Processo e metodologia
===========================

Questo modello dati comune è stato definito come profilo applicativo del Vocabolario di servizio pubblico \ |LINK6|\  (d'ora in poi indicato come CPSV-AP). Un \ |LINK7|\  è una specifica che riutilizza i termini da uno o più standard di base, aggiungendo più specificità identificando gli elementi obbligatori, consigliati e facoltativi da utilizzare per una particolare applicazione, nonché le raccomandazioni per i vocabolari controllati da utilizzare.

 

L'identificazione e la gestione delle richieste di modifica seguono il "Processo di rilascio e pubblicazione della gestione delle modifiche per le specifiche dei metadati strutturali sviluppati dal programma ISA". In particolare questo deliverable copre la gestione delle richieste delle modifiche.

.. _h386873735a7c773d1f1f4793d4c2e:

Figura 1. Gestione richieste
============================


|REPLACE1|

CPSV-AP 2.1 è stato sviluppato sotto la responsabilità del programma \ |LINK8|\  della Commissione europea e le sedie del gruppo di lavoro. Il gruppo di lavoro è responsabile della definizione delle specifiche ed è costituito da:

* Membri della rete EUGO;

* Rappresentanti degli SM da altri portali di eGovernment;

* Membri del gruppo di lavoro CPSV;

* Rappresentanti del comitato \ |LINK9|\ ;

* Esperti in materia di governo e modellizzazione di eventi della vita e servizi pubblici; e

* Istituzioni e iniziative europee (ad es. DG GROW, YourEurope, eSENS ...).

La metodologia spiega il processo di specifica e il suo approccio. Descrive gli elementi che dovrebbero essere inclusi nelle specifiche, inclusi casi d'uso e definizione dei termini (ad es. Classi e proprietà) e vocabolari controllati raccomandati, basati sulla ricerca e la revisione delle soluzioni esistenti.

 

Naturalmente, la specifica del CPSV-AP 2.2 è iniziata con la versione originale CPSV-AP 2. 1 e il contributo degli Stati membri e delle organizzazioni che hanno avuto esperienze dirette sull'utilizzo di esso. Che WA ingresso ha raccolti e analizzati nel corso di due webinar e un workshop che ha portato alla registrazione di una serie di richieste di modifica specifici.

 

In generale, il feedback ricevuto è stato positivo. Naturalmente, implementarlo nei contesti nazionali implica l'esigenza di adattare il modello ai contesti corrispondenti. Nella maggior parte di queste implementazioni, il CPSV (-AP) è stato esteso con ulteriori classi, proprietà, vocabolari controllati ...

.. _h512b605c7d2579263d7d3e307052654e:

1.3. Struttura di questo documento
==================================

Questo documento è costituito dalle seguenti sezioni:

* La Sezione 2 definisce i principali casi d'uso che guidano le specifiche del Profilo dell'applicazione;

* Le classi e le proprietà definite per il profilo dell'applicazione sono identificate nella sezione 3;

* Nella sezione 4, i vocabolari controllati sono proposti per l'utilizzo come set di valori per un numero di proprietà;

* Un esempio, che aiuta a mostrare come l'APC CPSV può essere utilizzato nella pratica per descrivere un servizio pubblico, è descritto nella sezione 5;

* La sezione 6 contiene la dichiarazione di conformità per questo profilo applicativo;

* Accessibilità e questioni multilingue sono trattate nella sezione 7;

* Nomi e prefissi utilizzati in tutte le specifiche sono elencati nella sezione 8;

* I ringraziamenti relativi allo sviluppo di questo profilo dell'applicazione sono contenuti nella sezione 9;

* Infine, nella sezione 0 , una panoramica delle modifiche alle specifiche viene fornita nel registro delle modifiche.

.. bottom of content


.. |REPLACE1| raw:: html

    <img src=https://raw.githubusercontent.com/cirospat/-vocabolario-controllato-servizi-pubblici/master/static/figura1.PNG />

.. |LINK1| raw:: html

    <a href="http://ec.europa.eu/isa/index_en.htm " target="_blank">(ISA) della Commissione europea</a>

.. |LINK2| raw:: html

    <a href="https://joinup.ec.europa.eu/release/core-public-service-vocabulary-application-profile/22" target="_blank">CPSV-AP v2.2</a>

.. |LINK3| raw:: html

    <a href="https://github.com/catalogue-of-services-isa/CPSV-AP/issues" target="_blank">GitHub</a>

.. |LINK4| raw:: html

    <a href="https://joinup.ec.europa.eu/event/catalogue-services-webinar-reuse-and-implementation-cpsv-ap-19-march-2018" target="_blank">webinar</a>

.. |LINK5| raw:: html

    <a href="https://joinup.ec.europa.eu/event/catalogue-services-workshop-15-june-back-back-semic-2018" target="_blank">Sofia</a>

.. |LINK6| raw:: html

    <a href="https://joinup.ec.europa.eu/asset/core_public_service/description" target="_blank">ISA Core</a>

.. |LINK7| raw:: html

    <a href="http://dublincore.org/documents/2001/04/12/usageguide/glossary.shtml#A" target="_blank">profilo applicativo</a>

.. |LINK8| raw:: html

    <a href="https://ec.europa.eu/isa2/home_en" target="_blank">ISA</a>

.. |LINK9| raw:: html

    <a href="https://ec.europa.eu/isa2/home_en" target="_blank">ISA</a>



.. rubric:: Footnotes

.. [#f1]  Commissione europea. Interoperabilità per le pubbliche amministrazioni europee (ISA). Accesso alle risorse informative degli Stati membri a livello europeo.   `http://ec.europa.eu/isa/actions/01-trusted-information-exchange/1-3action_en.htm <http://ec.europa.eu/isa/actions/01-trusted-information-exchange/1-3action_en.htm>`__  
