
# Getting-started-with-ST-Microcontroller
A beginning guide for ST-Microcontroller

# Tools we use
- STM32CubeMX
- Keil MDK-ARM
- STM32CubeIDE

# Prepare the working environment
1. Download the STM32CubeMX from this [link](https://www.st.com/en/development-tools/stm32cubemx.html)
2. Download the Keil MDK-ARM from this [link](https://www2.keil.com/mdk5)

# Create your first project in STM32CubeMX
1. Open STM32CubeMX
2. In manage software installations, choose **install / remove**
3. In the pop out windows, click STM32F4 and install the 1.24.1 packages
4. Wait until the installation is done, then close the window
5. Click **ACCESS TO MCU SELECTOR** on the home screen
6. In Part number search, type in **STM32F427IIH**
7. Double click **STM32F427IIHx**, a MCU pin graph will show up
8. Reference to [RoboMaster Development Board User Guide](https://rm-static.djicdn.com/tem/RoboMaster%20Development%20Board%20Type%20A%20User%20Guide.pdf), Pin Out digram, PG1 is connect to one of the LED.
9. Find PG1 and left click it, set it as GPIO_Output
10. Click on **Project Manager** section, fill in project name, project location and change the toolchain to **MDK-ARM V5**
11. Click **GENERATE CODE**, when finished, click open project.
12. In **main.c** file, use **HAL_GPIO_TogglePin()** and **HAL_Delay()** to make LED blink once per second.
13. Build the project and Flash to Development Board, check if it is working as desire.
