# lipo_singlecell-charger
This project is an attempt to Create a single cell LiPo battery charger by modelling a buck converter and a CC-CV control system totally analog without using any black box ICs. 
The key application of this project is to shocase the working behind the working of a CC-CV mode charging (Mobile chargers,EV charging etc).
The Nominal voltage of the LiPo battery is 3.7V while a safe to assume fully charged state is 4.15V. so the buck converter must be capable of taking a wide range of volage and converting it into 3.2 to 4.15 volts. 
The contorl system for the CC-CV mode is going to be implemented using OP-Amps as main components.
  Control system sub-circuits:
          -Reference voltages for voltage and current of the buck output.
          -Triangle Wave generator (for PWM)
          -Differential Amplifier,Comparator for PWM from triangle wave.
          -Mosfet driver(depending on the input voltage range taken into account)
  The project aims to bring these into a Single PCB starting with designing and validating the circuits in Ltspice and later using Kicad for schematic and PCB layout.
