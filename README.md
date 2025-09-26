Designed and built a solar panel-powered constant current charger for NiMH batteries and an iPhone, 
with the batteries functioning as a power bank or used in other devices.

Sketched the design concept, with transistors acting as current sources and buck converters regulating PV voltage. 
Researched the iPhone charging handshake protocol, modified the circuit in NI Multisim to correct functionality, and integrated it onto a 2-layer PCB using KiCad.

The charger delivered 5 W to the iPhone and approximately 4 W to five AA NiMH batteries in series. 
Once fully charged, the auto-cutoff reduced the charging current by 58.33% to below 0.1C. I
n theory, the batteries could also charge an iPhone 12 Pro Max up to three times without the solar panels.

Note: The descriptions are below their corresponding images.

![sketchIdea](https://github.com/user-attachments/assets/a798d90c-eaf5-4b76-b7a3-2d167c629f24)

<img width="452" height="310" alt="KiCadSchematic" src="https://github.com/user-attachments/assets/27abac9c-3c68-4ecf-8c56-6b1fb8303408" />

<img width="452" height="338" alt="solarChargerPCB_diagramPic" src="https://github.com/user-attachments/assets/0beba35f-348f-4680-a6ce-3043729a4e4e" />

The PCB size could be reduced significantly by using smaller switches and diodes, 
switching to surface-mount devices, and removing test components such as screw connectors. 
I did not use surface-mount devices because my inexpensive soldering kit could not solder them precisely.


<img width="452" height="103" alt="KiCadPic" src="https://github.com/user-attachments/assets/3de56da4-e0ac-41f8-99d5-0ff58d4aa47c" />

<img width="452" height="96" alt="KiCadPic3D" src="https://github.com/user-attachments/assets/f6273008-9e21-4305-918d-26eba389186c" />

![breadboardTest_iPhone](https://github.com/user-attachments/assets/f18b6622-74e6-42cb-978d-7142cfd17847)

If you look closely, you can see the iPhone lightning symbol, which indicates charging. 
The power adapter could not give more than 0.53 A in the breadboard testing.

<img width="940" height="599" alt="image" src="https://github.com/user-attachments/assets/356b1c90-31ff-46f3-bd56-34be84826407" />

The graph above is the data gathered from testing the breadboard prototype on charging NiMH battery.
It indicates auto-cutoff at 7.25 V or 1.45 V each.

![NiMHBatteryCharging](https://github.com/user-attachments/assets/77f162cd-4f6b-4a62-8642-5ab6176955d2)

0.48 A is the charging current of the NiMH battery.

<img width="452" height="239" alt="NiMHChargeGraph" src="https://github.com/user-attachments/assets/34b08b46-f177-4980-bd69-2e78b5c5fa1b" />

The graph above is the data gathered from testing the PCB prototype on charging NiMH battery. 
It indicates auto-cutoff at 7.33 V or 1.466 V each.

![iPhone5WCharg](https://github.com/user-attachments/assets/f9acb1dd-e3b3-4317-9361-545f94991015)

<img width="452" height="269" alt="iPhoneChargeGraph1" src="https://github.com/user-attachments/assets/9ec02643-34d9-4bdd-be50-32ae7d992c6a" />
