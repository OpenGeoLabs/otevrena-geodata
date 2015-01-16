.. index::
    single: WMTS
    single: Časové řady
    single: Verzování

.. _wmts-cas:

Příloha C: OGC WMTS -- dimenze a~časové řady
============================================

Příklad OGC WTMS Capabilities response s časovou řadou
------------------------------------------------------

.. code-block:: xml

    ...
    <Layer>
    <Name>time</Name>
    <Title>Časová vrstva - Příklad</Title>
    ...
    <Dimension>
       <ows:Identifier>time</ows:Identifier>
       <UOM>ISO8601</UOM> 
       <Default>2013-05-29</Default>
       <Current>true</Current>
       <Value>2012-05-08/2013-05-29/P1D</Value>
    </Dimension>
    ...
    </Layer>
    ...

WMTS požadavek s parametrem TIME
--------------------------------

Kódování Key-Value-Pairs (KVP)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

::

    ...&TIME=1996-01-02&...

Kódování REST
~~~~~~~~~~~~~

**Šablona**

::

  http://foo/wmts/{Product}/{Style}/{Time}/{TileMatrixSet}/{TileMatrix}/
  {TileRow}/{TileCol}.jpg 

.. raw:: latex

   \newpage

**Konkrétní příklad**

http://foo/wmts/ortofoto/default/2012-07-09/EPSG5514/6/13/36.jpg
