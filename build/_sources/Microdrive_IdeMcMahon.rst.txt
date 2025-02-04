============================================
Microwire Brush Array (MBA) Electrodes
============================================

.. contents:: :local:

.. _mba:

MBA Electrodes
==========================

.. figure:: ../_images/Guides/BrushArrayElectrodes/MicroProbes_MBA.png
  :align: right
  :width: 100%
  :figwidth: 50%

  **Figure 1.** Chronic `microwire brush array <https://microprobes.com/images/products/mc/mba/>`_ manufactured by MicroProbes, MD. 

.. figure:: ../_images/Guides/BrushArrayElectrodes/MBA_Implanted.png
  :align: right
  :width: 100%
  :figwidth: 50%

  **Figure 2.** Coronal MR image and micro-CT showing an implanted chronic microwire multielectrode and an illustration of the 'brush' tip (MR image courtesy of McMahon et al., 2014).

The microwire 'brush' array (MBA) electrodes that are now commonly used in the SCNI were initially developed in collaboration with `Igor Bondar <https://www.ihna.ru/en/employees/igor.bondar/>`_ and first reported by `Bondar et al., (2009) <http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0008222>`_. The concept is to take a bundle of insulated microwires and insert them into the brain through a guide tube. As the electrode tip is lowered, the individual wires splay out in the tissue, allowing for stable isolation of extracellular spiking activity for a local population of neurons over long time periods. Each microwire consists of a nickel-chromium-aluminum core of 12.5 µm diameter, insulated with polyimide by the manufacturer (‘IsaOhm’, Isabellenhuete, Germany). These electrodes are currently commercially available from `MicroProbes (MD) <https://microprobes.com/products/multichannel-arrays/mba>`_ in lengths from 2.5 mm to 120 mm. Similar electrodes have been developed independently by other groups (e.g. `Krüger et al., 2010 <https://doi.org/10.3389/fneng.2010.00006>`_).

.. _MBA_TipDev_

Microwire brush tip development notes
-----------------------------------------

.. figure:: ../_images/Guides/BrushArrayElectrodes/BrushTipTests.png
  :width: 100%
  :figwidth: 50%
  :align: right
  :alt: MBA brush tip designs

  **Figure 3.** Simulations of microwire brush tip trajectories in tissue. Columns show different brush tip preparations. Top row shows the state of the array tip prior to insertion in the guide tube. The second and third rows show the gradual deflection of individual microwires with distance emerged from the guide tube tip. (Figure courtesy of :ref:`Dr. Kenji Koyano <kwk>`). 

In order to improve the cell yield per implant, we attempted moving from 64-channel bundles to 128-channel bundles several years ago. However, our experience was that 128-channel bundles do not produce comparable yield to 64-channel bundles, possibly due to the mechanical properties of the increased bundle size. We subsequently reverted to using 64-channel bundles, but also miniaturized the microdrive design in order to obtain between 128-256 channels per implant using multiple 64-channel bundles.

During our tests to discern why the 128-channel bundles might not be working as well as we had hoped, Dr Kenji Koyano performed a series of tests, producing microwire bundles with a variety of tip designs, and inserting them into gelatin as a simulated brain tissue medium. His observations of how the individual microwires deflect upon entering the gelatin are shown here (Figure 3). The results suggest that a non-flat tip shape and active pre-splaying of the wires prior to insertion in the guide tube both improve splaying of the wires in tissue. 


Microprobes MBA Order Specifications
-----------------------------------------

.. figure:: ../_images/Guides/BrushArrayElectrodes/MBA_Specifications.png
  :align: right
  :width: 100%
  :figwidth: 40%

When ordering MBAs from `MicroProbes for Life Sciences <https://microprobes.com/images/products/mc/mba/>`_, you will need to provide certain specifications. The figure to the right illustrates typical specifications for SCNI MBA orders. Important factors to consider include:

-  **Connectors**. Nickel-free `Omnetics 32-channel, 36-pin nano-connectors <https://www.omnetics.com/products/neuro-connectors/nano-strip-connectors>`_ are preferred for connecting with existing SCNI and NIF eletrophysiolpogy headstages, MRI-compatibility and for minimizing footprint on the implant. If the connectors will be housed in a 3D-printed casing (see information on :ref:`chronic microdrives <chronicMicrodrives>` below) then it is important to specify to MicroProbes that the epoxy reinforcing the wires at the connector should not protrude beyond the extent of the connector block itself.

- **Lengths**: Total electrode shaft length should be determined by target distance and planned implant trajectory. For electrodes implanted vertically in stereotaxic coordinates and targeting ventral visual stream areas, the SCNI typically have used the following lengths: 50 - 60mm: middle and anterior fundus of STS; 65 - 75mm: ventral surface of IT, AMTS, perirhinal cortex, amygdala. Additional typical lengths specified include:

  - Tip length: 5mm
  - Flexible cable length: 40mm
  - Flexible cable per connector: 10mm
  - Sliver ground wires (1 per connector): 100mm

- **Materials**: MicroProbes offer two material choices of microwire: Nickel-Chromium (NiCr20AISi) and Platinum-Iridium (PlIr). The SCNI has always used Nickel-Chromium (`IsaOhm(R), Isabellenhuette, Germany <https://www.isabellenhuette.de/fileadmin/Daten/Praezisionslegierungen/Datenblaetter_Widerstand/Englisch/ISAOHM.pdf>`_). 

.. _chronicMicrodrives: 

Chronic Implanted Microdrives for MBAs
=========================================

.. panels::
  :column: col-lg-12 p-0 border-1
  :header: bd-primary text-bold p-1 pl-2
  :body: bg-light border-0 p-2

  :opticon:`info,mr-1` **Note**
  ^^^^^^^^^^^^^^^^^^^^^^^^
  The Ide-McMahon microdrive design was the SCNI's first generation of chronically implanted micro drive hardware for use with MBAs. However, development of implant designs and procedures is ongoing. Information on the Ide-McMahon design is provided here for reference, but the system now used for MBA implants in the SCNI is the :ref:`MIDAS system <Microdrive_MIDAS>`, which offers numerous improvements.


Ide-McMahon Microdrive
-------------------------------

.. image:: ../_images/Guides/BrushArrayElectrodes/IdeMcMahonMicrodrive.jpg
  :width: 50%
  :align: right
  :alt: Ide-McMahon microdrive design

This original design for a chronically implantable microdrive was conceived at NIH by David Ide (`Section on Instrumentation <https://www.nimh.nih.gov/research/research-conducted-at-nimh/research-areas/research-support-services/section-on-instrumentation/index.shtml>`__) and David McMahon (:ref:`former SCNI postdoc <SCNI_Alum>`), and was published in `McMahon et al., 2014 <https://www.physiology.org/doi/10.1152/jn.00052.2014>`__. The original drive design consists of three Ultem disks, stacked on three ceramic rods, with a single central PEEK drive screw. Turning the drive screw (accessible from the top of the drive) advances or retracts the central drive disk, to which the electrode shaft is clamped. The drive mounts to a cylindrical (19mm diameter) Ultem chamber base via two nylon screws, and is protected by an Ultem cap, which attaches via four brass set screws. 

The microdrive is intended for use with a single :ref:`microwire brush array <mba>`, as described by McMahon et al (2014) and currently sold by `MicroProbes <https://microprobes.com/products/multichannel-arrays/mba>`__. The system is is entirely MR-compatible, provided that nickel-free Omnetics connectors are used in electrode construction.

.. figure:: ../_images/Guides/BrushArrayElectrodes/McMahon_2014.jpeg
  :align: right
  :width: 100%
  :figwidth: 50%

  **Figure 1**. Photograph and illustration of the original microdrive design (with permission from `McMahon et al. (2014) <https://www.physiology.org/doi/10.1152/jn.00052.2014>`__).

The original design was CNC machined from Ultem rods by the Section on Instrumentation at NIH. Since the design was published, it is now also manufactured by `Hybex Innovations <http://hybex.com/portfolio/chronic-microdrive/>`__ (Brian Hines) and `Rogue Research <https://www.rogue-research.com/veterinary/tools-implants/>`_ with minor modifications, and retails for $742.00 each. As a lower cost alternative, we also provide .stl files for 3D-printing this microdrive `here <https://www.thingiverse.com/thing:3501708>`__, and a list of additional parts needed for assembly is provided below. However, researchers interested in 3D-printed microdrives are advised to check out our newer designs that are more compact, require less user finishing and assembly, and offer several other improvements.
   

.. link-button:: https://www.thingiverse.com/thing:3501708
    :type: url
    :text: Download CAD files
    :classes: btn-success

.. csv-table:: 
  :file: ../_static/CSVs/SCNI_IdeMcMahon_MicrodriveBOM.csv
  :widths: 20 20 40 10 10
  :header-rows: 1
  :align: left


Surgical Implantation Procedure
=====================================

The panel below provides an illustrated step-by-step overview for the typical surgical procedure of implanting the Ide-McMahon microdrive system with a single pre-loaded MBA electrode. 

.. panels:: 
  :column: col-lg-12 p-0
  :body: bg-dark text-justify text-light

    .. tab:: 1. Mark locations

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide1.png
        :align: right
        :width: 100%

      - Clean the skull surface
      - Position chamber using stereotax
      - Check clearance from headpost (with attachment)
      - Mark chamber location
      - Mark screw locations

    .. tab:: 2. Drill skull

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide2.png
        :align: right
        :width: 100%

      - Drill and tap screw holes
      - Insert ceramic screws
      - Mark craniotomy location by lowering guide tube and stylet in stereotax
      - Drill craniotomy

    .. tab:: 3. Insert guide tube

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide4.png
        :align: right
        :width: 100%

      - Lower guide tube and stylet on stereotaxic arm
      - Stop at appropriate target depth
      - Fill in the craniotomy around the guide tube with bone wax
      - Coat the bone surface with Copalite varnish to seal it

    .. tab:: 4. Place chamber

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide5.png
        :align: right
        :width: 100%

      - Slide the chamber down over the guide tube
      - Position the chamber base against the skull surface
      - Apply a thin layer of dental acrylic between the skull and the chamber

    .. tab:: 5. Build acrylic cap

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide6.png
        :align: right
        :width: 100%

      - Build up the dental acrylic around the chamber to cover the screws
      - Ensure that acrylic does not impede attachment of the cap
      - Make the contour of the acrylic as smooth as possible

    .. tab:: 6. Remove the stylet

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide7.png
        :align: right
        :width: 100%

      - Fix the guide tube in place with a small drop of glue
      - Once glue is dry, slowly remove the stylet
      - Cut the top of the guide tube diagonally, just below the top of the chamber

    .. tab:: 7. Insert the electrode

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide8.png
        :align: right
        :width: 100%

      - Mount the electrode (loaded into the microdive) onto the stereotaxic arm
      - Lower the electrode until the tip approaches the guide tube
      - Tie a loose loop of vicryl suture around the tip of the brush, to reduce the splay
      - See :ref:`detailed description of electrode insertion procedure <MBA_insertion>` below.


    .. tab:: 8. Lower the drive

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide9.png
        :align: right
        :width: 100% 

      - Carefully lower the brush tip just below the top of the guide tube
      - Move the electrode in the M-L or A-P direction to get the wires into the diagonal cut
      - Lower until the microdrive is seated on the chamber

    .. tab:: 9. Secure microdrive

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide10.png
        :align: right
        :width: 100% 

      - Insert nylon screws to fix microdrive firmly to the chamber
      - Fill in around the guide tube-electrode interface with Kwik-Cast silicone

    .. tab:: 10. Advance microdrive

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide11.png
        :align: right
        :width: 100%

      - Turn the drive screw to lower the electrode
      - Lower until the electrode tip is <1mm inside the guide tube
      - Further electrode advancement should be done during neural recording

    .. tab:: 11. Secure cap

      .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide12.png
        :align: right
        :width: 100%

      - Lower cap over microdrive 
      - Run electrode wire under cap through wire channel in chamber
      - Secure the cap with set screws (careful not to press on wire)
      - Attach electrode connectors in dental acrylic


.. _MBA_insertion:

MBA Electrode Insertion Procedure
---------------------------------------

.. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/MBA_GuideTube_Procedure.png
  :align: left
  :width: 100%

.. image:: ../_images/spacer.png
  :width: 1

.. tab:: Step 1

  i) The stainless steel stylet should be prepared with a pointed but dull tip, and a collar (made from the guide tube material) glued to it just above the top of the guide tube. The stylet should be threaded through the chamber before being attached to the stereotaxic arm. Use tape to hold the chamber in place at the top of the stylet during insertion.
  ii) Using the stereotaxic arm, lower the guide tube with the stainless steel stylet inside, through the craniotomy and along the planned trajectory to the calculated depth.
  iii) Plug the craniotomy around the guide tube with bone wax.

.. tab:: Step 2


  i) Remove the tape holding the chamber in place and gently lower the chamber down to the skull surface. Apply a thin coat of dental acrylic around the craniotomy and position the chamber on it. Fill any gaps under the chamber and build up dental acrylic around the external chamber walls, being careful not to go above the line where the chamber cap will sit.
  ii) Fill the chamber with Kwik-Cast silicone to minimize air pockets within the implant that might allow bacteria to harbour.

.. tab:: Step 3

  i) Holding the top of the guide tube in place with forceps, gently remove the stainless steel stylet.
  ii) Using sharp scissors, make a diagonal cut across the guide tube, just below the level of the chamber top.

.. tab:: Step 4

  i) With the MBA pre-loaded into the microdrive, and the microdrive attached to the stereotaxic arm, slowly lower the arm until the brush tip of the MBA is just above the guide tube.
  ii) Carefully tie a loop of Vicryl suture around the MBA shaft and gently slide it down to the brush tip. Tighten it until the splayed microwires of the brush are pulled closer together.
  iii) Position the MBA tip on the side of the guide tube where the diagonal cut is lowest, and with the tip of the brush lower than the guide tube cut is highest.


.. tab:: Step 5

  i) Using the stereotaxic arm, slowly move the MBA laterally toward the guide tube. The Brush tip should clear the lower edge of the guide tube opening and make contact with the opposite side of the opening.
  ii) If none of the microwires appear to be outside of the guide tube then begin slowly lowering the assembly using the stereotaxic arm. Any wires that have not entered the guide tube will begin to splay as the electrode tip enters the tube. You may choose to proceed and thus sacrifice some channels if the number of straggling microwires is sufficiently small, but it is otherwise recommended to raise the electrode assembly out of the tube and try again.

.. tab:: Step 6

  i) Once you are satisfied with the number of microwires that have successfully entered the top f the guide tube, continue to slowly lower the electrode assembly using the stereotaxic arm.
  ii) As you lower the electrode assembly pay careful attention to the alignment of the electrode shaft / microdrive and the guide tube. Small deviations during initial electrode tip insertion are permissible due to the flexibility of the electrode shaft, but as the portion of the electrode shaft attached to the drive shuttle approaches the guide tube, alignment may need to be corrected to minimize bending of the electrode shaft.



Microdrive Variant Designs
==============================


.. dropdown:: Microdrive cap with embedded connectors
  :open:

  One limitation of the original Ide-McMahon version of microdrive is that there is nowhere to house electrode connectors, so these end up embedded in dental acrylic surrounding the implant. This can make the connectors difficult to access, can lead to blockage of connector sockets (either with dental acrylic during surgery, or other solids after surgery), and complicates replacement of electrodes. 

  This new microdrive cap design is intended to both protect the Ide-McMahon microdrive described above and additionally houses four 32-channel (36-pin) Omnetics connectors, allowing for up to 128-channel electrodes. The arrangement of the connectors accommodates several low-profile headstages that use Omnetics 32-channel nano connectors, including `Intan RHD2164 64-channel boards <http://intantech.com/RHD2164_amp_board.html>`__), TDT Omnetics-ZIF clip adapters, and NeuroNexus 2x16 - 32 channel Omnetics adaptors.

  The additional screws used to assemble this cap are as follows:

  .. csv-table:: 
    :file: ../_static/CSVs/SCNI_IdeMcMahon_CapBOM.csv
    :widths: auto
    :header-rows: 1
    :align: left


  The .stl files for 3D-printing can be downloaded from `Thingiverse <https://www.thingiverse.com/thing:2968645>`__. We have had good results printing prototypes of this design on the SCNI's FormLabs Form2 printer. For stronger materials that can be autoclaved prior to implantation, we've outsourced printing of the parts in carbon-PEEK (`Impossible Objects <http://impossible-objects.com/products-services/>`__) and Ultem 1010 (`Stratasys <http://www.stratasys.com/materials/search/ultem1010>`__). It should be noted that, despite earlier reports to the contrary (e.g. `Mulliken et al.,(2015) <https://www.sciencedirect.com/science/article/pii/S0165027014004324>`__), carbon-PEEK is now considered unsuitable for MR-compatibility due to it's conductivity.


.. dropdown:: Chamber base with detachable connector casing
  :open:

  This design extends the footprint of the original cylindrical chamber, but in doing so provides sufficient space to place a detachable connector block, which holds up to four 32 channel Omnetics connectors (for 2x 64 channel bundles, or 1x 128 channel bundle). Making the connector block detachable facilitates electrode replacements, while keeping the connector block independent of the microdrive cap makes replacement of broken caps easier.

  Since the design is asymmetric, `two versions are provided <https://www.thingiverse.com/thing:2996902>`__ (denoted by suffix A or B on the .stl files), allowing the electrode to be located either anterior-lateral, anterior medial, posterior-lateral, or posterior-medial, depending on your needs. Either version of the connector casing and cap can be used in order to angle the connectors in such a way as to maintain easy access (e.g. avoiding headposts). The base (i.e bottom surface) of the chamber base can be further customized prior to printing by applying boolean subtraction of either a skull model, or some approximation of the skull surface.

  The spacing between the Omnetics connectors has been selected to accommodate connection of a pair of `Intan RHD2164 64-channel headstages <http://intantech.com/RHD2164_amp_board.html>`__. There are two options for installing the Omnetics connectros in the casing:

  | 1) When placing your microwire brush array order with MicroProbes, specify that the epoxy on the back of the Omnetics connectors must not exceed the width of the connector itself in order to be able to space adjacent connectors correctly.
  | 2) Arrange to send MicroProbes the 3D-printed connector casing inadvance, so that they can epoxy the Omnetics connectors directly into the casing with the correct spacing.

  .. raw:: html

    <html xmlns="http://www.w3.org/1999/xhtml"><head></head><body><dl><img width="320" src="https://user-images.githubusercontent.com/7523776/42398508-17e92bc6-8138-11e8-8cd1-991649a02d16.gif" data-src="https://user-images.githubusercontent.com/7523776/42398508-17e92bc6-8138-11e8-8cd1-991649a02d16.gif" onerror="this.style.display = 'none';" />
   <img width="320" src="https://user-images.githubusercontent.com/7523776/42398119-92cd88e8-8136-11e8-818d-564873949bcb.png" data-src="https://user-images.githubusercontent.com/7523776/42398119-92cd88e8-8136-11e8-818d-564873949bcb.png" onerror="this.style.display = 'none';" /> 
   </dl></body></html>

  We outsource printing of these parts in Ultem 1010 - a high-strength heat-resistant plastic, which retains MR-compatibility whilst still allowing us to steam autoclave the parts prior to implantation. The current cost for a single implant (chamber base, connector case, and microdrive cap) from Stratasys is $338, although savings can be made for larger orders, and also by customizing the chamber base to better fit the skull prior to ordering.

  The 3D printed parts should be sanded to ensure a smooth fit between surfaces in contact with each other. The small (1mm diameter) holes for the guide tube and ground wire may need to be drilled to ensure there is sufficient clearance (depending on the tolerances of the printing method). Additionally, six holes on the top surface of the chamber base should be tapped with a 4-40 closed-end tap (red circles on the above diagram), while the six holes in the sides of the cap should be tapped with a 4-40 through-hole tap.

  The parts required for finishing and assembly of the connector casing are as follows:

  .. csv-table:: 
    :file: ../_static/CSVs/SCNI_IdeMcMahon_ConnectorCaseBOM.csv
    :widths: 20 40 20 10
    :header-rows: 1
    :align: left




References
---------------------------------------

* Baeg et al (2021). `MRI Compatible, Customizable, and 3D-Printable Microdrive for Neuroscience Research. <https://doi.org/10.1523/ENEURO.0495-20.2021>`_
* Bondar IV, Leopold DA, Richmond BJ, Victor JD, Logothetis NK (2009). `Long-Term Stability of Visual Pattern Selective Responses of Monkey Temporal Lobe Neurons. <https://doi.org/10.1371/journal.pone.0008222>`_
* McaMahon DBT, Afuwape OAT, Ide DC, Leopold DA (2014). `One month in the life of a neuron: longitudinal single-unit electrophysiology in the monkey visual system. <https://doi.org/10.1152/jn.00052.2014>`_
* Mulliken GH, Bichot NP, Ghadooshahy A, Sharmab J, Kornblith S, Philcock M, Desimone R (2015). `Custom-fit radiolucent cranial implants for neurophysiological recording and stimulation. <https://doi.org/10.1016/j.jneumeth.2014.12.011>`_
* Englitz B, David S, Depireux DA, Shamma SA (2011). `The Array Drive : Optimizing the Yield and Flexibility of Chronic, Multielectrode Array Recordings <http://www.open-ephys.org/multielectrode-array-drive/>`_