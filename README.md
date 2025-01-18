<p align="center"><img src="https://socialify.git.ci/411568/DC-DC_Converter_Tester/image?custom_description=Device+for+measuring+output+regulation+and+efficiency+of+DC+converters.&description=1&font=Source+Code+Pro&language=1&name=1&pattern=Circuit+Board&theme=Dark" alt="DC-DC_Converter_Tester" width="640" height="320" /></p>

<h2>🧐 Features</h2>


![Project photo](/Dokumentacja_projektu/Engineering_project/images/zdjecie_kompletne.jpg)

Here're some of the project's best features:

*  Allows measurement of output regulation and efficiency of DC/DC converters.
*  Integrates the controler, dc power supply and an active load.
*  Can act as a simple voltage source or an active load, just like your typical lab equipment.
*  Does not need any external software to function.
*  Integrates USB type B and RS485 interfaces for communicating with the PC, as well as a SD card slot.
*  Big 7" display and physical buttons for eas of control.
*  Modular and expandable - can be anything you want it to be!

<h2>🔧 How does it work?</h2>

![Menu diagram](/Dokumentacja_projektu/Engineering_project/images/schemat_blokowy.png)

The block diagram shown here shows all the main components making up the DC Converter Tester. 

The device can automatically measure the efficiency and output regulation of any connected DC converter (DUT).
It first sets the DUT input voltage by adjusting the power supply. Then it measures the converter output voltage.
Afterwards, it steps the output current and calculates efficiency and output voltage drop for each measurement.

It displays the data in the form of a graph on the display. You can also write them onto an SD card or send to PC via
USB or RS485 interface. 


<h2>💾 Electronic modules</h2>

<h3> Controller board </h3>

![Controller board PCB](/Dokumentacja_projektu/Engineering_project/images/controller_PCB.jpg)

Controller board is designed around a STM32F401 microcontroller. It has an interface for LCD with SSD1963 controller, 
inputs for buttons and encoder, three RS485 outputs for controlling submodules, thermocouple interface (K type) and a fan driver.


<h3> Power supply board </h3>

![Power supply board PCB](/Dokumentacja_projektu/Engineering_project/images/converter_PCB.jpg)

Power supply board is based on a buck converter - MP9928. It can deliver up to 20V at 3A. The output current 
is controlled by the STM32F3 microcontroller. The output current is measured by INA219 and voltage can be sensed using the internal ADC.

<h3> Active load board </h3>

![Active load board PCB](/Dokumentacja_projektu/Engineering_project/images/dc_load_PCB.jpg)

Active load module works using the principle of a current source. It consists of a single power mosfet with op-amp controlled
feedback. The output current can be set in the range of 0 to 3A using the microcontroller's DAC. The power mosfet is being cooled
down by an LGA1700 cpu radiator.


<h2>💻 Built with</h2>

Technologies used in the project:

*  STM32F401 and STM32F303 microcontrollers
*  MAX3485 for RS485 communication
*  MP9928 DC converter IC
*  OPA237 opamps
*  MAX6675 temperature sensor
*  INA219 sensor for reading output/input current and voltages
*  And many more!  

<h2>📖 Documentation and project files </h2>

The files are split into a few folders. In this repository there are two submodules, namely Firmware and Hardware. 
The firmware contains three STM32CubeIDE projects.  The hardware submodule is made up of five Altium Designer projects.

Folder "Dokumentacja_projektu" contains all the required datasheets and the engineering project thesis, that documents the whole project.
"Materialy" contains a number of images and measurements of the device.


<h2>🛡️ License:</h2>

This project is licensed under the MIT License.


<h2> 🙋‍♂️Authors </h2>

- Krzysztof Sikora

<h2>💖Like my work?</h2>

If you have any questions about the project feel free to contact us via email: krzysieksikora717@gmail.com