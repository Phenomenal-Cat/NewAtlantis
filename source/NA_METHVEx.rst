.. _NA_METHVEX:

====================================================================
METHVEX - Monkey Eye Tracking for Head-free Visual EXperiments
====================================================================



.. grid:: 

  .. grid-item::
    :columns: 9
    :margin: 0
    :padding: 2 0 0 0

    Neuroscientists are increasingly interested in studying brains in the contexts they evolved to process, which requires greater ethological validity of experimental designs.
    To take advantage of paradigms involving immersive environments including
    large enclosures and virtual-reality dome projections, it is desirable to record the subject's eye position (in head-centered coordinates) in head-free animals.
    This poses several technical challenges:

    1) The head-mounted video eye-tracking apparatus must be sufficiently light and robust for extended use by chaired animals.

    2) The frames that hold the polarizing filters of the 3D glasses and the eye cameras in front of the eyes must minimize the portion of the visual field that they occluded. 

    3) Head direction signals (in world-centered coordinates) must be integrated with eye direction signals (in head-centered coordinates) in order to compute gaze direction in world-centered coordinates online.


  .. grid-item::
    :columns: 3
    :margin: 0
    :padding: 2 0 0 0

    .. image:: _images/Designs/METHVEX/METHVEx_30deg.png
      :width: 100%
      :align: right


`PupilLabs <https://pupil-labs.com/>`_ video eye tracker
===========================================================================

.. grid:: 

  .. grid-item::
    :columns: 7
    :margin: 0
    :padding: 0

    Many of the commercial video eye-tracking cameras intended to be head-mounted on human subjects are relatively large and heavy, thus obstructing the visual field and putting strain on the wearer. The open-source system from `Pupil Labs <https://pupil-labs.com/>`_ utilizes some of the smallest and lightest cameras available. Many of the camera specs are comparable to those of the industry standards (such as `SR Research's EyeLink <https://www.sr-research.com/>`_) (see the table and `Ehinger et al., 2019 <https://doi.org/10.7717/peerj.7086>`_ for a more in depth comparison of performance), but the hardware are substantially smaller and lighter. This allows them to be discretely mounted below the eye with a direct line of sight - thus avoiding the need for cumbersome and delicate hot mirrors, while still minimizing occlusion of the subject's visual field.

  .. grid-item::
    :columns: 5
    :margin: 0
    :padding: 0

    .. image:: _images/Logos/PupilLabs.svg
      :width: 200px
      :align: right
      :target: https://pupil-labs.com/

    +--------------------+------------------------+------------+
    |                    | SR Research EyeLink II | Pupil Labs |
    +====================+========================+============+
    | Sampling frequency | 500 Hz                 | 200 Hz     |
    +--------------------+------------------------+------------+
    | Gaze accuracy      | 0.5 deg                | 0.6 deg    |
    +--------------------+------------------------+------------+
    | Gaze precision     | 0.01 deg               | 0.08 deg   |
    +--------------------+------------------------+------------+
    | Camera Latency     | 3 ms                   | 4.5 ms     |
    +--------------------+------------------------+------------+
    | Weight             | XXX g                  | 32 g       |
    +--------------------+------------------------+------------+
    | Cost               | $20,000                | $2,000     |
    +--------------------+------------------------+------------+





.. grid:: 

  .. grid-item::
    :columns: 8
    :margin: 0
    :padding: 0 0 0 2

    The PupilLabs `eye cameras <https://pupil-labs.com/products/core/accessories>`_ are very small and can be easily removed from the black 3D-printed casing provided for human head-mounted use. Instead, we designed a lower-profile camera casing to integrate with the 3D glasses frames that the macaque subjects wear, as seen in the photo. The camera and LED slot into the casing from above, with the ribbon cable protruding temporally (i.e. to the subject's right for the right eye camera). 


  .. grid-item::
    :columns: 4
    :margin: 0
    :padding: 0

    .. image:: _images/Designs/METHVEX/PupilLabs_Image1.jpg
      :width: 100%
      :align: right




3D glasses frames for NHP
==================================

.. grid:: 

  .. grid-item::
    :columns: 8
    :margin: 0
    :padding: 0 0 0 2

    To minimize occlusion of the subject's field of view (FOV), we designed a pair of spectacle frames to closely fit the contours of the
    face of an average Rhesus macaque (see computer renders above). The wrap-around frame style can optionally house circular polarizing filters (taken from commercial 3D glasses with flexible filter material) for use in immersive dome projection environments. This not only maximizes the FOV but also preserves continuity across the visual field.

    Using open-source `CAD software <www.freecad.org>`_, the :bdg-success:`camera holder` casing is digitally positioned appropriately for the subject's anatomy (e.g. angled upward and inwards towards the subject's pupil) and fused with the glasses :bdg-primary:`frames` into a single .stl file for 3D-printing. Customized mounting points can be added to the top of the frames, for securing them to the subject's head. The frames should be 3D printed in a relatively impact-resistant material, such as `Kevlar-reinforced <https://markforged.com/materials/continuous-fibers/kevlar>`_ thermoplastic, for durability. 

    .. button-link:: https://grabcad.com/library/methvex-eye-tracking-camera-mount-1
       :color: primary

       GrabCAD Download


  .. grid-item::
    :columns: 4
    :margin: 0
    :padding: 0

    .. image:: _images/Designs/METHVEX/Camera_positioning.png
      :width: 100%
      :align: right



