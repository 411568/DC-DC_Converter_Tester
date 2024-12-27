# Modular Device for Measuring DC/DC Converter Parameters

The DC/DC converter tester is a device built for an engineering project at AGH University in Cracow. 
It consists of three modules: 
* Controller board
* Regulated power supply
* Active load

## Working principle

![Menu diagram](/Dokumentacja_projektu/Engineering_project/images/schemat_blokowy.png)

The device can automatically measure the efficiency and output regulation of any connected DC converter (DUT).
It first sets the DUT input voltage by adjusting the power supply. Then it measures the converter output voltage.
Afterwards, it steps the output current and calculates efficiency and output voltage drop for each measurement.

It displays the data in the form of a graph on the display. You can also write them onto an SD card or send to PC via
USB or RS485 interface. 



## Controller board
![Controller board PCB](/Dokumentacja_projektu/Engineering_project/images/controller_PCB.jpg)

Controller board is designed around a STM32F401 microcontroller. It has an interface for LCD with SSD1963 controller, 
inputs for buttons and encoder, three RS485 outputs for controlling submodules, thermocouple interface (K type) and a fan driver.


## Power supply board

![Power supply board PCB](/Dokumentacja_projektu/Engineering_project/images/converter_PCB.jpg)

Power supply board is based on a buck converter - MP9928. It can deliver up to 20V at 3A. The output current 
is controlled by the STM32F3 microcontroller. The output current is measured by INA219 and voltage can be sensed using the internal ADC.

## Active load board

![Active load board PCB](/Dokumentacja_projektu/Engineering_project/images/dc_load_PCB.jpg)

Active load module works using the principle of a current source. It consists of a single power mosfet with op-amp controlled
feedback. The output current can be set in the range of 0 to 3A using the microcontroller's DAC. The power mosfet is being cooled
down by an LGA1700 cpu radiator.



## Documentation and project files

The files are split into a few folders. In this repository there are two submodules, namely Firmware and Hardware. 
The firmware contains three STM32CubeIDE projects.  The hardware submodule is made up of five Altium Designer projects.

Folder "Dokumentacja_projektu" contains all the required datasheets and the engineering project thesis, that documents the whole project.
"Materialy" contains a number of images and measurements of the device.



### Autor
Krzysztof Sikora

2024
