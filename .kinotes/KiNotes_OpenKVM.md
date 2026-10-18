# **OpenKVM - Design Notes**

## **Overview**
OpenKVM - X01

## **Schematic Notes**
- HDMI MUX
- EDID Emulation

## **Layout Considerations**
<!-- Layer stackup, impedance, keep-outs -->

## **Component Notes**
<!-- Click on designators like **R1**, **C5**, **U3** to highlight on PCB -->
- **U1**
- **U3**
VCC = 2.6V to 4.**5V**
HPD Pull-Down Resistor should be 100k Ohm and placed on the source side HPD line.
Pull-up Resistors to 5V must be placed on the source side DDC clock and data lines. (2k Ohm to 5V)
AC Coupling Capacitors in 75nF - 200nF range must be placed on the MathLink (ML) and AUX Lanes. DisplayPort
AUX+ Line must be pulled-down weakly through a resistor to ground.
AUX- Line must be pulled-up weakly through a resistor to VCC.
- **U6**
VOL of 5V_uC_I2C1_SCL and 5V_uC_I2C1_SDA must be below 0.45V for proper operation. 
## **Power Distribution**
<!-- Power rails, decoupling strategy -->
- **+3V3**
- **5V**
## **Signal Integrity**
<!-- Critical nets, routing constraints -->
- **HDMI_1_CK+**
- 
## **References**
<!-- Datasheets, application notes, calculations -->

---
*KiNotes - PCBtools.xyz*

