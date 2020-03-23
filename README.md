# SmartParks Rhino Tracker
<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/irnas_logo.png" height="100">

Device is composed from 3 different PCBs thah are stacked in to box like shape.

Stackup of PCBs is in this order:
- GPS (Top PCB)					Size: 28mm x 20mm 
- MCU (Side PCB)				Size: 28mm x 20mm (After final assembly)
- LORA ANTENNA (Side PCB)		Size: 28mm x 15.5mm
- BATTERY (Between side PCBs)

PCB specifications:
- 0.8mm PCB thinknes
- 0.152mm (6mil) trace to trace and trace to polygon clearance
- 0.75mm RF line thinknes

Connections between PCBs:
- MCU -> GPS - Solder pads on each PCB
- MCU -> LORA antenna - Coaxial cable

Assebled view
 
<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_6.png" height="200">			<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_7.png" height="200">			

Exploded view
 
<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_8.png" height="200">			<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_9.png" height="200">

Future changes:
- GPS
	- Reposition of GPS antenna to the center of the PCB
	- Better power supply for GPS (Lower working voltage)
	- Improve GND polygon for better GPS antenna performance	
	
		<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_10.png" height="200">			<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_11.png" height="200">	

- MCU
	- Optimize track path for antenna
	- Change PCB orientation in final assembly like so that MCU is under battery
	- Optimize hardware for battery voltage measure
	- Move REED switch closer to the MCU
	
		<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_12.png" height="200">
		
- LORA ANTENNA
	- Component value optimization for better antenna performance
 	
		<img src="https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/11_DOC/Rhino_V2_1_13.png" height="200">

- Mehanical Specification:
	- Device dimensions 32x24x27mm
	- Device weight: ~30g
	- Device is put in polyurethane resin to protect it (https://si.farnell.com/electrolube/ur5640rp250g/resin-pur-packet-250g-transparent/dp/2786027)
	- Inside of the device and around the battery there is pa peace of plastic for:
		- Keeping the gap between battery na LORA antenna eqalu on all devices assebled
		- Preventing the resin to go under the MCU metal case (There was a problem with RF radio when resin came under matel case of MCU)
		- Preventing the resin to go under GPS BGA chip (There was a problem when resin came under BGA and coused cold solder joints)
	- Resin thinknes arount the device is 2mm	
 
  
Currently under development, for all information see the [schematic PDF file](https://github.com/IRNAS/smartparks-rhino-tracker-hardware/blob/master/10_OUTPUT_FILES/).Produced board versions can be found in the [release section](https://github.com/IRNAS/smartparks-rhino-tracker-hardware/releases) of the repository.

**Latest release: [v2.5](https://github.com/IRNAS/smartparks-rhino-tracker-hardware)**


All comments and suggestions can be added to the [Issues]() section of the repo. For additional details see the [Issue]() section.

---

## Licensing

Rhino tracker hardware with documentation is licensed under [CERN OHL v.1.2. license](https://www.ohwr.org/licenses/cern-ohl/license_versions/v1.2).

What this means is that you can use this hardware and documentation without paying a royalty and knowing that you'll be able to use your version forever. You are also free to make changes but if you share these changes then you have to do so on the same conditions that you enjoy.

IRNAS is name and mark of Institute IRNAS Rače. You may use these name and terms only to attribute the appropriate entity as required by the Open Licence referred to above. You may not use them in any other way and in particular you may not use them to imply endorsement or authorization of any hardware that you design, make or sell.
*