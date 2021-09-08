.. _NA_MIDAS

=====================================================================
|HW| Multidrive Implant Designer for Accurate Stereotaxy (MIDAS)
=====================================================================

.. |HW| image:: _images/Icons/oshw_button.png
  :height: 30
  :target: https://www.oshwa.org/

.. |SW| image:: _images/Icons/osi_button.png
  :height: 30
  :target: https://opensource.org/



Manual Multidrive Customization in FreeCAD
===============================================

The following guide provides step-by-step instructions for manually customizing the digital model of the multidrive system in the open-source software FreeCAD. Specifically the part names are based on the version of the file :code:`Multidrive_Livingstone_V4Custom.FCStd` (July 2019).

1. Customize the drill guides
---------------------------------

In the DrillGuides folder, select the DrillGuideHole_1 part
Update the X and Y position of the part as desired
Select the DrillGuide_blank part
Hold the Command key down and reselect the DrillGuideHole_1 part
In the ‘Parts’ workbench, click the Boolean subtraction tool icon.
Select the final Cut part and click File > Export and save the grid part as a .stl file for 3D printing. 
Repeat this process to create a drill guide for each electrode location. You may be able to fit multiple drill guide screws (M4 vented screws)

2) Customize the guide-tube guide grid
------------------------------------------------------------------

In the Grid folder, select the ElectrodeHole part
Update the X and Y position of the part as desired
Select the Grid_blank part
Hold the Command key down and reselect the ElectrodeHole part
In the Parts workbench, click the Boolean subtraction tool icon.
The product of this operation now appears as Cut. Repeat this process for as many electrodes as you want.
Select the final Cut part and click File > Export and save the grid part as a .stl file for 3D printing. 

3) Position the drive tower assembly
------------------------------------------------------------------

In the DriveTower folder, select all parts
Right click on the selected parts and copy and paste to create a new DriveTower
Set the view to from above
In the Draft workbench, select the Move tool
Enter the desired X and Y chamber-centered coordinates of the electrode target.
In the Draft workbench, select the Rotate tool
Enter a suitable rotation in the XY plane so that the drive tower fits on the chamber


4) Combine drive tower with base
------------------------------------------------------------------

In the DriveTower folder(s), select the ElectrodeHole and DriveWell parts.
In the Part workbench, use the Boolean add tool to fuse the parts together.
Select the DriveBase_Blank part and then the newly created Fusion part, and use the Boolean subtract tool.
Use the Boolean add tool to add the DriveShaft parts to the Fusion part.
Use the Boolean add tool to add the ConnectorBlock part to the Fusion part.
Export the finished drive assembly as an .stl file.


5) Combine drive tower caps
------------------------------------------------------------------

In the DriveTower folder(s), select all DriveShaftCaps
Apply the Boolean addition
Select all DriveShaftCapCutout and DriveShaftAccessHole parts
Apply the Boolean addition
Select the first Fusion part that was created in step 2, and then the second Fusion part that was created in step 4.
Apply the Boolean subtract tool.
Export the drive shaft caps as a .stl



Multidrive Surgical Implantation Procedure
================================================

.. tab:: 1. Mark locations

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide1.png
    :align: right
    :width: 50%

  - Clean the skull surface
  - Position chamber using stereotax
  - Check clearance from headpost (with attachment)
  - Mark chamber location
  - Mark screw locations

..tab:: 2. Drill skull

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide2.png
    :align: right
    :width: 50%

  - Drill and tap screw holes
  - Insert ceramic screws
  - Mark craniotomy location by lowering guide tube and stylet in stereotax
  - Drill craniotomy

.. tab:: 3. Insert guide tube

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide4.png
    :align: right
    :width: 50%

  - Lower guide tube and stylet on stereotaxic arm
  - Stop at appropriate target depth
  - Fill in the craniotomy around the guide tube with bone wax
  - Coat the bone surface with Copalite varnish to seal it

  4. Place chamber

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide5.png
    :align: right
    :width: 50%

  - Slide the chamber down over the guide tube
  - Position the chamber base against the skull surface
  - Apply a thin layer of dental acrylic between the skull and the chamber

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide6.png
    :align: right
    :width: 50%

  - Build up the dental acrylic around the chamber to cover the screws
  - Ensure that acrylic does not impede attachment of the cap
  - Make the contour of the acrylic as smooth as possible

.. tab:: 5. Remove the stylet

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide7.png
    :align: right
    :width: 50%

  - Fix the guide tube in place with a small drop of glue
  - Once glue is dry, slowly remove the stylet
  - Cut the top of the guide tube diagonally, just below the top of the chamber

..tab:: 6. Insert the electrode

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide8.png
    :align: right
    :width: 50%

  - Mount the electrode (loaded into the microdive) onto the stereotaxic arm
  - Lower the electrode until the tip approaches the guide tube
  - Tie a loose loop of vicryl suture around the tip of the brush, to reduce the splay

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide9.png
    :align: right
    :width: 50% 

  - Carefully lower the brush tip just below the top of the guide tube
  - Move the electrode in the M-L or A-P direction to get the wires into the diagonal cut
  - Lower until the microdrive is seated on the chamber

.. tab:: 7. Secure microdrive

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide10.png
    :align: right
    :width: 50% 

  - Insert nylon screws to fix microdrive firmly to the chamber
  - Fill in around the guide tube-electrode interface with Kwik-Cast silicone

.. tab:: 8. Advance microdrive

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide11.png
    :align: right
    :width: 50%

  - Turn the drive screw to lower the electrode
  - Lower until the electrode tip is <1mm inside the guide tube
  - Further electrode advancement should be done during neural recording

9. Secure cap

  .. image:: ../_images/Guides/IdeMcMahon_ImplantProcedure/Slide12.png
    :align: right
    :width: 50%

  - Lower cap over microdrive 
  - Run electrode wire under cap through wire channel in chamber
  - Secure the cap with set screws (careful not to press on wire)
  - Attach electrode connectors in dental acrylic




