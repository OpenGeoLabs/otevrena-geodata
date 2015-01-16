.. index::
    single: Formát
    see: Formát souboru; Formát

#################################################
Technické a právní aspekty otevírání datových sad
#################################################

**********************************
Výběr licence pro otevřená geodata
**********************************

.. note:: Autoři následující kapitoly nejsou právníci, pouze popisují své
    zkušenosti v dané oblasti. Před aplikací doporučení z tohoto textu je proto důrazně doporučeno
    jej konzultovat s expertem na autorské právo.

Otevíraná data by měla být licencovaná tak, aby na straně jedné zbytečně
neomezovala uživatele a na straně druhé dostatečně chránila práva poskytovatele
dat. Podstatné podmínky tedy jsou:

* Uživatel smí data kopírovat a využívat v rámci své činnosti, rovněž smí
  poskytnutá data začlenit do svého díla
* Uživatel nesmí přeprodávat původní data
* Uživatel musí vždy uvést zdroj dat a licenci; nesmí tak ale činit způsobem,
  který naznačuje, že je podporován poskytovatelem dat

Od nového roku upravuje problematiku licenčních smluv nový občanský zákoník
(část čtvrtá, hlava druhá, díl druhý, oddíl 5). Podstatný je § 2373 odst. 1),
který umožňuje projevit vůli k uzavření smlouvy i směrem k *“neurčitému počtu
osob”*. Dále tento odstavec obsahuje ustanovení, že *“Obsah smlouvy nebo jeho část
lze určit také odkazem na licenční podmínky, jež jsou stranám známé nebo veřejně
dostupné.”*

Následující paragraf pak umožňuje vyjádřit “souhlas s návrhem na uzavření
smlouvy provedením určitého úkonu bez vyrozumění navrhovatele, zejména
poskytnutím nebo přijetím plnění.”

Poskytovatel může data opatřit licenčními podmínkami, které uživatel přijme
samotným užíváním díla. Podmínkou je, aby byl text licence uživateli dat volně
dostupný.

Tuzemská státní správa už tento způsob licencování místy využívá, jde konkrétně o
licenci Creative Commons [ref47]_. Obsah pod touto licencí zveřejňují Český
hydrometeorologický úřad, Ústav zdravotnických informací a statistiky ČR či
Celní správa.

**************************************************************
Otevřené formáty, webové služby a distribuce otevřených geodat
**************************************************************

Tato kapitola se zabývá formáty otevřených geodat.
Jsou zde popsány populární datové formáty, které jsou ale pro účel otevírání dat nevhodné i nové,
rychle se rozvíjející vhodné formáty.
Podrobněji jsou zde zhodnoceny dostupné webové služby jako vhodný a široce využívaný
způsob distribuce geodat.

**Formát** určuje význam dat v elektronickém souboru. Formát je způsob, jakým jsou
data v souboru uložena. Formáty jsou často navrženy specificky pro
určitý typ dat. V základu lze formáty rozdělit na binární (z pohledu člověka se
jedná o souvislý tok hodnot 0 a 1) a textové (které jsou pro člověka poměrně jednoduše
čitelné). Příkladem binárního formátu může být JPEG speciálně navržený k
ukládání obrazových dat. Příkladem textového formátu může být formát JSON či XML
určený k popisu a ukládání libovolných stromových datových struktur.

**Webové služby** jsou softwarové systémy umožňující interakci dvou strojů v
počítačové síti. Počítače mezi sebou komunikují pomocí strojově zpracovatelného formátu
zpráv. Webové služby ke své komunikaci využívají protokolu HTTP (Hypertext
Transfare Protocol), o který je opřen World Wide Web (WWW -- odtud webové
služby). Jeden z počítačů ve vzájemné komunikaci vždy
vystupuje jako klient (požaduje po serveru splnění nějakého úkolu), druhý jako
server (vyřizuje žádost a posílá klientovi odpověď). Výsledkem odpovědi může
například být i obrázek v patřičném souborovém formátu, jako je např. JPEG.

Legislativní pravidla otevírání dat - INSPIRE
---------------------------------------------

Kromě souvisejících zákonů a nařízení je pro otevírání geodat relevantní zejména
evropská směrnice INSPIRE [ref26]_ ze dne 25. dubna 2007, která vstoupila v platnost
15. května 2007. Tato směrnice tvoří evropský legislativní rámec potřebný k
vybudování evropské infrastruktury prostorových informací zejména k podpoře
environmentálních politik a politik, které životní prostředí ovlivňují.
Hlavním cílem směrnice INSPIRE je poskytnout množství kvalitních a
standardizovaných prostorových informací. Směrnice byla transponována do
národní legislativy České republiky novelou zákona č. 380/2009 Sb. [ref27]_.  

.. index:: 
    single: Formáty
    see: Otevřené formáty; Formáty

================
Otevřené formáty
================
Formáty pro publikování otevřených geodat by měly být zejména otevřené -- ať už
proprietární, tj. spravované konkrétní firmou anebo standardizované
konsorciem OGC či technickou
normou ISO. Otevřený formát je takový formát, ke kterému existuje
volně dostupná dokumentace a zároveň jeho licence umožňuje jeho volné
využívání. V ideálním případě je vyvíjen nezávislou mezinárodní
standardizační organizací a není navázán přímo na žádný privátní
subjekt.

Z dlouhodobého hlediska je výhodnější využívat formáty otevřené a
standardizované, než proprietární (jakkoliv mohou být široce rozšířené mezi
uživateli a jimi používanými programy), zejména protože:

* Stává se, že firma (autor proprietárního formátu a držitel licenčních práv k
  němu) svůj formát změní, případné programové nástroje třetích stran
  pak reagují se zpožděním, pokud vůbec 
* Uživatelé jsou nuceni používat konkrétní software, což nemusí být pro některé z
  nich z technických, licenčních nebo finančních důvodů akceptovatelné
* Celý systém se stává závislý na jedné firmě či dodavateli softwarového řešení,
  je nepřenositelný a~v budoucnu jen těžko rozšiřitelný

Z pohledu výše zmíněné :ref:`pětihvězdičkové konvence
<pet-hvezdicek>`, můžeme pro geodata uvést následující příklady
vhodných datových formátů:

.. tabularcolumns:: p{.1\textwidth}p{.8\textwidth}

+-------+--------------------------------------------------------------------------------+
| ★     | Tisknutelná mapa je uložena ve formátu PDF nebo v rastrovém formátu jako       |
|       | obrázek, například JPEG, GIF či PNG                                            |
+-------+--------------------------------------------------------------------------------+
| ★★    | Vektorová data jsou uložena v uzavřeném proprietárním formátu, například DWG   |
|       | firmy Autodesk                                                                 |
+-------+--------------------------------------------------------------------------------+
| ★★★   | Vektorová data jsou uložena ve formátu  SHPP který j e sice                    |
|       | proprietární, ale je otevřený; nebo jako GML, což je otevřený standard a       |
|       | zároveň technická norma ISO                                                    |
+-------+--------------------------------------------------------------------------------+
| ★★★★  | Data jsou opatřena metadaty a jednotlivé datové sady jsou jimi navzájem        |
|       | provázány. Předpokládá se existence metadatového katalogu, založeného na       |
|       | standardu OGC CSW, ve kterém lze data a služby                                 |
|       | vyhledávat                                                                     |
+-------+--------------------------------------------------------------------------------+
| ★★★★★ | Jednotlivé soprvkyvky datové sadu avzájem provázány pomocí unikátních          |
|       | identifikátorů                                                                 |
+-------+--------------------------------------------------------------------------------+

Formáty souborů pro distribuci otevřených geodat
------------------------------------------------

Pro ukládání, zpracování a výměnu geodat existuje velké množství
formátů. Z hlediska otevřených dat se prozatím můžeme omezit na formáty
rastrové a vektorové. 

.. index::
    single: Rastry
    pair: GeoTIFF; TIFF
    single: JPEG
    single: PNG
    single: GIF

Rastrová data
^^^^^^^^^^^^^

"""""""
GeoTIFF
"""""""

Formát GeoTIFF [ref16]_ je typickým a nejrozšířenějším otevřeným formátem pro
distribuci rastrových geodat. Tento formát umožňuje uložit nejen
rastrová data, ale také všechny typy gridových dat. Informace o souřadnicovém
systému, souřadnicovém umístění a další popisné informace jsou uloženy přímo v
hlavičce  souboru. Při uložení dat do tohoto formátu nedochází při vhodné volbě
komprese k nevratné ztrátě informace.

""""
JPEG
""""

Formát JPEG [ref17]_ je kompresní formát určený k uložení rastrových souborů. Jeho výhodou
je úspora místa a tudíž i menší nároky na datový přenos. Jeho nevýhodou je to,
že komprese je ztrátová -- formát tedy není vhodný pro použití v GIS, neboť data
jsou nenávratně poškozena a jsou tak pro další zpracování nepoužitelná. Na
druhou stranu, pokud obrázek JPEG je použit pouze jako podkladová vrstva (např.
u leteckých snímků, u kterých se nepředpokládá žádné jiné využití), lze tak
snížit nároky na datový tok. Soubory ve formátu JPEG jsou nejčastěji výsledkem volání WMS služby. Pokud jsou soubory šířeny samostatně, je potřeba je opatřit metadatovým
souborem se souřadicovým umístěním (koncovka .jpw).

"""
PNG
"""

Formát PNG [ref76]_ byl vytvářen jako nástupce formátů JPEG a GIF kvůli softwarovým
patentům, které jsou v nich použité. Způsob komprese nepoškozuje ostré hrany. Z tohoto
důvodu se tento formát využívá pro
topografické podkladové mapy v prohlížecích službách WMS a WMTS. Komprese
fotografií s množstvím gradientů již není tak efektivní. Pro uložení geodat je
tento formát opět nevhodný, kvůli limitu barevné škály, částečně ztrátové
kompresi dat a omezení na 3 barevné kanály + průhlednost. Soubory ve formátu PNG
jsou nejčastěji výsledkem volání WMS služby. Pokud jsou soubory šířeny
samostatně, je potřeba je opatřit metadatovým souborem se souřadnicovým umístěním
(koncovka .pnw).

"""
GIF
"""
Formát GIF měl své využití v minulosti hlavně
mezi webovými mapovými aplikacemi. GIF disponuje omezenou barevnou
škálou, pro geodata je nevhodný (nejedná-li se o data binární nebo s rozsahem
hodnot 0-255). Z tohoto důvodu byl GIF nahrazen zmíněným modernějším formátem
PNG. Pro GIF platí to samé, co pro soubory JPEG a PNG, je nejčastěji výsledkem volání WMS služby. Pokud jsou soubory v tomto formátu šířeny samostatně, musí u
nich být přítomen metadatový soubor se souřadnicovým umístěním (koncovka .gfw).

""""""""""""""""""""""""
Ostatní rastrové formáty
""""""""""""""""""""""""

Ostatní formáty pro uložení rastrových dat nedosáhly takového rozšíření v oblasti GIS jako
formát GeoTIFF. Řada z nich je proprietárních a jsou používány často pouze
oborově. Jedná se například o formáty MrSID, BMP, ArcSDE Raster a další.

.. index::
    single: Vektory
    pair: SHP; Esri Shapefile
    single: GML
    single: KML
    tripple: JSON; GeoJSON; TopoJSON
    single: SpatiaLite
    single: GeoPackage
    single: CityGML

.. _citygml:

Vektorová data
^^^^^^^^^^^^^^

"""""""""""""""""""""""""""""
OGC Geography Markup Language
"""""""""""""""""""""""""""""

OGC GML [ref19]_ jako otevřený standard je perspektivním formátem pro přenos
vektorových dat. Jedná se o jednosouborový textový formát založený na
značkovacím jazyce XML, je proto interpretovatelný i bez speciálního software.
Kromě standardizace na úrovni OGC je definován technickou normou ISO 19136.
Vzhledem k tomu je podporován většinou moderních GIS nástrojů. GML je také
předepsaný technickými dokumenty INSPIRE a výchozím formátem služby WFS.

GML se používá jako univerzální formát pro data, která mohou mít i
komplikovanější stromovou strukturu. Díky tomu, že je postaven na XML, je jeho
strojové zpracování jednoduché i běžnými systémy, například pomocí transformace
XSLT.


OGC City GML
""""""""""""

Formát CityGML [ref79]_ je formát založený na XML, určený k reprezentaci souborů
městských objektů ve 3D. Pomocí tohoto formátu je možné reprezentovat třídy,
jejich vazby a~vztahy relevantních topografických objektů ve městech a
respektovat přitom jejich geometrické, topologické a sémantické vlastnosti.
Pomocí tohoto formátu lze dosáhnout také určité generalizace, popsat
hierarchické vazby mezi objekty, agregace atp. 

CityGML je odvozený od formátu GML verze 3 a je vhodný zejména při tvorbě analýz nad daty v městském prostředí, simulací,
správě budov a podobně.

OGC Keyhole Markup Language
"""""""""""""""""""""""""""

OGC KML je určen především pro vizualizaci
jednotlivých prvků geodat. Formát byl původně vyvinut firmou Google a je postavený na jazyce XML. Data v souborech KML, na rozdíl od GML, umožňují použít
pouze souřadnicový systém WGS 84.

KML podporují produkty firmy Google, ale i řada služeb a programů
třetích stran. Bývá často podporován moderními GPS přijímači. V minulosti býval
nasazován ve webových mapových aplikacích, protože je v porovnání s GML menší a obsahuje
zmíněnou informaci o vizualizaci jednotlivých prvků geodat. Ačkoliv byl v době před
cca 3 lety tento formát populární, dnes je často nahrazován formátem GeoJSON.

JSON a jeho odvozené formáty
""""""""""""""""""""""""""""

Populárními formáty se v poslední době stávají formáty odvozené z formátu JSON,
především GeoJSON a TopoJSON. Dalším odvozeným formátem od JSON je formát firma
MabBox [ref82]_ používaným zejména pro předgenerované vektorové soubory uložené
ve formě dlaždic pro rychlejší přenos dat.

Formáty JSON mají své uplatnění především mezi webovými technologiemi.  Oproti
formátům odvozených z XML (GML, KML) mají kratší zápis, což  je výhodné při
přenosech v prostředí Internetu.  Stejně jako při využití formátů odvozených z
XML, je i zde je možné zabezpečit správnost struktury dat to pomocí schémat.

JSON je velice přívětivý k netypovým programovacím jazykům, je srozumitelný
prostým lidským okem. Souřadnicový systém není v těchto formátech jak
specifikovat, předpokládá se, že se jedná o WGS 84. Data lze libovolným způsobem
zanořovat a větvit.

GeoJSON [ref68]_ je využíván u webových služeb pro svůj malý objem a jednoduchost.
Je méně náročný na zpracování, což je vhodné zejména u webových prohlížečů. U
uživatelů mimo svět GIS je oblíbený, protože jeho strukturu je možné rychle
pochopit a připravit vlastní parser.

TopoJSON je druhým formátem odvozeným z formátu JSON, který ale zatím nenabyl takové
popularity jako Geo\-JSON. Hlavním úkolem formátu TopoJSON je
minimalizace datového toku mezi webovým serverem a klientem. Formát je částečně
ztrátový, neboť souřadnice bodů a lomových bodů jsou zapisovány v relativní
poloze od daného počátku a v celých číslech (ztrácí se přesnost). K úspoře
datové velikosti vede také fakt, že např. hranice polygonů jsou uloženy pro dvě
sousedící plochy pouze jednou (formát je tedy topologický).

Formát TopoJSON je velice slibný, v budoucnu se očekává jeho rozšíření. V tuto
chvíli naráží zejména na nedostatečnou podporu v softwarech. Není ani vhodný
jako obecný formát pro výměnu dat mezi systémy. Formát byl navržen s ohledem na
optimalizaci aplikací ve webovém prostředí a tam má taky své místo.

Geodatabáze SpatialLite
"""""""""""""""""""""""

Geodatabáze SpatiaLite je postavená na souborové Open Source databázi SQLite.
SQLite je přítomna v řadě zařízení či programech, interně ji využívá např.
prohlížeč Firefox. SpatiaLite je její prostorové rozšíření, podobně jako PostGIS
pro databázi PostgreSQL. SpatialLite umožňuje uložit a pracovat s geodaty v
prostředí SQL databáze, která je ovšem uložena v jednom jednoduše přenositelném
souboru.

SpatiaLite je vhodný formát na lokální uložení dat, ale v praxi se pro výměnu
dat příliš nepoužívá.

Esri Shapefile
^^^^^^^^^^^^^^

Formát SHP je v praxi již dlouhou dobu nejpoužívanějším
formátem pro výměnu vektorových geodat [ref18]_. Bohužel je tento formát v
dnešní době již poněkud omezující, zejména z~důvodů zmíněných níže.
Stále je ale používán pro menší datové soubory a jednoduché datové sady bez
komplikovaných vazeb mezi objekty a tabulkami, protože je to formát jednoduchý a
poskytuje jistotu kompatibility mezi různými softwarovými platformami.

Mezi slabá místa formátu patří zejména to, že data nejsou uložena v jednom
souboru, ale hned ve trojici (shp+shx+dbf). Různé softwarové produkty si navíc
přidávají vlastní metadatové soubory, které nejsou součástí specifikace tohoto
formátu [#shp]_. Názvy atributů jsou omezeny pouze na deset znaků. Data
neobsahují informaci o znakové sadě, což vede k problémům při automatické
konverzi dat a používání na více operačních systémech. Velikost souborů je
maximálně 2GB.  Neumožňuje ukládat topologické informace o vzájemných vztazích
mezi prvky geodat.  Každý soubor SHP umožňuje ukládat pouze jeden typ geometrie
(bod, linie, polygon) a neumožňuje uložit stromovou strukturu dat.

.. _geopackage-ref:

Komplexní formát OGC GeoPackage
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Moderním nástupcem výše zmiňovaných rastrových, ale především vektorových
formátů je standard OGC GeoPackage [ref39]_. Tento formát umožňuje uložit libovolná
vektorová data spolu s daty rastrovými, ať už ve formě dlaždic, nebo souborů ve
formátu GeoTIFF do prostředí databáze SQLite. Poskytuje tak jednoduché rozhraní
jazyka SQL pro práci s daty [#geopackage]_. Vektorová data jsou uložena dle specifikace OGC
Simple Features for SQL [ref40]_. Maximální velikost databázového souboru je 140 TB,
což je pro praktické použití většinou dostačující. Data v jedné datové vrstvě,
tedy  databázové tabulce, mohou mít různé typy geometrií. Řada GIS nástrojů již
podporu pro OGC GeoPackage nabízí, včetně Open Source knihovny GDAL od verze
1.11 či proprietárního prostředí Esri ArcGIS od verze 10.2.1.

OGC GeoPackage se zatím v praxi příliš nepoužívá. Nicméně vzhledem k tomu, že se
jedná o standard OGC umožňující  práci s velice komplexními datovými
strukturami, jsme toho názoru, že by se tento formát měl pro otevřená geodata
využívat a to i přesto, že podpora tohoto formátu není v běžných programech mimo
svět GIS příliš rozšířena.


.. index::
    single: Distribuce geodat

============================
Distribuce otevřených geodat
============================

Na způsob distribuce libovolných dat má vliv mnoho faktorů, zejména životní
cyklus poskytovaných dat a typ uživatele, který je bude využívat.

S ohledem na životní cyklus dat je třeba rozlišovat mezi statickými daty a těmi,
které se průběžně mění (dynamická data). Příkladem statických dat jsou výstupy
analýz a data popisující konkrétní stav. Data, která se v čase mění můžeme potom
dále dělit na dva základní okruhy. Do prvního náleží taková data, která popisují
v reálném čase se měnící jev, to může být například znečištění, demografická
data atd. Druhým typem jsou data, která nepopisují proměnlivý jev, ale jsou
průběžně nebo nárazově aktualizována. Takovými daty může být například digitální
model reliéfu.

Typ uživatele je druhým z faktorů, který je vhodné mít na paměti při volbě
způsobu distribuce geodat. S určitou mírou zjednodušení lze konstatovat, že čím
jsou data komplexnější, tím obtížnější je jejich uchopení na straně příjemce.
Základním způsobem distribuce dat pro uživatele by měly být webové služby OGC. V tomto
případě získává uživatel vždy nejaktuálnější data. Náročnějším způsobem 
získávání dat je tzv. vytěžování (harvesting) poskytovaných dat a budování databáze na vlastním hardware. U dat,
která jsou průběžně aktualizována, je v těchto případech nutné umožnit získávání stavových dat (tj. dat platných k určitému datu) a změnových souborů. 

Specifickou oblastí u poskytování otevřených dat je poskytování dat agregovaných (znepřesněných
nebo bez některých atributů). Obvyklým důvodem agregace [#agregace]_ bývají citlivé údaje
(osobní údaje, data vlastněná třetími stranami) obsažené v datech, které se nesmí poskytovat třetím osobám. V tomto případě je nutné geodata od těchto údajů očistit před samotnou distribucí.

Výdejní systém, má-li být efektivní a funkční, musí kopírovat charakter dat, nad
kterými je postaven. Nelze jej vyvíjet nezávisle na datech, 
které má vydávat.

Obsahem kapitoly jsou vhodné způsoby distribuce otevřených geodat, zejména
pomocí webových služeb OGC a publikačního standardu Atom.
Nakonec bude uvedena alternativní možnosti publikace geodat pomocí služby GitHub.

.. index::
    single: INSPIRE
    single: Implementační pravidla INSPIRE
    single: Atom

Implementační pravidla INSPIRE
------------------------------

Jedním z osvědčených způsobů distribuce geodat v Evropské unii je využití
prohlížecích, stahovacích služeb a vyhledávacích služeb podle směrnice INSPIRE,
která se také opírá o standardy konsorcia OGC. O tom, že směrnici INSPIRE, resp.
technické dokumenty s ní svázané, lze považovat za *"best practice"* svědčí i to,
že podobné postupy se prosazují i jinde ve světě, například na Novém Zélandu
[ref46]_. Popis implementace jednotlivých částí směrnice je obsažen v tzv.
implementačních pravidlech. Na publikaci vektorových a rastrových dat se
vztahuje technický průvodce [ref28]_. 

Technický průvodce pro implementaci *Stahovací služby INSPIRE* se dotýká právě
problematiky velkých datových sad. Nabízí dvě možnosti implementace této služby:

* Předgenerované soubory s datovou sadou a jejich distribuce prostřednictvím
  dokumentu ve formátu Atom -- ovšem bez možnosti jejich dotazování či
  výběru části dat prostřednictvím serveru.
* Webové služby OGC WFS a WCS (tak zvané *datové sady s přímým přístupem*). 
  Ty rozšiřují možnosti předgenerovaných datových sad o možnost filtrovat
  požadovaná data již na straně serveru. 

V obou případech je k dispozici tzv. Get Download Service Metadata Request. V
prvním případě seznam odkazů ve formátu Atom (viz kapitola :ref:`atom`), v
druhém případě pomocí WFS nebo WCS GetCapabilities.

Implementační pravidla směrnice INSPIRE definují také požadavky na dostupnost
služeb, jejich kapacitu a rychlost odezvy.  Praxe ukazuje, že požadavky
definované v technických specifikacích INSPIRE jsou velice vágní, nedostatečně
specifikované a v praxi dokonce podhodnocené (např. požadovaná dostupnost služby
99% znamená, že služba může být nedostupná 3.65 dne v roce!).

Otevřené webové služby - OGC OWS
--------------------------------

Základním způsobem distribuce otevřených geodat je využítí otevřených
webových standardů OGC Open Web Services (OWS). Nejpoužívanějšími službami jsou
OGC Web Map Service, Web Feature Service a Web Coverage Service. Existují však i jiné standardy, mající opodstatnění v
některých případech použití. Standardy OGC jsou postaveny nejčastěji na
komunikaci mezi serverem a klientem prostřednictvím zpráv ve formátu XML. Tyto
standardy jsou podporovány ve většině používaných GIS softwarech. OGC služby jsou
použité i v technických normách směrnice INSPIRE.

Při distribuci pomocí webových služeb získává uživatel vždy nejaktuálnější data. Nevýhodou tohoto způsobu je zátěž na
straně infrastruktury poskytovatele, kterou není možné vždy předvídat, konzument
navíc očekává garanci jejich dostupnosti. Zátěž serverů je potřeba průběžně
sledovat a adekvátně na ni reagovat. V tomto směru může být cestou pro
distribuci otevřených geodat využití cloudového řešení na pronajatých sdílených
serverech, kde je výkon dynamicky zvyšován podle potřeby a cena potom odpovídá
využití. K tomu je však potřeba překonat určitou psychologickou bariéru, jelikož
data a infrastruktura zdánlivě nejsou pod kontrolou jako v případě, že poskytovatel použije
vlastní řešení.

V této části jsou zmíněny pouze nejčastěji používané standardy, které pokrývají
většinu případů použití:

* OGC Web Map Service
* OGC Web Map Tiled Service
* OGC Web Feature Service
* OGC Web Coverage Service
* OGC Sensor Observation Service

OGC Web Map Service 
""""""""""""""""""""

Služba OGC WMS [ref20]_ je standard, pomocí kterého může klient požádat o
mapový obraz ve formě rastrového souboru. Server jej na základě klientských
požadavků vytvoří a klientovi odešle. Klient specifikuje obsah obrázku
(zobrazené vrstvy), souřadnicový systém, hraniční souřadnice, velikost, formát
obrázku a další možné detaily. Server odešle pouze rastrový obraz dat, nikoli
vlastní data. To lze s výhodou využít pro případ poskytnutí dat pouze k nahlédnutí z důvodu, že poskytovatel nechce nebo nemůže zpřístupnit zdrojová data. Standardním formátem výstupu je obrázek ve~formátech PNG nebo JPEG podle charakteru dat.

OGC Web Map Tiled Service
"""""""""""""""""""""""""""""

Služba OGC WMTS [ref23]_ je používána v případě, kdy se data v čase příliš nemění (například letecké snímky, obecně podkladové
mapy) a lze pro ně na straně serveru připravit předgenerované dlaždice (tiles - obrázky o
pravidelné velikosti, většinou 256x256 pixelů) do vyrovnávací paměti pro určitá
měřítka a v určitém rozsahu (cache). Tyto dlaždice pak lze zpřístupnit podle
standardu WMTS (nebo i WMS). Výhodou je rychlé odbavení příchozího
požadavku a nižší zátěž IT infrastruktury. Nevýhodou je, že dlaždice musí být
omezeny pro určitá měřítka. Obsah je statický (v čase se nemění, datové vrstvy
vykreslené v obrázku jsou stále stejné). Takto vytvořenou databázi dlaždic je
potřeba udržovat, pravidelně aktualizovat a mít pro ni dostatečně velkou
diskovou kapacitu.  Standardním formátem výstupu je obrázek ve formátech PNG
nebo JPEG podle charakteru dat.

Jako vhodná sada měřítek spolu s výchozím “počátkem” dlaždic se ukazuje řada
dlouhodobě používaná servery ČÚZK, který pro souřadnicový systém S-JTSK
(EPSG:5514, dříve EPSG:2065 či ESRI:102067) vyvinul vlastní řadu měřítek
[ref24]_. Pro globální souřadnicové systémy (jako je např. “Spherical Mercator”
EPSG:3857) se doporučuje používat měřítkovou řadu vyvinutou firmou Google.

OGC Web Feature Service
""""""""""""""""""""""""

Služba OGC WFS [ref21]_ slouží k distribuci vektorových dat. Standard WFS
2.0.0 umožňuje také spouštět některé analytické operace přímo na serveru,
jsou-li na něm podporovány. WFS dále podporuje filtrování požadovaných
prvků geodat (vzhled jevů, *features*), není tak potřeba stahovat celou datovou
sadu. Pro větší objemy dat je možné použít možnost stránkování odpovědi, tj.
nemusí být stahována všechna data najednou v jedné odpovědi. Pomocí WFS může
server vrátit data v libovolném formátu, který podporují knihovny pracující na
pozadí (např. SHP, GeoJSON, …), standardní bývá formát GML.

OGC Web Coverage Service
""""""""""""""""""""""""

Služba OGC WCS [ref22]_ slouží k distribuci rastrových dat. Tento standard
je vhodný zejména tam, kde chceme uživatelům nabídnout ke stažení velká rastrová
data, která mohou být i multispektrální, či mohou obsahovat více rozměrů.
Standardním formátem výstupních dat bývá GeoTIFF.

OGC Sensor Observation Service
"""""""""""""""""""""""""""""""""

Služba OGC SOS[ref72]_ je vhodná pro zpřístupnění měření ze
senzorů a senzorových sítí, stejně jako pro jejich popis. Senzory většinou
publikují několik měření k danému místu a v~daném čase. Poloha senzoru může být
statická, ale může se i v čase měnit. Senzory mohou měřit různé veličiny a
v~různých časových úsecích. Nemění se celý dataset, ale získáváme časovou řadu
měření.

.. index::
    single: Atom
    single: FTP

.. _atom:

Předgenerované soubory a formát Atom
------------------------------------

Pro datové sady větších objemů je vhodné předgenerovat jejich obsah do cílových
vektorových formátů a postavit kolem nich architekturu, která v nich umožní
efektivně vyhledávat. Jedním z vhodných nástrojů je např. formát Atom
[ref25]_. U dat, která jsou průběžně aktualizována, je nutné umožnit jak
získávání stavových dat (tj. dat platných k určitému datu), tak změn formou předgenerovaných změnových souborů. Režim poskytování dat je vhodné nastavit s ohledem na
objem změn. Toto řešení často vede ke snížení zátěže na infrastrukturu
poskytovatele.

Tento způsob se blíží populárnímu a velice jednoduchému přístupu "vystavit
soubory na FTP server". To se s formátem Atom nevylučuje - Atom slouží pouze
jako metadatový dokument, ze kterého lze rychle vyčíst referenci k cílovým
souborům.

Atom
"""""""
Atom je v principu XML dokument, který obsahuje odkazy na dostupné datové sady nebo soubory a jejich základní metadata. Tento formát je využíván i v dalších technologických standardech, jako je
například OGC OWS Context [ref38]_.

Soubor ve formátu Atom je webový standard pro publikování syndikovaného obsahu.
Syndikovaný obsah je takový obsah, který na webu již může být publikován,
souborem Atom se mu ale zpětně přidají vybraná metadata a tím se zjednodušeně
popíše pro automatické zpracování. Atom má nahradit starší (proprietární a
stále populární formát RSS) a je původně určen pro webové stránky. Nicméně jeho
využít pro data se nabízí.

Soubor Atom obsahuje hlavičku, která identifikuje vlastní zdroj a autora
a seznam "záznamů", také s jednoznačnou identifikací a vlastním
obsahem nebo odkazem na tento obsah.

Příklad formátu atom je uveden v :ref:`atom-priloha`.


.. index::
    single: GitHub

.. _github:

Služby GitHub
-------------

Služba GitHub [ref41]_ je webové rozhraní k systému pro správu verzí Git, který
byl původně napsán za účelem správy a údržby zdrojového kódu jádra operačního
systému GNU/Linux. Od roku 2014 je možné do této služby nahrávat i geografická
data v některých z formátů GeoJSON a TopoJSON. GitHub soubory uložené v těchto
formátech umí přímo vizualizovat. Podle různých údajů lze usoudit, že limit pro
velikost vstupního souboru, má-li být zobrazen v mapové prohlížečce, je v
současnosti cca 4.5 MB, záleží ale také na struktuře vstupního souboru
[ref42]_. U jednodušších struktur může být limit až 10 MB (maximální velikost
souboru na serverech GitHub je cca 100 MB). Pokud je datový soubor příliš
veliký, není zobrazen. Jeho praktickou dostupnost to ale nijak neovlivní.

Takto jednoduše publikovaná data lze stáhnout opět v jednom z podporovaných
formátů. Výhoda tohoto přístupu je mimo jiné v tom, že poskytovateli dat zcela
odpadá starost o IT infrastrukturu. O tu se stará třetí strana - v tomto případě
GitHub. Uživatelé navíc  získají efektivní nástroj pro verzování dat v čase.
Pokud by byla služba GitHub v budoucnu uzavřena anebo by se změnila výrazně její
obchodní politika, nejednalo by se o tak zásadní problém. Systém Git je
decentralizovaný, každý uživatel má u sebe lokální kopii celé datové sady včetně
veškeré historie. Vzhledem k tomu, že je systém pro správu verzí Git vyvíjen
jako Open Source, tak by bylo možné případný přechod na jinou formu distribuce
ze služby GitHub realizovat bez větších problémů.

Do prostředí GitHub lze nahrát i dlaždicovaná rastrová data a odkazovat se na ně
formou zápisu identifikátoru URL podle standardu OGC TMS.  Podle zkušeností
uživatelů se jeví tato služba jako dostatečně rychlá. 

Se službou GitHub již experimentují některé menší obce a samosprávy (např.
[ref43]_, [ref44]_), ale i větší města  (např. Chicago [ref57]_).  Tento přístup
k publikování geodat je vhodnější pro menší města bez vlastního IT oddělení.
Nicméně některé koncepty tohoto přístupu (správa verzí, distribuce, náhled,
atd.) jsou aplikovatelné i na tuto případovou studii.

.. _casove_rady:

***************************
Verzování dat a časové řady
***************************

Geografická data nejsou již delší dobu omezena pouze na dvoudimenzionální
prostor (2D). Data jsou často trojdimenzionální (3D a to jak gridová - volumes,
tak vektorová). Mohou být ale i n-dimenzionální (v případě pásem družicových
snímků). V případě časoprostorových dat je dalším rozměrem, který je potřeba
zohlednit, čas. Potom mluvíme o 4D datech.

Na časovou složku v datech se můžeme dívat minimálně ze dvou pohledů: Datová
sada může obsahovat "časovou řadu" nějakého fenoménu (např. vývoj teploty na
daném území, pohyb senzorů v prostoru a~čase, vývoj jejich hodnot) nebo změna
verze celé datové sady (nové přesnější zaměření budov, stav k~určitému datu a
podobně). 

Z hlediska distribuce a formátů dat se k oběma typům přistupuje stejně. Tam, kde
je některá služba nebo formát vhodnější na jeden z typů časové složky je to zdůrazněno.

===============================
Časové řady prohlížecích služeb
===============================

Standard WMS nabízí možnost, jak definovat další dimenze pro poskytovaná
data. Nejčastější formou použití je právě čas, ale může to být např. nadmořská
výška, teplota, atd. či případně i jejich kombinace. V metadatech služby lze
uvést buď přesnou časovou specifikaci výčtem časových okamžiků nebo počáteční
čas a velikost časového kroku mezi jednotlivými datovými vrstvami. Příklady jsou
uvedeny v~ :ref:`wms-cas`.

Standard WMTS navíc umožňuje definovat různé dimenze k předgenerovaným
datovým sadám. Princip je podobný jako u zmíněného standardu WMS, příklady
jsou uvedeny v :ref:`wmts-cas`.

==========================================
Časové řady a verzování stahovacích služeb
==========================================

OGC Web Feature Service
-----------------------

Standard WFS nemá přímou podporu pro časovou dimenzi.
Standard odkazuje na OGC Filter Encoding Specification (FES) [ref49]_, pomocí
kterého lze filtrovat požadovaná data na základně požadavků ze strany klienta.
Pomocí FES lze nastavit počáteční a koncový hraniční čas (startTime a endTime),
mezi kterými klient požaduje stáhnout data. Verzovat lze také pomocí vlastních
klíčových slov (např. číslem revize "1.2.3" nebo datem "2014-01-20" a podobně).

Z uvedeného vyplývá, že WFS slouží jako rozhraní k datové sadě, která obsahuje
data v různých časových intervalech. Na data vztažená k určitému časovému
okamžiku se lze dotazovat právě pomocí filtru dle standardu FES 2.0.

OGC Web Coverage Service
------------------------

OGC WCS podporuje ve své nejnovější verzi specifikace [ref50]_ časový rozsah
požadovaných dat jako jeden z možných rozměrů. Syntaxe pro definici času sleduje
stejně jako u výše zmíněných služeb technickou normu ISO 8601. Příklad je uveden
v :ref:`priloha-d`.

Podle ústního sdělení editora standardu OGC WCS Petra Baumana, se momentálně v
rámci organizace OGC téma času zásadním způsobem mění, neboť se začínají
zohledňovat různé kalendáře (historické, i používané v různých kulturách či
technických společnostech) a další s touto problematikou související komplikace.
Viditelné je to zejména na tom, že ve starších verzích standardů býval definován
parametr TIME explicitně jako vstupní parametr. U nových verzích standardů se
čas mění v jeden z rozměrů dat. Stejně jako stávající rozměry mají své zobrazení
a souřadnicový systém, musí mít i čas společnou referenci.

=================================================================
Verzování a časové řady u souborových formátů a jejich distribuce
=================================================================

OGC GeoPackage
--------------

Formát OGC GeoPackage [ref39]_ je postavený na souborové databázi SQLite (viz
kapitola :ref:`geopackage-ref`), což umožňuje v porovnání se stávajícími souborovými
formáty pokročilejší funkce pro dotazování a manipulaci s daty pomocí jazyka
SQL. Lze využít standardních datových typů TIME a DATETIME jako atributu daného
geoprvku. Další důležitou vlastností je metadatová tabulka ``gpkg_content``,
obsahující mimo jiné informace last_change (datový typ DATETIME) pro jednotlivé
tabulky (datové vrstvy). Dále existuje metadatová tabulka ``gpkg_metadata``,
obsahující vlastnost timestamp, kterou lze využít na označení aktuálnosti
libovolné jednotky v souboru -- buď celé databáze, jednotlivé tabulky či
geoprvku, tj. záznamu v tabulce.

Verzování systémem Git
----------------------

Git je systém na správu verzí, nejčastěji textových souborů, viz kapitola
:ref:`github`. To znamená, že pomocí Gitu lze udržovat přehled o souborech, o tom, kdo
je měnil a jaké změny provedl. Případné konfliktní změny lze řešit poměrně
komfortně, lze se “vracet v čase”, získat stav souboru k určité revizi nebo
časovému okamžiku. Soubor s daty by měl být v Gitu uložen ideálně v textové
podobě (GML, GeoJSON, ...). Binární formáty lze technicky vzato spravovat v
prostředí Git také, potom ale nelze využít specializované verzovací nástroje.

Poskytování změnových souborů (RÚIAN best practice)
---------------------------------------------------

ČÚZK zavedl pro distribuci dat Registru Územní Identifikace, Adres a Nemovitostí
(RÚIAN) systém měsíční aktualizace stavových dat s denními dávkami změnových
souborů. Tento systém plně pokryje jak potřeby uživatele, který potřebuje
jednorázově získat podkladová data, tak uživatele, který potřebuje udržovat
aktuální obraz celé databáze, aniž by byl nucen stahovat velké objemy dat po
síti. Možnost získat seznam přírůstků od libovolného data zvyšuje na straně
uživatele pružnost procesu aktualizace dat.
*Datové sady jsou nabízeny v různě
obsáhlých verzích, v některých případech je dokonce možné volit generalizované
hranice. Data jsou nabízena buď pro celé území České republiky, anebo po
jednotlivých obcích. To umožňuje při poměrně malé zátěži na straně serveru
efektivně obsloužit velké množství klientů. Práce s aktualizací dat se přesouvá
ze strany serveru ke klientům.*

V jedné věci se však RÚIAN nechová ideálně: Jednotlivé stavové a změnové soubory
mají sice pevnou a~strojově předvídatelnou strukturu, chybí jim však centrální
strojově zpracovatelný zdroj. Tím by mohl být například zmiňovaný formát Atom
(viz :ref:`atom`). Podle ústního sdělení bude Atom v nejbližší době doplněn [#cuzk-atom]_.

.. index::
    single: 3D data

*******
3D Data
*******

3D data obsahují kromě svého umístění v prostoru i informaci o "hloubce". To se
týká jak rastrových tak vektorových dat.

================
3D rastrová data
================

Nejtypičtějším příkladem 3D rastrových dat bývá digitální model reliéfu. V tomto
případě se ale nejedná o plnohodnotná 3D data. V rastrové matici je pouze uložena
výška povrchu, ale už ne informace o tom, co se děje "pod ní". Hovoříme tak o 2.5D
datech. 

Samozřejmě je možné uložit i plnohodnotná 3D rastrová data (tzv. volumes), obsahující např.
informaci o půdním profilu, srážkovou mapu a podobně. Většina specializovaných
GIS má pro podobná data vlastní formát. Pro technologicky neutrální distribuci
prostorových dat však můžeme využít např. formát GeoTIFF, a jednotlivé vrstvy
uložit jako "pásma"~rastrového snímku.

=================
3D Vektorová data
=================
Prakticky všechny formáty vektorových dat dnes umožňují uložení souřadnice z k
lomovým bodům. Některé formáty obsahují i speciální 3D vektorové objekty
(ekvivalent polygonu face, či ekvivalent 2D centroidu pro 3D objekt kernel).

Pro distribuci otevřených geografických dat ve 3D by pro většinu aplikací měl
dostačovat běžný formát (GeoPackage, SHP, GeoJSON, GML, ...).

Pro speciální aplikace je vhodné zvážit, zda by bylo možné data distribuovat ve formátu
CityGML (viz :ref:`citygml`). Tento formát umožňuje popsat nejen geometrický
tvar tělesa, ale i vztahy mezi objekty (bloky budov, čtvrtě), vnitřní strukturu
budov a podobně.

.. index::
    single: Metadata
    single: ISO 19115
    single: ISO 19139
    pair OGC CSW, CSW

********
Metadata
********

Veškerá publikovaná geodata a na ně navazující webové služby je potřeba opatřit
příslušnými metadaty.  Metadata jsou strukturovaná data o datech. Metadata
popisují data a služby ve strojově zpracovatelném formátu tak, aby bylo možné v
nich automaticky vyhledávat a to i na základě jejich relevance a aktuálnosti.
Pro metadata existuje množství standardů a doporučení, ale zdaleka ne všechny
jsou vhodné pro oblast geodat.

Vlastní metadata mohou (měly by) mít jak vlastní datové sady (kdo je vytvořil,
kdy, s jakou přesností, co obsahují, z jaké oblasti data
jsou atd.), tak i webové služby tyto datové sady publikující (kdo provozuje
danou službu, jaké datové sady služba publikuje, atd.).
Metadata by měla být dostupná přes rozhraní webové
služby OGC Catalog Service for Web (CSW) [ref37]_. Zároveň doporučujeme tuto službu
otestovat na dostupném software (Esri ArcGIS, QGIS a další) tak, aby byla
ověřena její praktická funkčnost a dostupnost na různých platformách.

V současné době postupně do oblasti GIS a geodat pronikají vznikající standardy pro obecná otevřená data a to se týká i metadat. Otevřená provázaná data (open linked data) mají vlastní
metadatové standardy, které jsou již v souladu s INSPIRE mapovatelné tak, aby
bylo v těchto datových souborech možné vyhledávat pomocí CSW a obráceně,
linkovaná geodata je možné publikovat na portálech s otevřenými daty.

Legislativní pravidla pro metadata
===================================

V současné době je pro pořizování a uchovávání metadat v
geodatové doméně klíčová  mezinárodní technická norma ISO 19115 [ref32]_. Tuto normu
navíc vyžaduje i evropská směrnice INSPIRE ve svém nařízení komise o metadatech
[ref33]_. Vlastní technickou implementací této normy se zabývají implementační
pravidla směrnice INSPIRE pro metadata [ref34]_. Vlastní fyzické uložení metadat
geografické datové sady nebo služby je definováno navazující technickou normou
ISO 19139 (XML) [ref35]_. Obecně lze říci, že je vhodné držet se metadatového
profilu České republiky [ref36]_, i když to v první fázi za vysloveně nutné
nepovažujeme.


.. index::
    single: Souřadnicové systémy
    single: S-JTSK
    single: UTM
    single: WGS84
    single: S-42
    single: EPSG

********************
Souřadnicové systémy
********************

Systém souřadnic je soustava základních údajů (referenčních bodů, přímek nebo
křivek), umožňující určovat souřadnice polohy objektu ve zvolené vztažné
soustavě. Protože převod tvaru Země na plochu papíru (dnes monitoru počítače) je
vždy provázen určitou nepřesností, existuje množství systémů, které v~daném místě
na Zemi poskytují známé a popsatelné zkreslení-nepřesnost (nebo
globální systémy, používané pro zobrazení celé Země).

.. note:: Protože existuje množství způsobů, jak popsat konkrétní systém a
    velké množství souřadnicových systémů, bývá v oboru zvykem, že se pro souřadnicové systémy používá databáze 
    EPSG (European Petroleum Survey Group). 
    Tu lze stáhnout ze stránek http://www.epsg-registry.org/ nebo využívat
    některou ze služeb nad touto databází postavenou, např. http://epsg.io.

Geografické datové sady jsou v České republice vedeny především v souřadnicovém
systému S-JTSK (EPSG 5514 [#5514]_). Pro vojenské mapové podklady se v minulosti používal
souřadnicový systém S-42 (EPSG 3835 [#3835]_). Vzhledem k zániku Varšavské smlouvy a
pozdějšímu přistoupení k NATO se začal místo souřadnicového systému S-42
používat systém UTM/WGS-84 (zóny 33 - EPSG 32633 [#32633]_ a 34 - EPSG 32634 [#32634]_). Evropská
směrnice INSPIRE [ref26]_ zejména pak ve specifikaci věnované souřadnicovým systémům
([ref29]_, str. VII) a pro měřítka větší než 1:500 000 mezi podporované systémy
přidává ETRS89-TM (EPSG 3035 [#3035]_). Praxe si vynutila použití souřadnicového systému
Spherical Mercator (EPSG 3857 [#3857]_), zavedeného firmou Google pro jejich mapové
produkty.

.. note:: Dříve používané zápisy S-JTSK, jako EPSG 2065 či ESRI/ESPG 102067, 
    vznikly díky tomu, že v databázi EPSG nebyl přítomný kód pro S-JTSK
    s "otočenými osami"~(a zápornými hodnotami souřadnic), tzv. "S-JTSK/Krovak
    East North". To dnes již není potřeba a všechny systémy by měly nadále
    používat EPSG 5514.

==========================================
Obecná doporučení souřadnicových systémů
==========================================

Pro stahovací služby se přikláníme k publikování datových sad v jejich původních
souřadnicových systémech, což je v praxi většinou S-JTSK. Navíc všechny
relevantní desktopové GIS programy jsou schopny transformovat geodata do
uživatelem požadovaných cílových souřadnicových systémů online. Pokud se přeci
jen ukáže, že je potřeba poskytnout některým klientům možnost stahovat data v
jiném souřadnicovém systému, doporučujeme zprovoznit transformační souřadnicovou
službu podle specifikace INSPIRE [ref30]_.

V každém případě je potřebné zajistit, aby distribuovaná data měla korektně
nastaveny definice souřadnicových systémů. V případě S-JTSK je nutné, aby
informace o souřadnicovém systému obsahovala parametry pro transformaci mezi
referenčním Besselovým elipsoidem a elipsoidem WGS-84, transformační
parametry anebo grid. Jinak může dojít k nepřesnosti při transformaci až v řádu
několika desítek metrů. Více informací k tomuto tématu lze najít například na
Portálu FreeGIS [ref31]_.

Vedle S-JTSK doporučujeme nabízet data v souřadnicovém systému WGS84 (EPSG
4326 [#4326]_). Zejména zahraniční uživatelé či uživatelé kombinující data z různých
datových zdrojů tento souřadnicový systém využijí. Kromě toho se používá v
navigacích a GPS zařízeních.

U prohlížecích služeb je vhodné umožnit zobrazení dat v souřadnicovém systému
Spherical Mercator, využívaný např. firmou Google ve svých mapových produktech,
projektem OpenStreetMap a nebo mapami Bing. To uživatelům umožní využívat tyto
zobrazovací služby v kombinaci s jinými podklady. Tento systém nesl kdysi
neoficiální označení 900913, nyní je již zastaralý a v EPSG je označen kódem
3857.

Obecně lze říci, že na běžných platformách webových serverů je přidání dalšího
souřadnicového systému otázku minimálního zásahu do konfigurace, takže lze
podporu pro další systémy přidávat i na požádání.

=================================================
Pořadí souřadnic v WMS 1.3.0, WFS 2.0.0 a GML 3.x
=================================================

Ve starších verzích standardů OGC se předpokládalo, že pořadí souřadnic v
požadavku (např. parametru BBOX u WMS) nebo při odpovědi (např. GML publikované
serverem WFS) je vždy ve formátu X,Y.

V nových verzích standardů (WMS 1.3.0, WFS 2.0.0, atd.) je explicitně
zdůrazněno, že záleží na předpisu daného souřadnicového systému -- pořadí os tedy
může být X,Y ale i Y,X. To platí zejména pro souřadnicové systémy WGS-84 (EPSG
4326) a ETRS-89 (EPSG 3035). U S-JTSK (EPSG 5514) se tento fakt v praxi
nezohledňuje.

Zdaleka ne všechny serverové ale i klientské implementace standardů jsou schopny
pořadí souřadnic korektně zohlednit [ref54]_, což je dobré mít na paměti.

********************
Závěrečná doporučení
********************

======================
Licence otevřených dat
======================

Pro účely vymezené v začátku tohoto oddílu se jeví jako vhodná licence Creative
Commons BY-SA 4.0 [ref47]_, případně Open Data Commons Attribution License (ODC-BY)
[ref48]_. Výhodou první je její obecná známost (i napříč veřejnou správou), druhá je
lépe přizpůsobena pro využití v oblasti geodat.

Třetí možností je vytvořit licenci na míru danému projektu, a to případně i
odvozením ze dvou zmíněných výše. V takovém případě je ale nezbytná spolupráce s
expertem na autorské právo.

==================================
Volba formátů a způsobů distribuce
==================================

Formát souborů
--------------

Nelze jednoduše doporučit jeden či dva formáty vhodné pro všechny uživatele a
datové sady. Vždy je potřeba zvážit charakter dat a převládající způsob jejich
použití. 

Pro předgenerované soubory vektorových dat doporučujeme, v dlouhodobém horizontu,
formát OGC GeoPackage. V krátkodobém horizontu lze použít i formát SHP nebo GML, z toho důvodu, že formát GeoPackage není zatím příliš rozšířen.

Pro publikování formou prohlížecích webových služeb (OGC WMS, WMTS) je vhodné
volit  v závislosti na charakteru dat formáty PNG a JPEG.

V případě stahovacích služeb doporučujeme pro vektorová data formát
GML a pro rastrová data potom podle jejich
charakteru GeoTIFF či JPEG.

Distribuce otevřených geodat
----------------------------

Jako primární doporučujeme využít standardy OGC OWS, zejména WMS, WFS a WCS.

Kde to z důvodu velikosti datových sad nebo pro technická omezení na straně
poskytovatele není možné, doporučujeme předgenerovat datové soubory ve vhodném
datovém formátu a poskytnout soubor ve formátu Atom s odkazy na takto vytvořené
soubory. Podobně jako se k tomu kloní implementační pravidla INSPIRE.

Pro datové sady, které se *mění v čase* a jsou příliš velké na to, aby se s každou
změnou vydávala aktualizovaná verze celé sady, je vhodné publikovat jednou v
pravidelných intervalech stavová data a současně k nim poskytovat v kratších
časových intervalech změnové soubory. Toto řešení může výrazně snížit zatížení
IT infrastruktury, neboť uživatelé nemusí vždy stahovat celou datovou sadu ve
formě stavových dat, ale pouze menší změnové soubory, které si sami aplikují na
kopii datové sady tak, aby ji měli co možná nejaktuálnější. Více k tomuto tématu
v kapitole :ref:`atom`. Více o~časových řadách v části :ref:`casove_rady`.

====================
Souřadnicové systémy
====================

Prohlížecí a stahovací služby
-----------------------------

OGC WMTS
^^^^^^^^

Pro prohlížecí službu OGC WMTS je výhodné nabízet předgenerované dlaždice
minimálně pro souřadnicové systémy EPSG 3857 (Spherical Mercator) a to ve
schématu, ve kterém je nabízí např. mapy firmy Google, ale i projekt
OpenStreetMap [ref52]_ (nebo služby ČÚZK) a pro souřadnicový systém S-JTSK
(EPSG 5514) ve schématu používaném servery ČÚZK [ref53]_.

OGC WMS, WFS a WCS
^^^^^^^^^^^^^^^^^^

Transformace mezi souřadnicovými systémy bývá u současných software poměrně
rychlá. Služby by měly nabízet data především v původním
souřadnicovém systému - převážně S-JTSK (EPSG 5514). Vzhledem k určité
exotičnosti tohoto systému je vhodné navíc podporovat minimálně ETRS-89 (EPSG
3035) a WGS 84 (EPSG 4326). Spherical Mercator (EPSG 3857) není v tomto případě
nezbytný, většina webových aplikací transformuje vektorová data z WGS84
automaticky, stejně tak většina desktopových nástrojů.

Předgenerované vektorové a rastrové soubory
-------------------------------------------

Vzhledem k plánovaným větším objemům dat doporučujeme publikovat datové soubory
v původním souřadnicovém systému (S-JTSK, EPSG 5514) a případně WGS 84 (EPSG
4326). Implementační pravidla směrnice INSPIRE doporučují poskytnout
transformační službu, která umožní na straně serveru transformovat data přímo do
cílového systému.

.. only:: html

   .. rubric:: Poznámky pod čarou

.. [#shp] Shoda napříč programy panuje alespoň na souboru s příponou .prj, který
    obsahuje informace o souřadnicovém systému.

.. [#agregace] *Agregace* je seskupení vybrané části určitých entit za účelem
    vytvoření nové entity -- seskupení datových prvků do větších skupin.  Tím
    dochází k odstranění některých detailů z dat. Agregace se může použít např.
    pro znepřesnění nebo anonymizaci citlivých dat.

.. [#cuzk-atom] Ústní sdělení, konference "Inspirujme se ...", 2014

.. [#geopackage] Formát OGC GeoPackage byl navržen primárně jako
                 výměnný formát. Nejedná se o alternativu ke geodatabázím
                 jako je např. SpatiaLite, které nabízejí podporu pro
                 pokročilé prostorové SQL dotazy *(spatial SQL queries)*.

.. [#5514] http://epsg.io/5514
.. [#32633] http://epsg.io/32633
.. [#32634] http://epsg.io/32634
.. [#4326] http://epsg.io/4326
.. [#3857] http://epsg.io/3857
.. [#3035] http://epsg.io/3035
.. [#3835] http://epsg.io/3835


