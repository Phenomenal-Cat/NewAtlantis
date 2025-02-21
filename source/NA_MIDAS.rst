.. _NA_MIDAS:

=====================================================================
Multidrive Implant Designer for Accurate Stereotaxy (MIDAS)
=====================================================================

.. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/FreeCAD_Livingstone.jpeg
  :width: 40%
  :align: right

MIDAS (Multidrive Implant Design for Accurate Stereotaxy) is a system for designing and implanting customized multi-shaft microdrives for use with chronic :ref:`microwire brush array (MBA) electrodes <mba>`. It was developed using open-source CAD software and 3D-printing to allow greater flexibility, improved anatomical targeting accuracy. MIDAS offers several important advantages over previous approaches:

- **Improved targeting accuracy**
  The MIDAS system divides implantation into two separate surgical procedures: first chamber implant, followed by electrode insertion. In between these two surgeries, a chamber localizer MRI scan is acquired, using MR contrast agent to visualize the chamber orientation relative to target regions. 

- **Increased electrode density**
  The MIDAS system shrinks the footprint of the microdrive assembly (compaired to the :ref:`Ide-McMahon drive <chronicMicrodrives>`), allowing for multiple independent microdrives to be housed over the same chamber. This allows researchers to increase the total channel count by using multiple :ref:`MBAs <mba>`, instead of having to increase the channel count of each MBA (:ref:`which is known to be problematic <MBA_TipDev>`). This additionally increases spatial sampling of the target region(s) using MBAs.

- **Reduced infection exposure**
  Since the skull remains intact during the first surgery (except for screw holes) and the  craniotomies made during the second surgery are small (~3mm) and inside the sealed chamber, the opportunities for ingress of bacteria that could potentially lead to intracranial infections are reduced.

- **Improved ease of replacement**
  The MDIAS system is modular. Importantly, unlike the Ide-McMahon system, the electrode guide tubes are glued to a *removable* grid, thus allowing for complete replacement of currently implanted electrodes if required.

The concept for the multidrive -an even smaller drive system than the original microdrive described in McMahon et al. (2014)- was inspired by the `EDDS Array Drive <https://www.microprobes.com/component/rsform/form/13-micro-electrode-array-mea-for-the-edds-microdrive?Itemid=1034>`_. The need for targeting multiple sites in close proximity to each other in the same hemisphere lead to development of the multidrive. The drive screws are PEEK 4-40 thread machine heads, which pass through a 3D-printed thermoplastic drive shuttle. The wings of the shuttle keep it locked inside the drive shaft, while a channel on the front surface allows close mating with the electrode shaft, which is epoxied directly to it.


Manual Multidrive Customization in FreeCAD
===============================================

The following guide provides step-by-step instructions for manually customizing the digital model of the multidrive system in the open-source software FreeCAD. Specifically the part names are based on the version of the file :code:`Multidrive_Mini_V5.FCStd` (2025).


.. button-link:: https://www.thingiverse.com/thing:3757888
    :color: primary
    :outline:

    Download CAD Files


.. card::
  :class-body: sd-bg-dark sd-text-justify sd-text-light

  .. tab-set::

    .. tab-item:: 1. Drill guides

      .. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Slide2.png
        :align: right
        :width: 100%

      - In the :bdg-primary:`DrillGuides` folder, select the :bdg-success:`DrillGuideHole_1` part
      - Update the X and Y position of the part as desired
      - Select the :bdg-success:`DrillGuide_blank` part
      - Hold the :bdg-secondary:`Command,badge-secondary` key down and reselect the :bdg-success:`DrillGuideHole_1,badge-success` part
      - In the :bdg-warning:`Parts` workbench, click the :bdg-warning:`Boolean subtraction` tool icon.
      - Select the final :bdg-success:`Cut` part and click :bdg-secondary:`File` > :bdg-secondary:`Export` and save the grid part as a .stl file for 3D printing. 
      - Repeat this process to create a drill guide for each electrode location. You may be able to fit multiple drill guide screws (M4 vented screws)

    .. tab-item:: 2) Guide-tube grid

      .. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Slide3.png
        :align: right
        :width: 100%

      - In the :bdg-primary:`Grid` folder, select the :bdg-success:`ElectrodeHole` part
      - Update the X and Y position of the part as desired
      - Select the :bdg-success:`Grid_blank` part
      - Hold the :bdg-secondary:`Command` key down and reselect the :bdg-success:`ElectrodeHole` part
      - In the :bdg-warning:`Parts` workbench, click the :bdg-danger:`Boolean subtraction` tool icon.
      - The product of this operation now appears as :bdg-success:`Cut`. Repeat this process for as many electrodes as you want.
      - Select the final Cut part and click :bdg-secondary:`File` > :bdg-secondary:`Export` and save the grid part as a .stl file for 3D printing. 

    .. tab-item:: 3) Drive tower positioning

      .. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Slide4.png
        :align: right
        :width: 100%

      - In the :bdg-primary:`DriveTower` folder, select all parts
      - Right click on the selected parts and copy and paste to create a new DriveTower
      - Set the view to from above
      - In the :bdg-warning:`Draft` workbench, select the :bdg-danger:`Move` tool
      - Enter the desired X and Y chamber-centered coordinates of the electrode target.
      - In the :bdg-warning:`Draft` workbench, select the :bdg-danger:`Rotate`  tool
      - Enter a suitable rotation in the XY plane so that the drive tower fits on the chamber

    .. tab-item:: 4) Merge drive towers

      .. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Slide5.png
        :align: right
        :width: 100%

      - In the :bdg-primary:`DriveTower` folder(s), select the :bdg-success:`ElectrodeHole,badge-success` and :bdg-success:`DriveWell` parts.
      - In the :bdg-warning:`Part` workbench, use the :badge`Boolean add,badge-danger` tool to fuse the parts together.
      - Select the :bdg-success:`DriveBase_Blank,badge-success` part and then the newly created Fusion part, and use the Boolean subtract tool.
      - Use the :bdg-danger:`Boolean add` tool to add the :bdg-success:`DriveShaft` parts to the :bdg-success:`Fusion` part.
      - Use the :bdg-danger:`Boolean add` tool to add the :bdg-success:`ConnectorBlock` part to the :bdg-success:`Fusion` part.
      - Export the finished drive assembly as an .stl file.


    .. tab-item:: 5) Merge drive caps

      .. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Slide6.png
        :align: right
        :width: 100%

      - In the :bdg-primary:`DriveTower,badge-primary` folder(s), select all :bdg-success:`DriveShaftCaps,badge-success` parts
      - Apply the :badge`Boolean add,badge-danger` tool 
      - Select all :bdg-success:`DriveShaftCapCutout,badge-success` and :bdg-success:`DriveShaftAccessHole,badge-success` parts
      - Apply the :bdg-danger:`Boolean add` tool 
      - Select the first :bdg-success:`Fusion,badge-success` part that was created in step 2, and then the second :badge`Fusion,badge-success` part that was created in step 4.
      - Apply the :bdg-danger:`Boolean subtract` tool.
      - Export the drive shaft caps as a .stl



Multidrive Surgical Implantation Procedure
================================================

Surgery #1: Chamber implantation
-----------------------------------


.. dropdown:: Surgery 1 Tools and Materials
  :open:
  :class-title: sd-bg-primary sd-text-light sd-text-justify
  :class-body: sd-bg-light sd-text-justify 

  .. csv-table::
    :file: _static/CSVs/MIDAS_Surgery1_materials.csv
    :align: left
    :header-rows: 1
    :widths: auto

.. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Multidrive_Surgery1_CoordinateSheet.png
  :align: right
  :width: 50%


1.Place animal in stereotax and confirm position with tooth marker

2.After sterilization and draping, open the skin with scalpel and separate the skin from muscle by blunt dissection.

3.Remove any cement that may be in the way of the surgery with dremel or drill. Clean the skull and keep moist.

4.Using the stereotaxic arm, find the X and Y position of the skull target. 

5.Use a pen to mark the location of chamber center on the skull.

6.Attach the chamber to the stereotaxic arm and lower it until it makes contact with the skull surface. Mark an outline of the chamber base against the skull and markthe desired screw locations for drilling.

7.Use hand drill and tap to place ceramic screws around the chamber.

8.Place a grounding screw near the chamber.

9.Put Quick-Stat FS on the skull and stop bleeding.

10.Put dental varnish (Copalite) on the skull 

11.Put some thin cement (or Geristore) on the skull

12.Place Chamber on the skull using stereotaxic arm. Pass the grounding gold pin through a hole of the chamber.

13.Check chamber height and angle, and cement the chamber to ceramic screws and skull

14.Solder copper wire to the grounding gold pin.

15.Attach temporary cap to chamber (and apply high vacuum grease).

16.Close up the scalp



Chamber localization MRI scan
----------------------------------

.. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Multidrive_localizerScan.png
  :align: right
  :width: 50%


.. container:: clearer

    .. image :: ../_images/spacer.png
       :width: 1

Surgery #2: Electrode implantation
-----------------------------------

.. dropdown:: Surgery 2 Tools and Materials
  :open:
  :class-title: sd-bg-primary sd-text-light sd-text-justify
  :class-body: sd-bg-light sd-text-justify 

  .. csv-table::
    :file: _static/CSVs/MIDAS_Surgery2_materials.csv
    :align: left
    :header-rows: 1
    :widths: auto

  .. csv-table::
    :file: _static/CSVs/MIDAS_Surgery2_tools.csv
    :align: left
    :header-rows: 1
    :widths: auto

.. image:: _images/Designs/MIDAS/ChamberEditing_FreeCAD/Multidrive_Surgery2_CoordinateSheet.png
  :align: right
  :width: 50%


PREPARATION
~~~~~~~~~~~~~~~~

1.Place animal in stereotax.

2.Remove the temporary chamber cap and clean the chamber.

3.Sterilize and drape surgical area.

GUIDE TUBE PLACEMENT
~~~~~~~~~~~~~~~~~~~~~~~~~

4.Insert the custom drill guide grid into the chamber.

5.Insert the 1.5 mm drill bit through the holes of the drill guide grid and make the craniotomies.

6.Remove the drill-guide grid and inspect the craniotomies. Flush the chamber again.

7.Insert the custom electrode guide grid into the chamber.

8.Place the custom guide-tube insertion guide in place.

9.Insert the guide-tube(s) into the holes of the guide-tube insertion guideand then electrode guide grid, through the craniotomy and down to theappropriate depth for the desired target.

10.With the guide tube inserted, apply a small dab of glue where the guide tube meets the electrode guide grid.

11.Remove stylet(s) and guide tube(s) from the guide tube carefully.

12.Cut guide tube(s) just below the guide-tube insertion guide.

13.Remove the guide-tube insertion guide. 

14.Glue the grid to the chamber.

15.Fill the space below the electrode grid with Kwik-Cast silicone sealant.

16.Cut the guide tube further if necessary, so the end of guide tube all beneath the edge of microdrive assembly.

ELECTRODE PLACEMENT
~~~~~~~~~~~~~~~~~~~~~~~~~

17.Adjust the length of electrode(s) on the microdrive so the tip ends 1 mm above the end of the guide tube.

18.Hold the microdrive assembly with microdrive holder and put on the stereotaxic arm.

19.Using surgical head loupe, lower the electrode close to the guide tube.

20.Slide the insertion sleeve down along the electrode and place into the guide tube end.

21.Lower the electrode into the guide tube, approx. 5-10 mm.

22.Slide the insertion sleeve up and detach from the electrode.

23.Put grounding wires into the hole of the microdrive assembly.

24.Lower the electrode further and place the microdrive on the chamber.

25.Screw microdrive down to the chamber.

26.Remove the microdrive holder and stereotaxic arm.

27.Fill the space at the guide tube end with Kwik-Cast silicone sealant.

28.Connect the grounding wires between the connector and gold pinusing soldering iron.

29.Connect Apollo system to the connector.

30.Using microdrive lower the electrode(s) to the target region, withchecking recording signal.

31.Place Chamber cap.
