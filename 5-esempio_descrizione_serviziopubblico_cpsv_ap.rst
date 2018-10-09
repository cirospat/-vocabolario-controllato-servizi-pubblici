
.. _h806668642a427043636445050224b65:

5.  Esempio di descrizione di un servizio pubblico con CPSV-AP
##############################################################

Questa sezione include una descrizione di esempio di un servizio pubblico e le sue proprietà principali e classi associate. L'esempio che è stato descritto inizia dalla descrizione del servizio pubblico ( 5.1 ).

 

Alcune delle proprietà di un servizio pubblico sono in realtà un'associazione con un'altra classe. Nel caso di "ha autorità competente", ad esempio, questo collega la classe di servizio pubblico con la classe di organizzazione pubblica . Nell'esempio "ha autorità competente" ottiene un URI come valore, e la stessa organizzazione pubblica è descritta nella sezione 5.6 . Nella descrizione di esempio di un servizio pubblico, questo vale anche per "è raggruppato per" ( 5.2 ), "ha input" (non descritto in dettaglio in questo esempio), "produce" ( 5.4 ), "ha un canale" ( 5.5 ) e "ha un costo" (non descritto in dettaglio in questo esempio).

 

L'esempio fornisce dati in due formati diversi:

* Leggibile dall'uomo: descritto in una tabella per classe, in cui ogni riga di una tabella è una proprietà della classe corrispondente per cui vengono forniti il ​​nome della proprietà, la cardinalità e il valore; e

* Leggibile a macchina: per ogni classe, le stesse informazioni sono anche rappresentate in RDF Turtle.

I dati sono stati creati sulla base di un servizio pubblico esemplificativo dal punto di contatto singolo finlandese\ [#F1]_\ , ma è stato integrato con dati fittizi dove necessario.

.. _h3c63454d7c1c72467714621c272e4b:

5.1. Classe di servizio pubblico
********************************

 

\ |STYLE0|\ 


+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Proprietà             |Valore                                                                                                                                                                                                                                                                       |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Identifier            |https://www.yrityssuomi.fi/en/palvelu/-/palvelu/electronicapplicationforatrademark?region=helsinki                                                                                                                                                                           |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Nome                  |Applicazione elettronica per un marchio                                                                                                                                                                                                                                      |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Descrizione           |Un marchio è un simbolo che distingue beni e servizi da beni e servizi simili di altri.                                                                                                                                                                                      |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |Un marchio è un simbolo che distingue beni e servizi da beni e servizi simili di altri.Un marchio è un simbolo che distingue i prodotti e i servizi di un'azienda dai prodotti e servizi simili di altre società. Un marchio rappresenta un mezzo di distinzione nel mercato.|
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |Un marchio è anche un diritto esclusivo. Assegna al titolare il diritto esclusivo di utilizzare il marchio nei documenti commerciali, di imballaggio o commerciali dei prodotti o servizi o in qualsiasi altro modo, anche per via orale.                                    |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |Esistono diversi tipi di marchi. Un marchio può, per esempio, essere una parola, una figura, uno slogan o persino un suono.                                                                                                                                                  |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |                                                                                                                                                                                                                                                                             |
|                      |Quando registri il tuo marchio, otterrai protezione per questo per dieci anni. La protezione fornita dalla registrazione inizia alla data della domanda e può essere rinnovata ogni dieci anni.                                                                              |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Ha autorità competente|https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/8566c45a-8b9e-46d5-8371-81c8ad002362&region=helsinki                                                                                                                                                   |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|linguaggio            |http://publications.europa.eu/resource/authority/language/ENG                                                                                                                                                                                                                |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|È raggruppato da      |http://europa.eu/youreurope/businessOntology#start-grow                                                                                                                                                                                                                      |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Ha input              |https://www.prh.fi/input/form                                                                                                                                                                                                                                                |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|produce               |https://www.prh.fi/output/result                                                                                                                                                                                                                                             |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Ha un canale          |https://www.prh.fi/channel/online                                                                                                                                                                                                                                            |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Ha un canale          |https://www.prh.fi/channel/mail                                                                                                                                                                                                                                              |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Ha un costo           |https://www.prh.fi/input/cost                                                                                                                                                                                                                                                |
+----------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

 

\ |STYLE1|\ 


+----------------------------------------------------------------------------------------------------------------------------+
|                                                                                                                            |
|                                                                                                                            |
|<https://www.yrityssuomi.fi/en/palvelu/-/palvelu/electronicapplicationforatrademark?region=helsinki> a cpsv: PublicService; |
|                                                                                                                            |
|    \ |STYLE2|\  "Applicazione elettronica per un marchio";                                                                 |
|                                                                                                                            |
|    \ |STYLE3|\                                                                                                             |
|                                                                                                                            |
|"Un marchio è un simbolo che distingue beni e servizi da beni e servizi simili di altri.                                    |
|                                                                                                                            |
|Un marchio è un simbolo che distingue beni e servizi da beni e servizi simili di altri.UN                                   |
|                                                                                                                            |
|il marchio è un simbolo che distingue i prodotti e servizi di un'azienda dai prodotti simili e                              |
|                                                                                                                            |
|servizi di altre società. Un marchio rappresenta un mezzo di distinzione nel mercato.                                       |
|                                                                                                                            |
|Un marchio è anche un diritto esclusivo. Conferisce al titolare il diritto esclusivo di utilizzare il marchio nel marketing,|
|                                                                                                                            |
|imballaggio o documenti commerciali dei prodotti o servizi o in qualsiasi altro modo, anche per via orale.                  |
|                                                                                                                            |
|Esistono diversi tipi di marchi. Un marchio può, per esempio, essere una parola, una figura, uno slogan o persino un suono. |
|                                                                                                                            |
|Quando registri il tuo marchio, otterrai protezione per questo per dieci anni. La protezione fornita da                     |
|                                                                                                                            |
|la registrazione inizia alla data della domanda e può essere rinnovata ogni dieci anni ";                                   |
|                                                                                                                            |
|    \ |STYLE4|\  <https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/                                    |
|                                                                                                                            |
|8566c45a-8b9e-46d5-8371-81c8ad002362 & regione = helsinki>;                                                                 |
|                                                                                                                            |
|    \ |STYLE5|\  <http://publications.europa.eu/resource/authority/language/ENG>;                                           |
|                                                                                                                            |
|    \ |STYLE6|\  <http://europa.eu/youreurope/businessOntology#start-grow>;                                                 |
|                                                                                                                            |
|\ |STYLE7|\  <https://www.prh.fi/input/form>;                                                                               |
|                                                                                                                            |
|    \ |STYLE8|\  <https://www.prh.fi/output/result>;                                                                        |
|                                                                                                                            |
|    \ |STYLE9|\  <https://www.prh.fi/channel/online>;                                                                       |
|                                                                                                                            |
|\ |STYLE10|\  <https://www.prh.fi/channel/mail>;                                                                            |
|                                                                                                                            |
|    \ |STYLE11|\  <https://www.prh.fi/input/cost>.                                                                          |
|                                                                                                                            |
|                                                                                                                            |
+----------------------------------------------------------------------------------------------------------------------------+

 

.. _h9429c3c395c1484f577ec522a64:

5.2.  Classe evento aziendale
*****************************

\ |STYLE12|\ 


+------------------+--------------------------------------------------------------------------------------------------+
|Proprietà         |Valore                                                                                            |
+------------------+--------------------------------------------------------------------------------------------------+
|Identifier        |http://europa.eu/youreurope/businessOntology#start-grow                                           |
+------------------+--------------------------------------------------------------------------------------------------+
|Nome              |Inizia e cresci                                                                                   |
+------------------+--------------------------------------------------------------------------------------------------+
|genere            |Registrazione della proprietà intellettuale                                                       |
+------------------+--------------------------------------------------------------------------------------------------+
|Servizio correlato|https://www.yrityssuomi.fi/en/palvelu/-/palvelu/electronicapplicationforatrademark?region=helsinki|
+------------------+--------------------------------------------------------------------------------------------------+

 

\ |STYLE13|\ 


+------------------------------------------------------------------------------+
|<http://europa.eu/youreurope/businessOntology#start-grow> a cv: BusinessEvent;|
|                                                                              |
|\ |STYLE14|\  "Start & grow";                                                 |
|                                                                              |
|\ |STYLE15|\  <http://127.0.0.1:3333/Registrazione+proprietà \ |STYLE16|\  >; |
|                                                                              |
|\ |STYLE17|\                                                                  |
|                                                                              |
|    / palvelu / electronicapplicationforatrademark? region = helsinki>.       |
|                                                                              |
|                                                                              |
+------------------------------------------------------------------------------+

 

.. _hd6b63204f142f5d7a21602c5c251459:

5.3. Prova
**********

\ |STYLE18|\ 


+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Proprietà               |Valore                                                                                                                                                                                                          |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Identifier              |https://www.prh.fi/input/form                                                                                                                                                                                   |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Nome                    |Modulo per richiedere un marchio                                                                                                                                                                                |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Descrizione             |La domanda deve includere il nome del richiedente o il nome della società, il domicilio o la sede legale e l'indirizzo. Un marchio può essere richiesto da una società, un'organizzazione o una persona privata.|
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|linguaggio              |http://publications.europa.eu/resource/authority/language/FIN                                                                                                                                                   |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|linguaggio              |http://publications.europa.eu/resource/authority/language/SWE                                                                                                                                                   |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Documentazione correlata|https://www.prh.fi/stc/forms/tavaramerkin_rekisterointihakemus.pdf                                                                                                                                              |
+------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

 

\ |STYLE19|\ 


+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|<https://www.prh.fi/input/form> a cv: Evidence;                                                                                                                                                                                |
|                                                                                                                                                                                                                               |
|\ |STYLE20|\ "Modulo da applicare per un marchio";                                                                                                                                                                             |
|                                                                                                                                                                                                                               |
|\ |STYLE21|\ "La domanda deve includere il nome o il nome della società, il domicilio o la sede legale e l'indirizzo del richiedente. Un marchio può essere richiesto da una società, un'organizzazione o una persona privata";|
|                                                                                                                                                                                                                               |
|\ |STYLE22|\ <http://publications.europa.eu/resource/authority/language/FIN>;                                                                                                                                                  |
|                                                                                                                                                                                                                               |
|\ |STYLE23|\ <http://publications.europa.eu/resource/authority/language/SWE>;                                                                                                                                                  |
|                                                                                                                                                                                                                               |
|    \ |STYLE24|\                                                                                                                                                                                                               |
|                                                                                                                                                                                                                               |
|                                                                                                                                                                                                                               |
+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

 

.. _h1f5713c5f7b74486c20782232742f:

5.4.  Produzione
****************

\ |STYLE25|\ 


+----------+--------------------------------+
|Proprietà |Valore                          |
+----------+--------------------------------+
|Identifier|https://www.prh.fi/output/result|
+----------+--------------------------------+
|Nome      |Marchio                         |
+----------+--------------------------------+
|genere    |Riconoscimento                  |
+----------+--------------------------------+

 

\ |STYLE26|\ 


+----------------------------------------------------+
|<https://www.prh.fi/output/result> a cv: Output;    |
|                                                    |
|\ |STYLE27|\ "Trademark";                           |
|                                                    |
|\ |STYLE28|\ <http://127.0.0.1:3333/Riconoscimento>.|
+----------------------------------------------------+

 

.. _h5366d3971223278371763ac554b:

5.5.  Canale
************

\ |STYLE29|\ 


+------------+-----------------------------------------------------------------------------------------------------------------------+
|Proprietà   |Valore                                                                                                                 |
+------------+-----------------------------------------------------------------------------------------------------------------------+
|Identifier  |https://www.prh.fi/channel/online                                                                                      |
+------------+-----------------------------------------------------------------------------------------------------------------------+
|Posseduto da|https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/8566c45a-8b9e-46d5-8371-81c8ad002362®ion=helsinki|
+------------+-----------------------------------------------------------------------------------------------------------------------+

 

\ |STYLE30|\ 


+------------+-----------------------------------------------------------------------------------------------------------------------+
|Proprietà   |Valore                                                                                                                 |
+------------+-----------------------------------------------------------------------------------------------------------------------+
|Identifier  |https://www.prh.fi/channel/mail                                                                                        |
+------------+-----------------------------------------------------------------------------------------------------------------------+
|Posseduto da|https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/8566c45a-8b9e-46d5-8371-81c8ad002362®ion=helsinki|
+------------+-----------------------------------------------------------------------------------------------------------------------+
|Ha input    |https://www.prh.fi/stc/forms/tavaramerkin_rekisterointihakemus.pdf                                                     |
+------------+-----------------------------------------------------------------------------------------------------------------------+

 

\ |STYLE31|\ 


+------------------------------------------------------------------------------------+
|<https://www.prh.fi/channel/online> a cv: Channel;                                  |
|                                                                                    |
|\ |STYLE32|\ <https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/|
|                                                                                    |
|8566c45a-8b9e-46d5-8371-81c8ad002362 & regione = helsinki>.                         |
|                                                                                    |
|<https://www.prh.fi/channel/mail> a cv: Channel;                                    |
|                                                                                    |
|\ |STYLE33|\ <https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/|
|                                                                                    |
|8566c45a-8b9e-46d5-8371-81c8ad002362 & regione = helsinki>;                         |
|                                                                                    |
|\ |STYLE34|\ <https://www.prh.fi/stc/forms/tavaramerkin_rekisterointihakemus.pdf>.  |
+------------------------------------------------------------------------------------+

 

 

 

.. _h64736524791576aa6f2711836701e:

5.6. Organizzazione pubblica
****************************

\ |STYLE35|\ 


+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Proprietà            |Valore                                                                                                                 |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Identifier           |https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/8566c45a-8b9e-46d5-8371-81c8ad002362®ion=helsinki|
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Nome                 |L'ufficio finlandese di registrazione e brevetti (PRH)                                                                 |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Etichetta preferita  |L'ufficio di registrazione e brevetti finlandese                                                                       |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Etichetta alternativa|PRH                                                                                                                    |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Ha un indirizzo      |http://www.prh.fi/address                                                                                              |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+
|Spaziale             |http://publications.europa.eu/resource/authority/atu/FIN                                                               |
+---------------------+-----------------------------------------------------------------------------------------------------------------------+

 

\ |STYLE36|\ 


+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|\ |STYLE37|\                                                                                                                                                         |
|                                                                                                                                                                     |
|\ |STYLE38|\ "L'ufficio finlandese di registrazione e brevetti (PRH)";                                                                                               |
|                                                                                                                                                                     |
|\ |STYLE39|\ "L'ufficio di registrazione e brevetti finlandese";                                                                                                     |
|                                                                                                                                                                     |
|\ |STYLE40|\ "PRH";                                                                                                                                                  |
|                                                                                                                                                                     |
|\ |STYLE41|\ <http://ec.europa.eu/taxation_customs/resources/documents/taxation/vat/traders/vat_refunds/refund_contact_details_table_en.pdf#country/Belgium/Address>;|
|                                                                                                                                                                     |
|\ |STYLE42|\ <http://publications.europa.eu/resource/authority/atu/FIN>                                                                                              |
|                                                                                                                                                                     |
|                                                                                                                                                                     |
+---------------------------------------------------------------------------------------------------------------------------------------------------------------------+

 

.. bottom of content


.. |STYLE0| replace:: **Tabella 2 : Esempio di classe di servizio pubblico: leggibile dall'uomo**

.. |STYLE1| replace:: **Tabella 3 : Esempio di classe di servizio pubblico: leggibile dalla macchina**

.. |STYLE2| replace:: **dct: titolo**

.. |STYLE3| replace:: **DCT: Descrizione**

.. |STYLE4| replace:: **cv: hasCompetentAuthority**

.. |STYLE5| replace:: **dct: lingua**

.. |STYLE6| replace:: **cv: isGroupedBy**

.. |STYLE7| replace:: **cpsv: hasInput**

.. |STYLE8| replace:: **cpsv: produce**

.. |STYLE9| replace:: **cv: hasChannel**

.. |STYLE10| replace:: **cv: hasChannel**

.. |STYLE11| replace:: **cv: hasCost**

.. |STYLE12| replace:: **Tabella 4 : Esempio di classe Evento aziendale: leggibile dall'uomo**

.. |STYLE13| replace:: **Tabella 5 : Esempio di classe di servizio pubblico: leggibile dalla macchina**

.. |STYLE14| replace:: **dct: titolo**

.. |STYLE15| replace:: **dct: digita**

.. |STYLE16| replace:: **intellettuale**

.. |STYLE17| replace:: **dct: relation <https://www.yrityssuomi.fi/en/palvelu/-**

.. |STYLE18| replace:: **Tabella 6 : Esempio di classe Evidence: leggibile dall'uomo**

.. |STYLE19| replace:: **Tabella 7 : Esempio di classe Evidence - Machine readable**

.. |STYLE20| replace:: **dct: titolo**

.. |STYLE21| replace:: **dct: descrizione**

.. |STYLE22| replace:: **dct: lingua**

.. |STYLE23| replace:: **dct: lingua**

.. |STYLE24| replace:: **foaf: pagina <https://www.prh.fi/stc/forms/tavaramerkin_rekisterointihakemus.pdf>.**

.. |STYLE25| replace:: **Tabella 8 : Esempio di classe Formal Framework: leggibile dall'uomo**

.. |STYLE26| replace:: **Tabella 9 : Esempio di classe di output: leggibile dalla macchina**

.. |STYLE27| replace:: **dct: titolo**

.. |STYLE28| replace:: **dct: digita**

.. |STYLE29| replace:: **Tabella 10 : Esempio di Channel Class 1 - Human readable**

.. |STYLE30| replace:: **Tabella 11 : Esempio di Channel Class 2 - Human readable**

.. |STYLE31| replace:: **Tabella 12 : esempio di classe di canale - leggibile dalla macchina**

.. |STYLE32| replace:: **cv: isOwnedBy**

.. |STYLE33| replace:: **cv: ownedBy**

.. |STYLE34| replace:: **cv: hasInput**

.. |STYLE35| replace:: **Tabella 13 : Esempio di classe di organizzazione pubblica : leggibile dall'uomo**

.. |STYLE36| replace:: **Tabella 14 : Esempio di classe di organizzazione pubblica : leggibile dalla macchina**

.. |STYLE37| replace:: **<https://www.yrityssuomi.fi/en/organisaatio?id=workspace://SpacesStore/8566c45a-8b9e-46d5-8371-81c8ad002362®ion=helsinki> a cv: PublicOrganisation;**

.. |STYLE38| replace:: **dct: titolo**

.. |STYLE39| replace:: **skos: prefLabel**

.. |STYLE40| replace:: **skos: altLabel**

.. |STYLE41| replace:: **cv: hasAddress**

.. |STYLE42| replace:: **spaziale**


.. rubric:: Footnotes

.. [#f1]   `https://www.yrityssuomi.fi/en/?region=helsinki <https://www.yrityssuomi.fi/en/?region=helsinki>`__  
