.. _NIF_ HardwareDev:

===========================
NIF Hardware Development
===========================

Conducting novel scientific research often requires the development of custom tools to address very specific needs for which there may be no suitable commercially available solutions. Fortunately, researchers at NIH have access to excellent resources to assist in the design, development and manufacture of custom research hardware, in the form of their institute's own machine shop. Beyond that, there are plenty of external companies capable of providing custom machining, 3D printing and electronic circuit board manufacture services, as well as open-source design software and tutorials freely available online. This page outlines some recommendations for custom hardware development. 


Computer Aided Design (CAD) resources
=========================================

The commercial software AutoDesk SolidWorks is the industry standard for CAD and is used by the NIMH Section on Instrumentation. However, with proprietary file formats and licenses starting at over $3K, it is anathema to open-science. Fortunately there are many open-source, cross-plaform CAD software options available.

.. csv-table::
  :file: ../_static/CSVs/NIF_HardwareOpenCAD.csv
  :header-rows: 1
  :widths: auto
  :align: left


3D-printing Prototypes
==========================================

The `SCNI <https://www.nimh.nih.gov/research/research-conducted-at-nimh/research-areas/clinics-and-labs/ln/scni/index.shtml>`_ has two `FormLabs <https://formlabs.com/>`_ SDL printers, located in the B1-A19 lab space (a Form2 and Form3) as well as an isopropyl alcohol bath and UV-curing oven for finishing prints. Additional 3D printers are available  when submitting print jobs to the :ref:`NIMH Section on Instrumentation <NIMH_SI>`, as listed in the table below:


.. |FormLabs| image:: ../_images/Logos/FormLabs.png
  :width: 100
  :target: https://formlabs.com/

.. |MarkForged| image:: ../_images/Logos/Markforged.png
  :width: 100
  :target: https://markforged.com/

.. |Stratasys| image:: ../_images/Logos/Stratasys.png
  :width: 100
  :target: https://www.stratasys.com/

.. |3Dsystems| image:: ../_images/Logos/3Dsystems.png
  :width: 100
  :target: https://www.3dsystems.com/

.. csv-table::
  :file: ../_static/CSVs/NIF_Hardware3Dprinting.csv
  :header-rows: 1
  :widths: auto
  :align: left

For specialist 3D-print jobs requiring speed, materials, dimensions or techniques not available using the 3D printers on campus, we recommend commercial options :ref:`below <External3Dprinting>`.


LN 'Quick Response' machine Shop
==========================================

The `Laboratory of Neuropsychology (LN) <https://www.nimh.nih.gov/research/research-conducted-at-nimh/research-areas/clinics-and-labs/ln/index.shtml>`_ has a communally shared 'quick response' machine shop located in :ref:`B1B55 <Facility-Floor-Plans>` of Building 49. Access to the room requires permission from your PI and meeting with LN Staff Scientist `Andy Mitz <https://www.nimh.nih.gov/research/research-conducted-at-nimh/research-areas/clinics-and-labs/ln/oc/people.shtml>`_ (B1C72) for basic safety training. Keys to the room are available to approved users from Andy Mitz and :ref:`Aidan Murphy <apm>`. The main tools available are listed in the table below, along with links to user manuals.

.. note:: Room B1B55 is only large enough for one person to use at a time. Please be courteous to other users of the shop by tidying up after use.


.. |Jet| image:: ../_images/Logos/Jet.png
  :height: 30
  :class: no-scaled-link

.. |Smithy| image:: ../_images/Logos/Smithy.png
  :height: 30
  :class: no-scaled-link

.. |Milwaukee| image:: ../_images/Logos/Milwaukee.png
  :height: 40
  :class: no-scaled-link

.. |Craftsman| image:: ../_images/Logos/Craftsman.png
  :height: 30
  :class: no-scaled-link

.. |DrillPress| image:: ../_images/Photos/B1B55/B1B55_DrillPress.jpg
  :height: 100

.. |BandSaw| image:: ../_images/Photos/B1B55/B1B55_BandSaw.jpg
  :height: 100

.. |Lathe| image:: ../_images/Photos/B1B55/B1B55_Lathe.jpg
  :height: 100

.. |TableSaw| image:: ../_images/Photos/B1B55/B1B55_Bench.jpg
  :height: 100

.. csv-table::
  :file: ../_static/CSVs/LN_QuickResponseShop.csv
  :header-rows: 1
  :align: left
  :widths: auto
 



.. _NIMH_SI:

NIMH Section on Instrumentation
==========================================

The NIMH `Section on Instrumentation <https://www.nimh.nih.gov/research/research-conducted-at-nimh/research-areas/research-support-services/section-on-instrumentation/index.shtml>`_ provide a range of machine shop services, including design and fabrication of custom equipment for addressing specific research needs. The SI machine shop is located in Building 13.


.. _External3Dprinting:

External Manufacturers
==========================

Sometimes NIH's in-house manufacturing resources cannot meet the demands of a project - either due to delay in turnaround or lack of access to specific materials or fabrication methods. Fortunately there are many external commercial manufacturing options available. Some companies that we have previously worked with for these purposes are listed in the sections below.

3D printing
-----------------




Waterjet and laser cutting
-----------------------------

The NIMH Section on Instrumentation's water jet machine is a fantastic resource and is the best option for most water jet jobs. However it does have size limits (24" is the maximum dimension it can cut) and turnaround times are often unspecified, so if you need a large part cut or would like a guaranteed delivery date then these external companies are worth considering:

.. |BigBlueSaw| image:: ../_images/Logos/BigBlueSaw.jpeg
  :width: 150
  :target: https://www.bigbluesaw.com/

.. |Xometry| image:: ../_images/Logos/Xometry.svg
  :width: 150
  :target: https://www.xometry.com/capabilities/waterjet-cutting/

.. |eMachineShop| image:: ../_images/Logos/eMachineShop.png
  :width: 150
  :target: https://www.emachineshop.com/waterjet/

.. csv-table::
  :file: ../_static/CSVs/NIF_HardwareWaterjet.csv
  :header-rows: 1
  :widths: auto
  :align: left


Aluminum T-slot Profile
---------------------------

For rapid DIY construction of structural framing, there are a number of commercial sources for extruded aluminum T-slot profile that offer various customizations (cutting to length, drilling and tapping holes, etc.) as well as compatible hardware. Some vendors we have previous used are listed below:


.. |8020| image:: ../_images/Logos/8020.svg
  :width: 150
  :target: https://8020.net/shop

.. |McMaster| image:: ../_images/Logos/McMasterCarr.svg
  :width: 150
  :target: https://www.mcmaster.com/t-slots/

.. |Misumi| image:: ../_images/Logos/Misumi.png
  :width: 150
  :target: https://us.misumi-ec.com/

.. |Bosch| image:: ../_images/Logos/Rexroth.svg
  :width: 150
  :target: https://www.boschrexroth.com/en/us/products/product-groups/assembly-technology/topics/aluminum-structural-framing/index


.. csv-table::
  :file: ../_static/CSVs/NIF_HardwareTslot.csv
  :header-rows: 2
  :widths: auto
  :align: left

