## EX. NO: 3.1 — CREATION OF A 3D MODEL FROM ORTHOGRAPHIC PROJECTIONS

## DATE: 05/11/2026

## AIM:

To construct an accurate 3D parametric solid model in Autodesk Fusion 360 using the dimensions and geometric details provided in the given orthographic views (Front, Top, and Side views).

## HARDWARE & SOFTWARE REQUIREMENTS
## Component	Specification
--Software	Autodesk Fusion 360 (Student / Commercial License)
--Operating System	Windows 10 / 11 (64-bit)
--Processor	64-bit multi-core processor (x86-64 or ARM64)
--Memory (RAM)	8 GB minimum (16 GB recommended)
--Graphics (GPU)	Dedicated GPU with 1 GB+ VRAM (DirectX 11 compliant)
--Network	Broadband internet connection for cloud storage & sync
## TOOLS & COMMANDS USED
 Sketch Tools: Create Sketch, Line (L), Circle (C), Two-Point Rectangle (R), Trim (T), Sketch Dimension (D)
 Geometric Constraints: Coincident, Horizontal/Vertical, Tangent, Equal, Parallel, Symmetry
 Solid Modeling Features: Extrude (E), Hole (H), Fillet (F), Chamfer
 Inspection & Visuals: Inspect > Measure (I), Appearance (A)
## PRINCIPLE / CONCEPT

Orthographic projection represents a three-dimensional object using two or more 2D views projected onto orthogonal reference planes (Horizontal Plane, Vertical Plane, and Profile Plane).

## Solid modeling in CAD reverses this process:

Interpret height, width, and depth across the standard views.
Sketch the most descriptive cross-section on the appropriate reference plane.
Add material volume using solid modeling operations (Extrude / Revolve).
Apply secondary cuts, bosses, and feature detailing until all orthographic requirements are satisfied.

## PROCEDURE
## Step 1: Document & Environment Setup
--Launch Autodesk Fusion 360 and create a New Design (Ctrl + N).
--Verify document units in the browser tree under Document Settings (set to Millimeters (mm)).
--Ensure the design history timeline is enabled at the bottom of the window.
## Step 2: Base Sketch Creation
--Click Create Sketch on the toolbar.
--Select the base reference plane corresponding to the most descriptive primary view (e.g., XY plane for front elevation or XZ plane for top plan).
--Using the Line, Rectangle, and Arc tools, draw the rough profile representing the primary baseline contour.
## Step 3: Constraining and Dimensioning the Sketch
--Apply Geometric Constraints (Horizontal, Vertical, Tangent, Coincident) to lock the geometry's behavior.
--Anchor at least one key point or symmetry axis to the Origin (0,0,0).
--Press D to activate Sketch Dimension and apply exact linear and angular dimensions as specified in the drawing.
--Verify that all sketch curves turn black, indicating the sketch is Fully Constrained.
--Click Finish Sketch.
## Step 4: Primary Solid Feature (Base Extrusion)
--Select the closed profile and press E to open the Extrude dialog.
--Set the extrusion depth corresponding to the third dimension indicated in the orthogonal view.
--Choose the operation as New Body (or Symmetric extrusion if the part is symmetrical across the center plane) and click OK.
## Step 5: Secondary Features (Cuts, Holes, and Ribs)
--Select a planar face on the 3D body and click Create Sketch.
--Sketch secondary features (e.g., internal pockets, through-holes, slots, or step cuts) matching the corresponding orthographic views.
--Fully dimension and constrain the secondary sketches.
--Use Extrude with the Cut operation (set distance to To Object or All for through-holes) to subtract material.
## Step 6: Finishing & Engineering Detailing
--Apply Fillets (F) and Chamfers to edges as specified in the drawing tolerances/notes.
--Use the Inspect > Measure (I) tool to verify critical linear dimensions, wall thicknesses, and center-to-center distances against the orthographic sheet.
## Step 7: Material Assignment & Saving
--Right-click the root component in the browser, select Physical Material, and assign the specified material (e.g., Mild Steel / Aluminum).
--Save the project to your Fusion 360 cloud folder (Ctrl + S) with a standardized naming convention: Ex3_1_<RollNumber>_<Name>.
--(Optional) Export a copy locally in standard format (.step / .f3d).

## PRECAUTIONS

--Always start sketching from or reference the coordinate Origin to avoid floating bodies.
--Do not proceed to solid features with an under-constrained sketch (curves must turn black/padlock icon should appear in the browser tree).
--Avoid overlapping or unclosed sketch contours when preparing for extrusion.
--Place edge blends (fillets and chamfers) at the end of the modeling timeline, not inside 2D sketches, to maintain ease of editing.

## INPUT:
![image](https://user-images.githubusercontent.com/113594316/198551872-276f8b80-bea8-4d4a-b2e8-bfdcd1e9d3cc.png)

## OUTPUT:
<img width="740" height="686" alt="Screenshot 2026-11-10 133211" src="https://github.com/user-attachments/assets/7f8912d0-5272-4dcd-b098-df8d07f1ded2" />
## Drawing:
<img width="970" height="690" alt="Screenshot 2026-11-10 133220" src="https://github.com/user-attachments/assets/029ba952-01a6-473b-b76b-7edce9eee8ec" />

## RESULT:
The 3D parametric solid model was successfully created from the given orthographic projections in Autodesk Fusion 360 according to the specified dimensions and geometric tolerances.

