# RoPod 

 RoPod is a toolkit that comprises microscopy chambers, in which you can grow and image Arabidopsis thaliana seedlings roots without taking the plants out, and a detailed protocol on how to do it. No stress!
Check out our  [semi-automated tool for root hair growth](https://github.com/AlyonaMinina/RoPod.Image.Processing)







<br/>
<br/>
<details><summary>Why use RoPod</summary> <br/>  
<p align="center">
<img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v23/RoPod%2023.4%20empty.png?raw=true" width="300"> 
<img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20with%20seedlings%201.png?raw=true" width="300"> 
<img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.applications/mounted%20on%20confocal%20RoPod%205.png?raw=true" width="300" > 
</p>

- Plants are **grown and imaged within the same chamber**, thus sample mounting and imaging causes there  little to none mechanical stress<br/><br/> 
- RoPods **prevent samples from drying during imaging**, allowing  long-term time-lapse series <br/><br/>
- Plant growth within RoPod **requires very small volume of the medium**, thus drug treatment will require a small amount of compounds <br/><br/>
- The watertight RoPods allow **drug treatment in chambers positioned vertically and horizontally**<br/><br/>
- RoPods allows **multiple biological replicates being imaged simultaniously** (up to 20 seedlings in a RoPod v23) <br/><br/>
- **Plants are immobilized within the chamber**, thus the same plant can be easily tracked in a RoPod in multiple imaging sessions <br/><br/>
- RoPods with individual lanes prevent roots crossing during growth and make **tracking of biological replicates easy**<br/><br/>
- **RoPods are very cheap and reusable**, printing one chamber with a lid takes ca 10g of a PETG or PLA filament and two 24 x 60mm microscopy coverglass (#1.5, i.e. 0.16-0.19 mm thick)<br/><br/>
- The **microscopy-grade glass is printed into the plastic** and will never detach from the chamber in the middle of your experiment<br/><br/> 
</details>

<details><summary>How to grow Arabidopsis in RoPods</summary> 
<br/> 
 
[<img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.applications/Screenshot%20for%20growing%20Arabidopsis%20in%20RoPods%20demo%20video.png?raw=true" width="500" title="Seed plating demo video">](https://www.youtube.com/watch?v=jWTp5Sgqe-Q&ab_channel=AlyonaMinina)
 
 In this video you can find a short step-by-step demonstration of how to prep RoPod chambers for *Arabidopsis thaliana* growth.
<br/>
<br/>

- **Step 1. Sterilize the RoPod.**
 The quickest way to do it is using UV in a laminar flow hood. Place the open chamber and the lid (inner side up) under the UV light, 30 minutes of exposure is usually sufficient.
 
 - **Step 2. Cast the growth medium.**
Thaw 0.5x MS in a microwave, let it cool to 60 C and pipette 3-4 mL into the sterile chamber. Make sure the medium is evenly distributed in the chamber and there are no bubbles.
 
 - **Step 3. Remove a strip of the growth medium.**
Let the medium solidify and then use a tip or toothpick to remove a ca 5 mm wide strip of the medium, this will give space for the areal part of seedlings. For RoPod with arcs (5, v24 etc.) make sure arcs are not covered by the medium.
 
  - **Step 4. Transfer seeds.**
Use a sterile toothpick to places seeds on the bottom glass by the edge of the medium. For RoPod 5 place the seeds “under” the arches, which are designed to guide young roots into the individual channels
 
   - **Step 5. Close the chamber.**
 RoPods with watertight lids do not need to be sealed individually, other RoPods require it. Place the chamber into a square Petri plate and seal it. 

 - **Step 6. Place the RoPod into a plant growth cabinet.**
Place the plate vertically under growth conditions. It is advisable to slightly tilt the chamber backwards to guide root growth along the bottom coverslip. Lids of some RoPod versions (e.g. v23.4, 23.4 etc) ensure such tilt <br/><br/>
</details>


<details><summary>How to print RoPods</summary> 
<br/> 
  
[<img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.applications/Screenshot%20for%20printing%20RoPods%20demo%20video.png?raw=true" width="500" title="Seed plating demo video">](https://www.youtube.com/watch?v=jWTp5Sgqe-Q&ab_channel=AlyonaMinina)

In this video you can find a short demo for RoPod chambers printing.
<br/>
<br/>
 
**For printing you will need:**
- access to an FDM 3D printer with a nozzle 0.4 mm
- clear PETG filament, ⌀ 1.75 mm. It is advisable to check the filament for toxicity. To our experience, clear PETG does not impact Arabidopsis growth.
- 24 x 60 mm microscopy coverslip #1.5, i.e. 0.16-0.19 mm thick ( VWR, 630-2108)
- superglue
- .3mf or .stl file for RoPods
 <br/>
 <br/>
 
 **Step 1. Generate the g-code:**

- Files required for printing are provided in the tables below
- Prior to printing, the models can be tunded using the provided Autodesk .3fd files 
- An example of recommended settings for printing each RoPod version is in the provided project file. 
- Make sure that the chamber and the lid are positioned with the rims looking upwards and the glass insertion layer closest to the print bed
- Print settings-> Layer height = 0.1 mm (if possible we recommend using variable layer height).  Variable layer height feature (available for Prusa printers) allows to use small layer height beneficial for efficient embedding of the glass into the print and a larger layer height for printing the rest of the structure. For an example see the provided Slic3r project files
- Print settings-> Fill density = 50%
- Print settings-> Fill pattern = 3D Honeycomb
- Print settings-> Layers and Perimeters-> Vertical shells-> Perimeters = 4
- Use of brim reduces warping and detachment of the first layers
- Slice the model and [insert a pause](https://help.prusa3d.com/article/insert-pause-or-custom-g-code-at-layer_120490) at the layer right before the layer with the slot for the glass
 - You can simultaneously print up to 17 RoPods on a Prusa MK2or MK3. However we strongly recommend to start with just one
 <br/>
 <br/>
 
  **Step 2. Clean the coverslip glasses:**
 - Remove dust and fat from the glasses by wiping them clean with a paper tissue soaked in acetone​
 <br/>
 <br/>
 
  **Step 3. Start the print:**
 - Start the print and wait until it automatically pauses on the layer programmed int the Step 1.
 - The extruder will move to the back left of the print bed while waiting for the user to resume the print
 <br/>
 <br/>
 
  **Step 4. Place the glasses into the slots:**
 - The chambers and lids models have ca 0.18mm deep slots for the coverslips
 - Add a small drop of super glue to two corners of a glass. This will secure the glass' position during printing
 - Use forceps and patience to carefully place the glass into its slot. Make sure it does not stick upwards or sideways
 - Press down on the the corners with glue and hold for a few seconds. sic! wear gloves! superglueing oneself to a 90C- hot print bed is not a good way to start your day
 

 <br/>
 <br/>
 
  **Step 5. Resume the print:**
 - Resume the print and make sure the the filament does not move the glass from its position and does not crack it
 - When the chamber is ready make sure there is no filament sticking sideways. If needed imperfections can be removed with a scalpel
 <br/>
 <br/>
</details>
<br/>

 ## RoPod.Hardware
Arabidopsis-optimized microscopy chambers for seedling growth and root imaging
<br/>
<br/>
**RoPods are plant-optimized chambers** with top and bottom made out of microscopy-grade glass. Plants are grown and imaged in the same chamber - no stress! RoPods with watertight design allow drug treatments and stress-free long-term time-lapse imaging at low and high magnifications. Separate lanes for individual roots enable easy tracking of the same biological replicate during experiments. 

Below you can find most used versions of RoPods optimized for a number of different applicaitons. We provide a brief description, object and project .3mf files for printing and Autodesk Fusion 360 3fd file to be used if fine-tuning of a model is needed.
<br/>
<br/>

 ### RoPod v23 
-	**Optimal for imaging roots of 3-6 days old Arabidopsis seedlings**
-	A single-well chamber, can accomodate up to 20 seedlings
-	Outer measurements 30 x 76 x 11 mm, compatible with standard inverted microscope stages
-	Chamber V = ca 6 ml
-	Designed for microscopy glass 24 x 60 x 0.17mm (#1.5) 
-	Glass is incorporated into the chamber and the lid during printing

|Version <img width="50"> |Preview<img width="400">|Files <img width="600"> |Comments<img width="300">|
| --- | --- | ---|---|
|**v23.4**|  <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v23/RoPod%2023.4%20preview.png?raw=true" width="400" title="RoPod23.4 preview"> <details><summary>Show more</summary> <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v23/RoPod%2023.4%20empty.png?raw=true" width="400" title="RoPod23.4 preview">  </details> |<details><summary>Model files</summary><br/> Individual model files:<br/>[RoPod v23.4 chamber.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v23/Chamber%20v23.4.3mf)<br/> [RoPod v23.4 lid.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v23/Lid%20v23.4.3mf)<br/><br/><br/> Slc3r project file:<br/>[RoPod v23.4 with adjustable layer height.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v23/RoPod%2023.4%20with%20adjustable%20height.3mf)<br/><br/> Autodesk Fusion 360 file: <br/> [RoPod v23.4.f3d](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v23/RoPod%20v23.4.f3d)</details><br/> <details><summary>Printing instructions</summary><br/> 1. Printing one chamber with a lid takes ca 2 h and ca 10 g of filament <br/><br/> 2. For general instructions see the information above ("How to print RoPods")</details> | The bottom edge of the lid is angled to slightly tilt the chamber for the optimal root growth along the bottom glass| 

<details><summary>Previous versions of the RoPod v23 </summary>
  
|Version <img width="50"> |Preview<img width="400">|Files <img width="500"> |Comments<img width="300">|
| --------- | --- | --- | --- |
| **v23.3** | --- | --- | --- |
| **v23.2** | --- | --- | --- |
| **v23.1** | --- | --- | --- |
  </details>
  <br/>
  <br/>
    
  ### RoPod v24 
-	**Optimal for imaging roots of 3-6 days old Arabidopsis seedlings**
-	A single-well chamber, can accomodate up to 11 seedlings
- Separators create lanes for individual root growth 
- An arc on the top of each lane guides young root growth in the desired direction
-	Outer measurements 30 x 76 x 11 mm, compatible with standard inverted microscope stages
-	Chamber V = ca 6 ml
-	Designed for microscopy glass 24 x 60 x 0.17mm (#1.5) 
-	Glass is incorporated into the chamber and the lid during printing

|Version <img width="50"> |Preview<img width="400">|Files <img width="600"> |Comments<img width="300">|
| --- | --- | ---|---|
|**v24.3**|  <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20preview.png?raw=true" width="400" title="RoPod24.3 preview"> <details><summary>Show more</summary> <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20empty%201.png?raw=true" width="400"> </br>  <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20empty%202.png?raw=true" width="400"> </br>  <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20with%20seedlings%201.png?raw=true" width="400"> </br>  <img src="https://github.com/AlyonaMinina/Files.for.RoPod.reps/blob/main/RoPod.v24/RoPod%2024.3%20with%20seedlings%202.png?raw=true" width="400"> </br>  </details> |<details><summary>Model files</summary><br/> Individual model files:<br/>[RoPod v24.3 chamber.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v24/Chamber%20v24.3.3mf)<br/> [RoPod v24.3 lid.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v24/Lid%20v24.3.3mf)<br/><br/><br/> Slc3r project file:<br/>[RoPod v24.3 with adjustable layer height.3mf](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v24/Chamber%20v24.3%20with%20variable%20layer%20height.3mf)<br/><br/> Autodesk Fusion 360 file: <br/> [RoPod v24.3.f3d](https://github.com/AlyonaMinina/Files.for.RoPod.reps/raw/main/RoPod.v24/RoPod%20v24.3.f3d)</details><br/> <details><summary>Printing instructions</summary><br/> 1. Printing one chamber with a lid takes ca 2 h and ca 10 g of filament <br/> <br/> 2. For general instructions see the information above ("How to print RoPods") </details> |The bottom edge of the lid is angled to slightly tilt the chamber for the optimal root growth along the bottom glass| 

<details><summary>Previous versions of the RoPod v24 </summary>
  
|Version <img width="50"> |Preview<img width="400">|Files <img width="500"> |Comments<img width="300">|
| --------- | --- | --- | --- |
| **v24.2** | --- | --- | --- |
| **v24.1** | --- | --- | --- |
  </details>
