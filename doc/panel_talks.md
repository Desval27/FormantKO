A 71 mm wide front panel corresponds to an industry-standard 14 HP Eurocard module width (nominally 70.78 mm to 71.12 mm). [1, 2] 
According to standard Schroff configurations for a 14 HP front panel, the module's component board is not centered down the exact middle of the 71 mm frame. Instead, the PCB card-guides align the card closer to the left edge to maintain the standardized chassis slot intervals. [3] 
The drill holes for your 60807-011 brackets must be placed at the following absolute panel coordinates: [3] 
## 1. Absolute Drill Hole Coordinates
Measure your dimensions from the Left-Most Edge and the Top-Most Edge of the raw aluminum front panel:

* Horizontal Position (X-Axis): 35.22 mm from the left-most edge.
* Upper Hole Vertical Position (Y-Axis): 14.20 mm down from the top edge.
* Lower Hole Vertical Position (Y-Axis): 114.20 mm down from the top edge. [2] 

(Note: The absolute vertical distance between your two drilled holes will be exactly 100.00 mm).
------------------------------
## 2. Panel Mounting Screw Hole Coordinates (To Secure Panel to Subrack Rails)
Because a 14 HP module is wide, it must be secured to the chassis subrack frame using its own peripheral mounting screws (independent of the PCB bracket screws). [3] 
To secure the panel itself to your subrack rails, add your external subrack mounting holes at these coordinates: [3] 

* Top-Left Subrack Hole: 7.45 mm from the left edge, 4.00 mm down from the top edge.
* Bottom-Left Subrack Hole: 7.45 mm from the left edge, 124.40 mm down from the top edge (or 4.00 mm up from the bottom).
* Top-Right Subrack Hole: 63.33 mm from the left edge, 4.00 mm down from the top edge.
* Bottom-Right Subrack Hole: 63.33 mm from the left edge, 124.40 mm down from the top edge. [4] 

------------------------------
## 3. Clear Visual Summary for Fabricating Your Front Panel
Use this 2D dimensional map when drilling or programming your CNC mill profile:

  0,0 (TOP-LEFT CORNER)
   +-----------------------------------------------------------+

   |   (O) 7.45mm, 4.00mm                         (O) 63.33mm  | <-- Chassis Rail Screws
   |                                                           |
   |                                                           |
   |                ( ) 35.22mm, 14.20mm                       | <-- UPPER BRACKET (60807-011)
   |                                                           |
   |                                                           |
   |                                                           |
   |                                                           |
   |                                                           |
   |                                                           |
   |                ( ) 35.22mm, 114.20mm                      | <-- LOWER BRACKET (60807-011)
   |                                                           |
   |                                                           |
   |   (O) 7.45mm, 124.40mm                       (O) 63.33mm  | <-- Chassis Rail Screws
   +-----------------------------------------------------------+
                                                               71.00mm, 128.40mm

## 4. Technical Design Reminders

* Drill Sizes: Use a 2.6 mm to 2.8 mm drill bit for the bracket holes at the 35.22 mm line to allow clean pass-through for the M2.5 screws. Use a 5.9 mm to 6.0 mm bit for the outer four subrack rail holes to clear standard subrack M2.5 collar sleeves.
* Chassis Clearance: The standard total vertical height of this front panel is 128.40 mm. [1, 2, 4, 5] 

Are you handling this panel milling manually on a drill press, or would a standard DXF profile file help you load it directly into CAM/CNC machining software?

[1] [https://uk.rs-online.com](https://uk.rs-online.com/web/p/rack-panels/4372028)
[2] [https://www.nvent.com](https://www.nvent.com/en-at/schroff/products/front-panel)
[3] [https://www.nvent.com](https://www.nvent.com/sites/default/files/acquiadam_assets/2023-04/7_1_schroff_cat_frontpanels_en.pdf)
[4] [https://www.farnell.com](https://www.farnell.com/datasheets/2622644.pdf)
[5] [https://www.nvent.com](https://www.nvent.com/en-us/schroff/products/enc20846-450)

