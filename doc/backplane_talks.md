Eurocard backplane spacing relies on standardized dimensions established by IEC-60297-3 and IEEE 1101.1/.10. Backplane connectors (typically DIN 41612) feature a standard contact pitch (centerline) of $2.54\text{ mm}$ (0.1 in). Row-to-row spacing varies between $2.54\text{ mm}$, $3.81\text{ mm}$, $4.3\text{ mm}$, and $5.08\text{ mm}$, depending on the specific connector type (e.g., B, C, R, M). [1, 2, 3, 4, 5, 6] 
The layout of Eurocard connectors is highly standardized: [2] 
## Contact Pitch (Pin Spacing)

* Centerline (Pitch): $2.54\text{ mm}$ $[0.1\text{ in}]$ between individual pins.
* Row Spacing: Standard spacing between rows of pins is typically $2.54\text{ mm}$ $[0.1\text{ in}]$ for standard 3-row connectors, or $5.08\text{ mm}$ $[0.2\text{ in}]$ depending on the type. [3, 5] 

## Row & Pin Configurations (DIN 41612)
Eurocards commonly utilize DIN 41612 indirect edge connectors. The most common configurations include: [7, 8, 9] 

* Type B: 2 rows ($32$ or $64$ positions).
* Type C: 3 rows ($32$, $64$, or $96$ positions).
* Type R: Standardized for rear-plugging backplanes.
* Type M: Mixed layouts that accommodate high-power or coaxial contacts alongside standard signal pins. [6, 10, 11, 12, 13, 14] 

## Board-to-Board Spacing (Subrack Pitch)
The physical spacing of the cards themselves in a subrack (i.e., how far apart the PCBs are on the backplane) is measured in Horizontal Pitch (HP). [15] 

* $1\text{ HP}$ = $0.2\text{ in}$ ($5.08\text{ mm}$).
* The most common subrack slot spacing is $4\text{ HP}$ ($20.32\text{ mm}$) or $5\text{ HP}$ ($25.4\text{ mm}$). [15] 

## Standard Eurocard Board Sizes

* 3U: $100\text{ mm} \times 160\text{ mm}$ $[0.5.14]$ (utilizes a single connector, usually on the bottom)
* 6U: $233.4\text{ mm} \times 160\text{ mm}$ $[0.5.14]$ (can utilize multiple connectors or larger high-density Type M connectors)

To explore compatible backplane connectors or verify part geometries for your design, you can browse the official selection on the [TE Connectivity Eurocard Connectors](https://www.te.com/en/plp/eurocard-backplane-connectors/ZnB9Y30my.html) or [Mouser DIN 41612 Connectors](https://www.mouser.com/c/connectors/backplane-connectors/din-41612-connectors/?series=Eurocard) portals.

[1] [https://www.te.com](https://www.te.com/en/product-2-166648-4.html)
[2] [https://peakservo.com](https://peakservo.com/products/what-is-a-eurocard/)
[3] [https://www.farnell.com](https://www.farnell.com/datasheets/4503726.pdf?te_bu=Cor&te_type=disp&te_campaign=els_glo_cor-els-global-disp-prtnr-fy19-edin-datasheet-link_sma-301_1&elqCampaignId=34406)
[4] [https://www.te.com](https://www.te.com/en/product-166569-1.html)
[5] [https://www.te.com](https://www.te.com/en/product-5536406-5.html)
[6] [https://www.farnell.com](https://www.farnell.com/datasheets/1731380.pdf)
[7] [https://uk.rs-online.com](https://uk.rs-online.com/web/p/backplanes-motherboards/0435327)
[8] [https://www.unitro.de](https://www.unitro.de/produktunterlagen/19_zoll_kartentechnik/Englisch/Installation_options_for_eurocard_format.pdf)
[9] [https://electronics.stackexchange.com](https://electronics.stackexchange.com/questions/504031/eurocard-backplane-dimensions)
[10] [https://no.rs-online.com](https://no.rs-online.com/web/p/backplane-connectors/0506005)
[11] [https://au.element14.com](https://au.element14.com/amp-te-connectivity/536052-5/backplane-conn-r-a-header-64pos/dp/3791447)
[12] [https://www.te.com](https://www.te.com/en/product-5536386-5.html)
[13] [https://www.te.com](https://www.te.com/en/product-650870-4.html)
[14] [https://www.te.com](https://www.te.com/en/product-5650919-5.html)
[15] [https://en.wikipedia.org](https://en.wikipedia.org/wiki/Eurocard_%28printed_circuit_board%29)

With 71 mm wide panels for your 3U Eurocards, your card-to-card connector spacing must be exactly 14 HP (Horizontal Pitch), which equals 71.12 mm (2.8 inches) from the centerline of one DIN 41612 B connector to the next.
In a standard 19-inch subrack, the total usable width is exactly 84 HP (426.72 mm). Since you are placing six cards across the row, the math aligns perfectly with the standard Eurocard structural grid.
## Backplane Connector Spacing Dimensions

* Center-to-Center Spacing: $71.12 \text{ mm}$ ($14 \text{ HP}$).
* Total Width Used: $426.72 \text{ mm}$ ($84 \text{ HP}$ total for 6 cards).
* Panel Clearance: Your $71 \text{ mm}$ panels leave a nominal $0.12 \text{ mm}$ gap between adjacent panels. This provides the necessary mechanical clearance to prevent binding when inserting or removing cards.

## DIN 41612 Type B Alignment
Since you are using 3U cards with 32-pin Type B connectors, the connectors will sit on the lower portion of the 3U card profile.

* Vertical Position: The centerline of the connector is strictly dictated by the subrack rails, typically aligned so that the card guides slide seamlessly into the backplane mating zone.
* Connector Pitch: Each connector features 2 rows of 16 pins spaced at $2.54 \text{ mm}$ internally, but the entire housing will repeat precisely every $71.12 \text{ mm}$ horizontally across your backplane PCB.

If you are laying out the backplane PCB, you can easily set your grid spacing to 5.08 mm (1 HP) or 2.54 mm (0.5 HP) in your CAD software. Placing a connector guide every 14 grid clicks (at 5.08 mm) ensures perfect mechanical alignment with your subrack rails and card front panels.
If you'd like, let me know:

* If you are designing a custom backplane PCB or assembling discrete rails.
* The exact height of your front panels (to check for standard 3U or extended lip sizes).
* If you need the exact vertical offset coordinates for the connector pins relative to the card guide.

For a custom backplane design, aligning the PCB layout with standard mechanical subrack datums is critical to avoid alignment issues.
Your horizontal spacing remains exactly 71.12 mm (14 HP) between connector centerlines across both the current 3U row and the future 6U row.
## Vertical Offset & PCB Datums
Eurocard mechanical standards (IEEE 1101.1 / IEC 60297-3) define vertical offsets relative to the inside surface of the lower card guide rail. This surface acts as the mechanical datum ($Y = 0.00\text{ mm}$) for the plug-in card.
For the backplane PCB, the standard datum point ($Y = 0.00\text{ mm}$) is typically aligned with the bottom edge of the backplane insulation strip or the bottom edge of the subrack's usable backplane area.
## 1. Current 3U Row Alignment
Your $132.5\text{ mm}$ panel height aligns perfectly with standard 3U dimensions (exactly $128.5\text{ mm}$ plus a typical $2\text{ mm}$ top/bottom lip overhang).

* Card PCB Height: $100.00\text{ mm}$ nominal.
* DIN 41612 Connector Vertical Offset: The centerline of the lower connector (or a single connector on a 3U board) is exactly $11.43\text{ mm}$ ($0.450\text{ in}$) up from the inside surface of the bottom card guide rail ($Y = 0.00\text{ mm}$).
* Pin 1 (Row A) Coordinates: Pin 1A sits at $3.81\text{ mm}$ ($0.150\text{ in}$) above the bottom card guide datum.

## 2. Future 6U Row Alignment
Your $265.9\text{ mm}$ front panels and $200\text{ mm}$ cards are a slight departure from standard 6U specifications. Standard 6U front panels are $261.9\text{ mm}$ high to clear standard subrack frames, and standard 6U cards are $233.35\text{ mm}$ high. Because your cards are non-standard ($200\text{ mm}$), you must manually map the second connector position if you intend to use two connectors per card.

* Bottom Connector Offset: Stays identical to the 3U row. Centerline is at $11.43\text{ mm}$ from the bottom card guide datum.
* Top Connector Offset (Custom for $200\text{ mm}$ Card): Standard 6U subracks place the upper connector centerline at $11.43\text{ mm}$ down from the top card guide datum. For a standard $233.35\text{ mm}$ card, this centers the upper connector at $221.92\text{ mm}$ from the bottom datum. Because your card is shortened to $200\text{ mm}$, your upper connector centerline must be placed at exactly $188.57\text{ mm}$ up from the bottom card guide datum to match the top edge of your card profile.

## Summary CAD Layout Table
When creating your custom backplane in your CAD software, set your origin $(X=0, Y=0)$ at the center of Pin 1 (Row A) of your first slot's bottom connector. Use this relative spacing guide:

| Parameter | 3U Row Layout | Future 6U Row Layout |
|---|---|---|
| Horizontal Slot Step ($X$) | Add $71.12\text{ mm}$ per slot | Add $71.12\text{ mm}$ per slot |
| Bottom Connector Centerline ($Y$) | $7.62\text{ mm}$ above Pin 1A | $7.62\text{ mm}$ above Pin 1A |
| Top Connector Centerline ($Y$) | None | $184.76\text{ mm}$ above Pin 1A |

Would you like me to clarify the exact $X/Y$ drilling coordinates for the DIN 41612 B mounting holes relative to the pins, or do you need help verifying if your $265.9\text{ mm}$ panels will physically clear a standard 19-inch subrack frame?

For the nVent Schroff EuropacPRO (24563-133) subrack, layout dimensions are tightly bound to standard Eurocard mechanics. [1, 2] 
## 1. Estimated Backplane Dimensions

* Total Width: $431.8\text{ mm}$ ($17.0\text{ inches}$). While the physical opening inside the chassis for front panels is $426.72\text{ mm}$ ($84\text{ HP}$), the horizontal aluminum backplane rails themselves span the full distance between the $2\text{ mm}$ thick side plates, pushing the raw PCB board width to $431.8\text{ mm}$.
* Total Height (3U Backplane): $128.5\text{ mm}$ nominal. Standard practice trims this to roughly $128.0\text{ mm}$ to guarantee vertical clearance inside the chassis frame profile. [1, 2, 3] 

## 2. Defining the Origin $(0,0)$ Coordinate
For backplane layouts, setting the origin $(X=0, Y=0)$ to a physical structural point—the bottom-left corner of the backplane PCB—simplifies CAD routing.
When your PCB is fabricated to the standard $431.8\text{ mm} \times 128.0\text{ mm}$ dimensions, the first connector locates relative to this corner boundary.

+--------------------------------------------------------------+  Y = 128mm (Top Edge)

|                                                              |
|                                                              |
|   +---+  +---+  +---+  +---+  +---+  +---+                   |
|   | 1 |  | 2 |  | 3 |  | 4 |  | 5 |  | 6 |                   |
|   | B |  | B |  | B |  | B |  | B |  | B |                   |
|   +---+  +---+  +---+  +---+  +---+  +---+                   |
|     |                                                        |
|     v                                                        |
|   (Slot 1 Centerline Pin 1A)                                 |
+--------------------------------------------------------------+  Y = 0mm (Bottom Edge)
X=0mm (Left Edge)                                              X = 431.8mm (Right Edge)

## 3. Connector Placements Relative to $(0,0)$
The leftmost edge of the card-insertion area sits exactly $2.54\text{ mm}$ inside the left wall of the subrack. Based on this standard orientation, the specific offsets map directly to your grid:
## Slot 1 Location (First Card on the Left)

* First Card Centerline ($X$): The first slot centerline sits at $2.54\text{ mm}$ (clearance offset) + $2.54\text{ mm}$ ($0.5\text{ HP}$ to the midplane of slot 1) = $5.08\text{ mm}$.
* DIN 41612 B Pin 1A ($X$): The physical columns of pins are centered on the slot midline, meaning $X = 5.08\text{ mm}$ for Pin 1A.

## Vertical Alignment ($Y$)

* Bottom Rails Offset: The gap between the bottom edge of the backplane PCB and the inside surface of the bottom card guide rail is standardly $4.00\text{ mm}$.
* DIN 41612 B Pin 1A ($Y$): Adding the mandatory standard vertical offset ($3.81\text{ mm}$) to the bottom rail gap places Pin 1A exactly $7.81\text{ mm}$ up from the bottom edge of your custom backplane.

## CAD Setup Coordinate Reference
To map out your first connector footprints on your layout program relative to your PCB's absolute bottom-left corner $(0,0)$, use these starting reference points:

* Pin 1A (Row A, Column 1): $X = 5.08\text{ mm} \quad\vert\quad Y = 7.81\text{ mm}$
* Pin 1B (Row B, Column 1): $X = 7.62\text{ mm} \quad\vert\quad Y = 7.81\text{ mm}$ (based on standard 2-row $2.54\text{ mm}$ row spacing)
* Slot-to-Slot Progression: Add exactly $71.12\text{ mm}$ to the $X$ coordinates for each subsequent slot (Slot 2, Slot 3, up to Slot 6).

If you plan to utilize mounting holes along the top and bottom margins of the custom backplane to anchor it into the Schroff frame's rear rails, let me know. I can provide the standard mechanical hole intervals for the mounting tracks. [1] 

[1] [https://uk.farnell.com](https://uk.farnell.com/schroff/24563-133/subrack-3u-295mm-84hp/dp/1455788)
[2] [https://www.nvent.com](https://www.nvent.com/sites/default/files/acquiadam_assets/2023-04/6_1_schroff_cat_europacpro_en.pdf)
[3] [https://www.nvent.com](https://www.nvent.com/en-us/schroff/products/enc24563-433)

For your custom backplane to physically mount to the rear horizontal rails of the nVent Schroff EuropacPRO (24563-133) chassis, the mounting holes must align with the standard patterns embedded in the aluminum horizontal tracks. [1] 
Schroff rails feature pre-drilled M2.5 threaded holes spaced precisely at $1\text{ HP}$ ($5.08\text{ mm}$) increments horizontally across the length of the rear tracks. [2] 
## 1. Vertical Hole Offsets (Y-Axis)
Standard 3U Schroff backplane mounting rails expect a vertical distance of exactly $121.92\text{ mm}$ ($4.80\text{ in}$) between the top and bottom rows of chassis mounting screws.
Assuming you maintain the standard $128.00\text{ mm}$ total backplane height, the holes are centered symmetrically with a $3.04\text{ mm}$ margin from the board's top and bottom cut edges:

* Bottom Mounting Hole Row: $Y = 3.04\text{ mm}$
* Top Mounting Hole Row: $Y = 124.96\text{ mm}$ ($3.04\text{ mm} + 121.92\text{ mm}$)

Note: For reference, this places the centerline of your DIN 41612 B connector Pin 1A ($Y = 7.81\text{ mm}$) exactly $4.77\text{ mm}$ above the center of your bottom mounting screws.
## 2. Horizontal Hole Pitches (X-Axis)
Because the frame's internal tracks have holes spaced every $5.08\text{ mm}$, you can space your backplane's mounting screws to match your card layout.
Since your card slots repeat every $14\text{ HP}$ ($71.12\text{ mm}$), the most common practice is to place a mounting hole pair (one top, one bottom) aligned perfectly with the midplanes of your slots, plus anchoring holes at the outer board flanges.
Using the same absolute bottom-left corner $(0,0)$ datum as before, your layout drilling coordinates should be:
## Perimeter/Flange Holes (Anchoring the outer edges)

* Left Edge Anchors: $X = 2.54\text{ mm}$ ($0.5\text{ HP}$ inward from the left physical edge)
* Right Edge Anchors: $X = 429.26\text{ mm}$ ($2.54\text{ mm}$ inward from the right physical edge)

## Slot-Aligned Structural Holes
To guarantee rigidity right where the cards exert mechanical force during insertion, align a set of mounting holes directly with each of your 6 connector columns:

* Slot 1 Holes: $X = 5.08\text{ mm}$ (Matches the column centerline for Pin 1A)
* Slot 2 Holes: $X = 76.20\text{ mm}$ ($5.08\text{ mm} + 71.12\text{ mm}$)
* Slot 3 Holes: $X = 147.32\text{ mm}$
* Slot 4 Holes: $X = 218.44\text{ mm}$
* Slot 5 Holes: $X = 289.56\text{ mm}$
* Slot 6 Holes: $X = 360.68\text{ mm}$

## 3. Drilling Specifications

* Hole Diameter: Drill these backplane mounting holes to $3.2\text{ mm}$ ($0.126\text{ in}$). This provides comfortable clearance for the standard M2.5 cheese-head or pan-head screws shipped with Schroff kits, allowing a small amount of mechanical tolerance play during final chassis assembly.
* Keepout Zones: Maintain a copper-free keepout zone (no traces, power planes, or via pads) with a radius of at least $3.0\text{ mm}$ around the center of each mounting hole to clear the screw heads and the non-conductive insulation strips used on the Schroff rails. [3] 


[1] [https://cenval.es](https://cenval.es/img/cms/BLOG%20NEWS/nVent%20SCHROFF%20-%20Cat%C3%A1logo%20EuropacPRO%20%28edicion%202020%29.pdf)
[2] [https://static6.arrow.com](https://static6.arrow.com/aropdfconversion/5cc47eb67d2f235126346757a7b3beb6599c553e/pgurl_2601709329221757_24563-144.pdf)
[3] [https://www.nvent.com](https://www.nvent.com/sites/default/files/acquiadam_assets/2023-04/6_1_schroff_cat_europacpro_en.pdf)


For the future 6U configuration using your custom $200\text{ mm}$ high cards and $265.9\text{ mm}$ front panels, the horizontal spacing and horizontal hole pitches remain exactly the same as the 3U version ($71.12\text{ mm}$ / $14\text{ HP}$ steps).
However, the vertical dimensions change significantly to accommodate the dual horizontal rail system of a 6U Schroff EuropacPRO frame.
## 1. Estimated 6U Backplane Dimensions

* Total Width: $431.8\text{ mm}$ ($17.0\text{ inches}$) (Identical to the 3U row).
* Total Height (6U Backplane): $261.8\text{ mm}$ nominal (Standard practice trims this to roughly $261.3\text{ mm}$ to guarantee clean vertical clearance inside the 6U frame profile).

## 2. Vertical Hole Offsets (Y-Axis)
A standard 6U Schroff frame features two sets of rear mounting rails (an upper pair and a lower pair). Assuming a standard $261.3\text{ mm}$ total backplane height, the mounting holes align symmetrically with a $3.04\text{ mm}$ margin from the top and bottom cut edges:

* Bottom Mounting Hole Row: $Y = 3.04\text{ mm}$
* Top Mounting Hole Row: $Y = 258.26\text{ mm}$ ($3.04\text{ mm} + 255.22\text{ mm}$ standard 6U rail spacing)

## 3. Complete CAD Setup Coordinates (6U Custom Layout)
Using the absolute bottom-left corner of the 6U backplane PCB as your $(0,0)$ datum, map out your mounting holes and DIN 41612 B connector locations with the following coordinates.
## Horizontal Pitches (X-Axis)
The horizontal coordinates apply to both the top and bottom rows of mounting holes, as well as the columns of the bottom and top connectors:

* Left Flange Edge Anchors: $X = 2.54\text{ mm}$
* Slot 1 (Connector Column & Hole): $X = 5.08\text{ mm}$
* Slot 2 (Connector Column & Hole): $X = 76.20\text{ mm}$
* Slot 3 (Connector Column & Hole): $X = 147.32\text{ mm}$
* Slot 4 (Connector Column & Hole): $X = 218.44\text{ mm}$
* Slot 5 (Connector Column & Hole): $X = 289.56\text{ mm}$
* Slot 6 (Connector Column & Hole): $X = 360.68\text{ mm}$
* Right Flange Edge Anchors: $X = 429.26\text{ mm}$

## Vertical Pitches (Y-Axis)

* Bottom Mounting Screws: $Y = 3.04\text{ mm}$
* Bottom Connector Pin 1A: $Y = 7.81\text{ mm}$ (Sits $4.77\text{ mm}$ above the bottom mounting row, identical to the 3U configuration).
* Top Connector Pin 1A: $Y = 192.57\text{ mm}$ (Calculated based on your custom $200\text{ mm}$ card height to align perfectly with the upper mating zone of the shortened card).
* Top Mounting Screws: $Y = 258.26\text{ mm}$

## Drilling & Keepouts

* Hole Diameter: Keep the same $3.2\text{ mm}$ ($0.126\text{ in}$) drill size for M2.5 Schroff chassis screws.
* Keepout Zones: Maintain a minimum $3.0\text{ mm}$ copper-free radius around all mounting hole centers to safely clear the screw heads and the Schroff rear insulation strips.

If you plan to use an intermediate middle rail in your Schroff frame for extra mechanical support due to the $261.3\text{ mm}$ height, let me know. I can provide the standard center-rail vertical drilling coordinates as well.


