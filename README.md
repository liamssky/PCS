# PCS
Power Conversion System for the Midnight Sun Solar Rayce Car

## Requirements
- The power conversion system must step-down voltage from the 90-154V Li-Ion pack to 12V for the low voltage systems in the electric vehicle.
- For safety, these two voltage domains must be isolated.
- It must be able to support greater than 60W continuous power output.
- It must be more efficienct than the Vicor DCM3623TA5N17B4T70 used previously (70%).

## Design Overview 
The design uses an Innoswitch 4 and ClampZero IC to control a DC-DC flyback converter. The ClampZero employes an active clamp to store the leakage inductance energy in a capacitor which can be recycled later in the switching cycle. The Innoswitch 4 drives the switching MOSFET and achieves zero-voltage-switching by forcing the voltage across the primary switch to zero before beginning a cycle. This results in a higher efficiency flyback converter. 

## Schematic 
![PCS-SCH-1](https://github.com/liamssky/PCS/blob/main/PCS-SCH-1.png)

## PCB layout
![PCS-Layout-1](https://github.com/liamssky/PCS/blob/main/PCS-Layout-1.png)

## 3D Model
![PCS-3D-Front](https://github.com/liamssky/PCS/blob/main/PCS-3D-Front.png)
![PCS-3D-Back](https://github.com/liamssky/PCS/blob/main/PCS-3D-Back.png)

## Transformer

