# Smart-Bank-Locker-with-RFID-using-LPC2129
Smart Bank Locking System Using RFID and Password Authentication

📌 Project Overview

The Smart Bank Locking System Using RFID and Password Authentication is an embedded security project designed to provide two-level authentication for bank lockers and other restricted areas.

The system uses an RFID card and a password to verify the user's identity. First, the RFID reader scans the card and sends its ID to the microcontroller. If the card is authorized, the user is asked to enter a four-digit password using a 4×4 keypad.

The locker is unlocked only when both the RFID card and password are valid. If an incorrect password is entered three times, the system activates an LED and buzzer as an alert.

🎯 Objectives

- To develop a two-level authentication security system.
- To provide access using RFID and password verification.
- To prevent unauthorized access.
- To generate an alert after multiple incorrect password attempts.
- To control a locking mechanism using an embedded microcontroller.

🛠️ Hardware Components

- LPC2129 ARM7 Microcontroller
- EM-18 RFID Reader (125 kHz)
- RFID Card
- 4×4 Matrix Keypad
- 16×2 LCD Display
- DC Motor
- Motor Driver
- LED
- Buzzer
- Power Supply

💻 Software Requirements

- Embedded C
- Keil µVision IDE
- Flash Magic
- LPC2129 Microcontroller
- UART Communication

⚙️ Working Principle

1. The system initializes the LCD display and UART communication.
2. The EM-18 RFID reader scans the RFID card.
3. The RFID reader sends the card ID to the LPC2129 microcontroller through UART.
4. The microcontroller compares the received ID with the authorized RFID ID.
5. If the card is valid, the LCD asks the user to enter a four-digit password.
6. The password is entered using the 4×4 matrix keypad.
7. The microcontroller checks the entered password.
8. If both authentication steps are successful, access is granted and the motor operates to unlock the system.
9. If the password is incorrect three times, the system activates the LED and buzzer to indicate unauthorized access.
10. If the RFID card is invalid, the LCD displays an invalid card message.

🔌 Communication Protocol

RFID Communication: The EM-18 reader uses radio frequency to identify the RFID card.

UART Communication: The EM-18 reader sends the decoded RFID card ID to the LPC2129 microcontroller through UART serial communication.

🔐 Security Features

- Two-level authentication.
- Authorized RFID card verification.
- Four-digit password protection.
- Three incorrect password attempts trigger an alert.
- LED and buzzer indication for unauthorized access.

🏢 Applications

- Bank locker security systems.
- Home security systems.
- Office access control.
- Jewellery showroom security.
- Restricted-area access control.
- Industrial security systems.

📂 Project Structure

Smart-Bank-Locking-System/
│
├── main.c
├── keypad.h
├── lcd_header.h
└── README.md

🚀 Future Enhancements

- Add GSM notifications for unauthorized access.
- Store multiple authorized RFID card IDs.
- Add password modification functionality.
- Integrate IoT-based remote monitoring.
- Add a mobile application for access monitoring.

👨‍💻 Project Domain

Embedded Systems | ARM7 | Embedded C | RFID | UART | Microcontroller Interfacing

---

Note: This project is a prototype for demonstrating RFID-based and password-based access control. Additional security measures would be required for deployment in a real bank locker system.
