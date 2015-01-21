==============================================
Otevírání geografických dat - Případová studie
==============================================

.. rubric:: Anotace

Tato případová studie shrnuje výsledky konzultací v oblasti otevírání
geografických dat, provedených ve prospěch `Institutu plánování a
rozvoje hlavního města Prahy <http://www.iprpraha.cz/>`_ (*IPR Praha*),
který vznik dokumentu finančně podpořil. Zástupci IPR Praha měli
velice kvalifikovaný a ucelený názor na celou problematiku. Konzultace
byly zaměřeny na celkový koncept otevírání dat a na technické pasáže,
kde byla potřeba většího detailu, doporučení vhodného postupu,
případně navržení řešení.  Tomu odpovídá i struktura dokumentu, která
nemusí být vždy zcela přehledná a dostatečně obecná.

Na základě našich zkušeností z praxe nastiňuje případná technická úskalí a
problémy, se kterými je třeba počítat, mají-li být publikovaná data dostupná co
nejširšímu okruhu uživatelů. Spíše než jednotlivými nástroji, které jsou v mnoha
ohledech věcí osobních preferencí, jsme se zabývali obecnými principy, které je
v souvislosti s otevíráním geografických dat potřeba respektovat. V textu jsme se snažili
maximálně zúročit naše praktické zkušenosti s různě kvalitními geografickými
daty a informačními systémy pro jejich správu. Cílem bylo shromáždit a utřídit
přehled témat, které usnadní navržení konkrétního řešení pro otevírání geografických dat.

.. rubric:: Licence

..
            .. image:: imgs/cc-by-sa.png
           
Dokument podléhá licenci *Creative Commons 4.0
BY-SA*. Informace o podrobnostech licence najdete na adrese
http://www.creativecommons.cz/.

.. rubric:: Spolupráce

Text studie můžete stáhnout ze serveru GitHub [#github-url]_ a dále rozšiřovat
standardními postupy (*fork*, *pull request*).

.. raw:: latex
    
         \clearpage
.. rubric:: Revize dokumentu

.. tabularcolumns:: |p{2cm}|p{1.5cm}|p{4cm}|p{6.5cm}|
         
+------------+------------+-------------------------------+---------------------------------+
| **Datum**  | **Revize** | **Editoři**                   | **Popis**                       |
+============+============+===============================+=================================+
| 2014-09-30 | 1.0.0      | Jáchym Čepický, Martin Landa, | První verze dokumentu.          |
|            |            | Radek Augustýn, Jan Cibulka,  |                                 |
|            |            | Jan Michálek                  |                                 |
+------------+------------+-------------------------------+---------------------------------+
| 2014-10-03 | 1.0.1      | Radek Augustnýn               | Drobné revize formátování.      |
+------------+------------+-------------------------------+---------------------------------+
| 2014-10-05 | 1.0.2      | Jáchym Čepický, Martin Landa, | Jazyková korektura textu.       |
|            |            | Radek Augustýn, Jan Michálek  |                                 |
+------------+------------+-------------------------------+---------------------------------+
| 2014-11-03 | 2.0.0      | Jáchym Čepický, Martin Landa, | Druhá verze dokumentu.          |
|            |            | Radek Augustýn, Jan Michálek, | Zapracování připomínek          |
|            |            | Lucie Prunarová               | IPR Praha.                      |
+------------+------------+-------------------------------+---------------------------------+
| 2014-11-06 | 2.1.0      | Jáchym Čepický                | Převod dokumentu do             |
|            |            |                               | formátu reStructuredTex a jeho  |
|            |            |                               | publikování na serveru          |
|            |            |                               | Git\-Hub.                       |
+------------+------------+-------------------------------+---------------------------------+
| 2014-12-01 | 2.2.0      | Jáchym Čepický, Martin Landa, | Revize textu dle připomínek     |
|            |            | Lucie Prunarová               | zástupců IPR Praha, seznam      |
|            |            |                               | zkratek, přeformátování         |
|            |            |                               | struktury.                      |
+------------+------------+-------------------------------+---------------------------------+
| 2015-01-02 | 2.2.1      | Lucie Prunarová,              | Revize textu, doplnění zkratek. |
|            |            | Jáchym Čepický                |                                 |
+------------+------------+-------------------------------+---------------------------------+
| 2015-01-21 | 2.2.1      | Lucie Prunarová,              | Začlenění připomínek k verzi    |
|            |            | Jáchym Čepický                | 2.2.1.                          |
+------------+------------+-------------------------------+---------------------------------+

.. raw:: latex
    
         \clearpage

.. rubric:: Seznam zkratek

.. tabularcolumns:: p{5cm}p{9cm}
         
+------------+-----------------------------------------------------------------+
| **Zkratka**| **Význam**                                                      |
+============+=================================================================+
| AOPK       | Agentura ochrany přírody a krajiny ČR                           |
+------------+-----------------------------------------------------------------+
| ATOM       | Atom Syndication Format je webový standard pro publikování      |
|            | syndikovaného obsahu (obsahu, kterému byly zpětně dodány        |
|            | aktuální informace)                                             |
+------------+-----------------------------------------------------------------+
| DBF        | dBase byl první masověji rozšířený systém řízení báze dat       |
+------------+-----------------------------------------------------------------+
| CAD        | Z angličtiny computer-aided design, česky počítačem podporované |
|            | projektování                                                    |
+------------+-----------------------------------------------------------------+
| CSV        | Comma-separated values (hodnoty oddělené čárkami) je jednoduchý |
|            | souborový formát určený pro výměnu tabulkových dat.             |
+------------+-----------------------------------------------------------------+
| CSW        | Catalogue Service for Web (přístup k informacím katalogu), OGC  |
|            | specifikace                                                     |
+------------+-----------------------------------------------------------------+
| ČSN        | Chráněné označení českých technických norem                     |
+------------+-----------------------------------------------------------------+
| ČÚZK       | Český úřad zeměměřičský a katastrální                           |
+------------+-----------------------------------------------------------------+
| EPSG       | European Petroleum Survey Group. Jedná se o široce využívanou   |
|            | databázi zemských elipsoidů, geodetických dat, zeměpisných a    |
|            | kartografických souřadnicových systémů, měrných jednotek, atd.  |
+------------+-----------------------------------------------------------------+
| ETRS89     | Evropský terestrický referenční systém, závazný geodetický      |
|            | referenční systém na celém území státu, definovaný technologiemi|
|            | kosmické geodézie a konstantami, které jsou součástí programů   |
|            | mezinárodních zpracovatelských center, souborem geocentrických  |
|            | souřadnic vybraných bodů geodetických základů, jejichž          |
|            | souřadnice byly vztaženy k epoše 1989.                          |
+------------+-----------------------------------------------------------------+
| FES        | Filter Encoding Specification je standard OGC, který popisuje   |
|            | na systému nezávislou syntaxi pro vyjádření výběru a třídění    |
|            | potřebné při dotazování se na objekty datových sad.             |
+------------+-----------------------------------------------------------------+
| GeoTIFF    | Rastrový formát pro geografická data postavený na formátu TIFF  |
+------------+-----------------------------------------------------------------+
| GeoJSON    | Vektorový formát pro geografická data využívaný především v     |
|            | prostředí webových aplikací                                     |
+------------+-----------------------------------------------------------------+
| GIF        | Graphics Interchange Format, souborový formát určený pro        |
|            | rastrovou grafiku                                               |
+------------+-----------------------------------------------------------------+
| GIS        | Geografický informační systém                                   |
+------------+-----------------------------------------------------------------+
| GML        | Geography Markup Language je na XML založený formát pro         |
|            | vektorová geografická data, OGC specifikace                     |
+------------+-----------------------------------------------------------------+
| GPS        | Global Positioning System, česky Globální polohovací systém     |
+------------+-----------------------------------------------------------------+
| HTML       | HyperText Markup Language, je značkovací jazyk pro hypertext.   |
|            | Je hlavním z jazyků pro vytváření stránek v systému World Wide  |
|            | Web, který umožňuje publikaci dokumentů na Internetu.           |
+------------+-----------------------------------------------------------------+
| HTTP       | Hypertext Transfer Protocol) je internetový protokol určený pro |
|            | výměnu hypertextových dokumentů ve formátu HTML.                |
+------------+-----------------------------------------------------------------+
| INSPIRE    | INfrastructure for SPatial InfoRmation in Europe je iniciativou |
|            | Evropské komise pro vybudování evropské                         |
|            | infrastruktury prostorových informací.                          |
+------------+-----------------------------------------------------------------+
| IPR Praha  | Institut plánování a rozvoje hl. m. Prahy                       |
+------------+-----------------------------------------------------------------+
| ISO        | Mezinárodní organizace pro normalizaci                          |
+------------+-----------------------------------------------------------------+
| JSON       | JavaScript Object Notation (JavaScriptový objektový zápis,      |
|            | JSON) je datový formát určený pro přenos dat                    |
+------------+-----------------------------------------------------------------+
| JPEG       | Metoda ztrátové komprese používané pro ukládání počítačových    |
|            | obrázků ve fotorealistické kvalitě.                             |
+------------+-----------------------------------------------------------------+
| KML        | Keyhole Markup Language je aplikací metajazyka XML pro          |
|            | publikaci, distribuci geografických dat                         |
+------------+-----------------------------------------------------------------+
| LPIS       | Veřejný registr půdy                                            |
+------------+-----------------------------------------------------------------+
| OGC        | Open Geospatial Consortium,  mezinárodní standardizační         |
|            | organizace pro oblast GIS a geoprostorových dat                 |
+------------+-----------------------------------------------------------------+
| OSM        | OpenStreetMap je projekt, jehož cílem je tvorba volně           |
|            | dostupných geografických dat                                    |
+------------+-----------------------------------------------------------------+
| OWS        | Open Web Services, skupina otevřených webových služeb podle     |
|            | standardů OGC                                                   |
+------------+-----------------------------------------------------------------+
| PNG        | Portable Network Graphics je grafický formát určený pro         |
|            | bezeztrátovou kompresi rastrové grafiky                         |
+------------+-----------------------------------------------------------------+
| RÚIAN      | Registr územní identifikace, adres a nemovitostí                |
|            | je jedním ze základních registrů ČR                             |
+------------+-----------------------------------------------------------------+
| SHP        | Formát vektorových dat Esri Shapefile                           |
+------------+-----------------------------------------------------------------+
| SDI        | Spatial Data Infrastructure                                     |
+------------+-----------------------------------------------------------------+
| S-JTSK     | Jednotná trigonometrická síť katastrální (JTSK, někdy S–JTSK)   |
|            | je pravoúhlá souřadnicová síť používaná v geo\-dézii na území   |
|            | České republiky a Slovenska                                     |
+------------+-----------------------------------------------------------------+
| SOS        | Sensor Observation Service, standard OGC OWS (otevřené webové   |
|            | služby podle OGC). SOS umožňuje klientům získat ze serverů různá|
|            | sensorová data a údaje o pozorování z nich.                     |
+------------+-----------------------------------------------------------------+
| SQL        | Structured Query Language je standardizovaný dotazovací         |
|            | jazyk používaný pro práci s daty v relačních databázích.        |
+------------+-----------------------------------------------------------------+
| TIFF       | Tag Image File Format je jeden ze souborových formátů           |
|            | pro ukládání rastrové počítačové grafiky.                       |
+------------+-----------------------------------------------------------------+
| TMS        | Tile Map Service, OGC specifikace                               |
+------------+-----------------------------------------------------------------+
| TopoJSON   | TopoJSON je extenze pro GeoJSON umožňující uložení vektorových  |
|            | dat v topologické formě                                         |
+------------+-----------------------------------------------------------------+
| URI        | Uniform Resource Identifier (jednotný identifikátor             |
|            | zdroje) je textový řetězec s definovanou strukturou, který      |
|            | slouží k přesné specifikaci zdroje informací na Internetu       |
+------------+-----------------------------------------------------------------+
| URL        | Uniform Resource Locator (jednotná adresa zdroje) je            |
|            | řetězec znaků s definovanou strukturou, který slouží k přesné   |
|            | specifikaci umístění zdrojů informací na Internetu              |
+------------+-----------------------------------------------------------------+
| VDP        | Veřejný dálkový přístup (viz RÚIAN)                             |
+------------+-----------------------------------------------------------------+
| VFR        | Výměnný formát RÚIAN                                            |
+------------+-----------------------------------------------------------------+
| VFK        | Výměnný formát katastru nemovitostí                             |
+------------+-----------------------------------------------------------------+
| WCS        | Web Coveradge Service, standard OGC OWS (otevřené webové služby |
|            | podle  OGC), umožňující klientovi požadovat po serveru obrazová |
|            | (rastrová) data                                                 |
+------------+-----------------------------------------------------------------+
| WFS        | Web Feature Service, standard OGC OWS (otevřené webové služby   |
|            | podle  OGC), umožňující klientovi požadovat po serveru          |
|            | vektorová data                                                  |
+------------+-----------------------------------------------------------------+
| WGS 84     | World Geodetic System 1984, česky Světový                       |
|            | geodetický systém 1984                                          |
+------------+-----------------------------------------------------------------+
| WMS        | Web Map Service, standard OGC OWS (otevřené webové služby podle |
|            | OGC), umožňující klientovi požadovat po serveru vyrenderované   |
|            | obrázky mapových kompozic                                       |
+------------+-----------------------------------------------------------------+
| WMTS       | Web Map Tile Service, OGC specifikace                           |
+------------+-----------------------------------------------------------------+
| WWW        | World Wide Web, soustava propojených hypertextových (na sebe    |
|            | navzájem odkazujících) dokumentů                                |
+------------+-----------------------------------------------------------------+
| XML        | Extensible Markup Language (rozšiřitelný značkovací jazyk) je   |
|            | obecný značkovací jazyk, který byl vyvinut a standardizován     |
|            | konsorciem W3C                                                  |
+------------+-----------------------------------------------------------------+
| XML-RPC    | Protokol, s jehož pomocí lze velice jednoduše                   |
|            | provádět vzdálené volání procedur.                              |
+------------+-----------------------------------------------------------------+
| XSD        | XML Schema XSD je jedno z XML schémat, jazyků pro popis XML.    |
+------------+-----------------------------------------------------------------+
| XSLT       | eXtensible Stylesheet Language Transformations (Transformace    |
|            | XSLT) slouží k převodům zdrojových dat ve formátu XML           |
|            | do libovolného jiného požadovaného formátu                      |
+------------+-----------------------------------------------------------------+
| ZCHÚ       | Zvláště chráněná území                                          |
+------------+-----------------------------------------------------------------+

.. only:: html

    .. rubric:: Obsah

.. toctree::
    :maxdepth: 2

    uvod
    opendata
    otevirani
    bib

.. raw:: latex
    
         % Set up the appendix mode and modify the LaTex toc behavior
         \appendix
         %\noappendicestocpagenum
         %\addappheadtotoc
         %\settocdepth{chapter}

.. toctree::
    :maxdepth: 2
    
    priloha-a
    priloha-b
    priloha-c
    priloha-d
    priloha-e
    priloha-f
    priloha-g

.. only:: html

	  .. rubric:: Poznámky pod čarou

.. [#github-url] https://github.com/OpenGeoLabs/otevrena-geodata/
