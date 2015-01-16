.. index::
    single: WMS
    single: Časové řady

.. _wms-cas:

Příloha B: OGC WMS -- dimenze a~časové řady
===========================================

Příklad OGC WMS Capabilities response s časovou řadou
-----------------------------------------------------

.. code-block:: xml

    ...
    <Layer>
    <Name>time</Name>
    <Title>Časová vrstva - Příklad</Title>
    ...
    <Dimension name="time" units="ISO8601" default="2003-10-17">
    1996-01-01/2003-10-17/P1D
    </Dimension>
    ...
    </Layer>
    ...

Různý způsob vyjádření obsahu elementu Dimension
------------------------------------------------

+-------------------------------------+-------------------------------------------------------------+
| Syntaxe                             | Význam                                                      |
+=====================================+=============================================================+
| hodnota                             | Samostatná jedna hodnota                                    |
+-------------------------------------+-------------------------------------------------------------+
| hodnota1,hodnota2,hodnota3,...      | Seznam více hodnot                                          |
+-------------------------------------+-------------------------------------------------------------+
| min/max/krok                        | Interval definovaný minimální a maximální hodnotou a krokem |
+-------------------------------------+-------------------------------------------------------------+
| min1/max1/krok1,min2/max2/krok2,... | Více různých intervalů                                      |
+-------------------------------------+-------------------------------------------------------------+

WMS GetMap požadavek s parametrem TIME
--------------------------------------

::

    ...&TIME=1996-01-02&...
