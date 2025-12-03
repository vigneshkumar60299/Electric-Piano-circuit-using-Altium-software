# Electric-Piano-circuit-using-Altium-software
# Exp-10--Design-a- Electric Piano-circuit-using-Altium-software-and-generate-the-Gerber-file.
# AIM:
To design the schematic and PCB layout diagram of an Electric Piano circui circuit using Altium software.
# EQUIPMENT REQUIRED:
●	Hardware: Personal Computer (PC)<br>
●	Software: Altium  <br>
# PROCEDURE:
•  Open Altium & create a project<br>
File → New → Project → choose PCB Project. Give it a name and folder.<br>
•  Add a schematic sheet<br>
Right-click the project → Add New to Project → Schematic. Save it (e.g., project.SchDoc).<br>
•  Place components<br>
Use Components panel or Place → Part. Search library parts (resistors, ICs, connectors). Place each part and assign a designator (R1, C1, U1).<br>
•  Wire the circuit<br>
Use the Wire tool to connect pins. Add net labels for power (VCC, GND) and important signals. Keep wires neat.<br>
•  Annotate & check<br>
Tools → Annotation to give unique designators if needed. Run Electrical Rule Check (ERC) and fix any errors/warnings.<br>
•  Add PCB document<br>
Right-click project → Add New to Project → PCB. Save it (e.g., project.PcbDoc).<br>
•  Compile and update PCB <br>
On the schematic: Design → Compile Project. Then Design → Update PCB Document → Review ECO → Execute to push parts to PCB.<br>
•  Define board shape<br>
In PCB view: Design → Define Board Shape → Draw outline to the required size.<br>
•  Place components on board<br>
Move parts from the component list onto the board. Place connectors at the edge, group related parts, keep critical parts (crystals, sensors) positioned carefully.<br>
•  Set design rules<br>
PCB → Design Rules → set trace width, clearance, via sizes. For beginners, use default rules or teacher-provided values.<br>
•  Route tracks<br>
Use Interactive Routing (Route → Interactive Route) to connect pads. Route power traces wider (e.g., 1.5–2×). Use ratsnest to see remaining connections.<br>
•  Add ground/power planes (optional)<br>
Place a polygon pour for GND or VCC for better grounding: Place → Polygon Pour → set layer & net → Pour.<br>
•  Run Design Rule Check (DRC)<br>
PCB → Design → Rules Check (or Tools → Design Rule Check). Fix spacing, un-routed nets, or overlapping pads.<br>
•  Add silkscreen & labels<br>
On the Silkscreen layer, add component names, polarity marks, board name/version.<br>
•  3D check (optional)<br>
View → 3D Layout Mode to inspect component heights and mechanical fit.<br>
•  Prepare fabrication outputs<br>
File → Fabrication Outputs → Gerber Files (select layers: top/bottom copper, solder mask, silkscreen). Also generate NC Drill Files.<br>
•  Generate assembly files<br>
File → Assembly Outputs → Pick and Place (Centroid) and BOM (Bill of Materials).<br>
•  Verify outputs<br>
Open generated Gerbers in a Gerber viewer to confirm layers and drill map look correct.<br>
•  Create final archive<br>
Zip the project folder and all output files (Gerbers, Drill, BOM, Pick-and-Place). Add a Readme with board name and revision.<br>
•  Send to manufacturer<br>
Upload the zip to your PCB fab and follow their order steps.<br>
# THEORY:
Electric Piano Circuit 
The electric piano circuit works on the principle of generating musical notes electronically rather than mechanically. When a key is pressed, an electronic oscillator produces an audio frequency corresponding to a musical tone. In this circuit, the 555 timer IC is configured as an astable multivibrator, generating square-wave audio signals. The pitch or frequency of the sound depends on the resistance selected by each piano key. Therefore, each key creates a different frequency, resulting in different musical notes.
Circuit Construction and Components
The circuit mainly consists of the NE555 timer IC, a series of resistors, push buttons (P1 to P6), a 100nF timing capacitor, a 10µF output coupling capacitor, and a small speaker. Six push buttons are connected in series with individual resistors so that each button creates a unique RC network when pressed. The 555 timer receives power from a 5–9V DC supply. The timing capacitor connected between pins 2/6 and ground controls the oscillation along with the resistor network from the push buttons. The output pin (pin 3) of the 555 is coupled to the speaker through a 10µF capacitor to deliver sound.
Working Principle
When the circuit is powered, the 555 remains inactive until a key is pressed. Pressing any push button (P1 to P6) inserts a resistor of a specific value into the RC circuit of the 555 timer. This changes the charging and discharging time of the timing capacitor, producing a unique oscillation frequency. Lower resistance results in higher frequency tones (high-pitch sound), while higher resistance produces lower frequency tones (low-pitch sound). The oscillating output from pin 3 of the 555 passes through the 10µF capacitor and drives the speaker, producing the corresponding musical note. When the key is released, the RC path breaks and the sound stops immediately.
This electric piano circuit is a simple and effective demonstration of electronic sound generation using the 555 timer. Different musical notes are obtained by selecting resistors through push buttons, making it a useful learning prototype for beginners in electronics and audio signal generation.
# CIRCUIT DIAGRAM:
 <img width="979" height="544" alt="image" src="https://github.com/user-attachments/assets/f3bb58ca-0fda-4cfa-803a-3dbb2ab54a68" />

 
# EXPECTED OUTPUT:
## Schematic diagram:
<img width="1002" height="515" alt="Screenshot 2025-11-28 205557" src="https://github.com/user-attachments/assets/2c469796-32ae-4a90-b9d2-cda766b5936d" />


## Layout diagram:
 <img width="1032" height="463" alt="image" src="https://github.com/user-attachments/assets/c74756f4-704a-42d1-9169-fe627b65ffdd" />

# RESULT:
Thus, the schematic and PCB layout for the Electric Piano circuit has been successfully designed using Altium software.

