=============================
PrimaThrone
=============================

.. image:: _images/Designs/PrimaThrone/PrimaThrone_V1_Demo.jpeg
  :width: 30%
  :align: left

PrimaThrone is an open-source testing chair design for use in neurobehavioural research with non-human primates (and more specifically, macaque monkeys). 

Motivation
==========

.. image:: https://www.nc3rs.org.uk/sites/default/files/Images/Animals/Restraint%20Monkey.jpg
  :width: 30%
  :align: right
  :target: https://www.nc3rs.org.uk/chair-restraint-training-non-human-primates


Neuroscientific research in non-human primates (NHPs) requires a range of esoteric products, that manufacturers are able to charge exorbitant prices for. The NHP testing 'chair' is one such item. 

Typical NHP chair designs (`McMillan, Bloomsmith & Prescott, 2017 <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5621573/>`_) consist of two main parts: a box structure that the animal can climb into and sit in with only the head exposed, and a base structure that is used to elevate the box and is typically on lockable casters for transportation. The main constraints on the materials and construction of NHP chairs is that they need to be able to safely and comfortably contain an adult NHP, while also withstanding the high temperature and pressure of regular cage wash. However, they also need to be light enough to move around fairly easily and designed with ease of use and the safety of researchers in mind. NHP chairs for use in MRI scanners places additional constraints on material choices and dimensions, which this design is not intended for.


Commercial options
==================

If your lab has the money, it's always nice to buy ready-made solutions
so that you can focus on science instead of engineering. The table below lists some
commercial options for typical NHP behavioural testing chairs.

.. csv-table:: 
  :file: _static/CSVs/MLab_NHPchair_Commercial.csv
  :widths: 30 20 20 20
  :header-rows: 1
  :align: left
 

Materials
=========

Polycarbonate
-------------

Polycarbonate (e.g. 'Lexan') is a popular choice of panel material for
constructing the box section of NHP chairs, since it is available in a
clear format that allows researchers visual access to the animal once
seated in the chair. Polycarbonate panels are inexpensive and can be cut
to custom shapes using a water-jet cutter (although they cannot be laser
cut). The downside of polycarbonate is that it becomes brittle through
repeated exposures to high-temperature cage wash systems, which combined
with the mechanical forces applied to it will eventually result in
cracks, especially around screw holes. The use of nylon or other
non-metal screws and hardware, and larger through-holes (rather than
tapped holes) can ameliorate this problem.


Aluminium
---------

A more durable alternative to polycarbonate is aluminium, with the
obvious trade-off that you won't be able to see through it. Using a
marine-grade aluminium alloy like
`5052 <https://en.wikipedia.org/wiki/5052_aluminium_alloy>`__ for the
side panels of the chair box will improve the chair's structural
stability and chemical resistance, while vent holes cut in these panels
can give some visibility and improve air flow.


T-slot aluminium profile
------------------------

Extruded aluminium 't-slot' profile is a simple and cost effective means
of constructing the chair base. Many companies offering NHP chairs
commercially will use t-slot, although this construction method is less
durable than a welded frame, and may require re-tightening over time. A
benefit of t-slot profile is that it is easy to attach additional
components to the chair, such as guides to help position the chair in a
stable and reproducible manner in the testing rig.


Hardware
--------

In addition to the t-slot hardware and locking casters needed for the
base, a hinge and latches are needed for the rear door, handles for
moving the chair around, corner brackets for attaching the panels to
each other, and a removable waste pan.


Bill of materials
-----------------

.. csv-table::
  :file: _static/CSVs/MLab_PrimaThrone_BOM.csv
  :header-rows: 1
  :widths: auto
  :align: left