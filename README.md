This project implements a Smart House Monitoring System using the STM32 Nucleo-L476RG microcontroller. The system is designed to enhance basic home security and environmental control through a combination of sensor monitoring, user input via a keypad, and automatic actuation based on predefined conditions.

The system integrates a 4x4 keypad that allows the user to arm or disarm the security functions of the system. When armed, the system can trigger alarms or take action based on sensor readings—such as temperature thresholds or motion detection (if applicable).

A temperature sensor (e.g., LM35) continuously monitors ambient temperature, and a 3.3V fan, driven by a 2N2222 transistor, is activated automatically when the temperature exceeds a defined limit (e.g., 30°C). The fan turns off when the temperature drops below a lower threshold (e.g., 28°C), ensuring energy efficiency through hysteresis.

Feedback is provided through an HD44780 1602 LCD display, which shows the current temperature and system status (e.g., “System Armed”, “Fan ON”, or “Disarmed”). Additionally, UART communication via PuTTY is used for debugging and monitoring, allowing real-time data transmission to a connected PC.
Key Features:

    Temperature Monitoring using ADC on STM32

    Fan Control using transistor and PWM logic

    Keypad Interface for security system arming/disarming

    LCD Display for real-time system feedback

    UART Communication with PC terminal (PuTTY)

    Efficient Power Usage with threshold-based control logic

Applications:

    Basic home security and environmental control

    Low-cost smart home prototyping

    Embedded systems and microcontroller education
