# 7-Segment Display Counter using 8051 Microcontroller

This project demonstrates how to display digits from 0 to 9 on a 7-segment display using the 8051 microcontroller. Each digit is displayed with a delay in between.

## 🛠 Hardware Requirements

- 8051 Microcontroller (e.g., AT89C51 or similar)
- Common Cathode 7-Segment Display
- Resistors (330Ω for each segment)
- Power Supply (5V)
- Connecting Wires
- Breadboard or PCB
- Crystal Oscillator (11.0592 MHz recommended)
- Capacitors (33pF for crystal, 10µF for reset circuit)
- Keil uVision for simulation and code development
- Proteus (optional for simulation)

## 🧠 Working Principle

Each segment of a 7-segment display is connected to Port 2 of the 8051. A hexadecimal value is sent to Port 2 to display each digit. The code runs through digits 0–9 with a delay between each update.

The binary pattern for each digit is written in hexadecimal. For example:
- `0x3F` = 0 → segments a, b, c, d, e, f ON
- `0x06` = 1 → segments b, c ON

## 🧾 Hex Codes for Digits (Common Cathode)

| Digit | Hex Code | Binary     |
|-------|----------|------------|
| 0     | 0x3F     | 0011 1111  |
| 1     | 0x06     | 0000 0110  |
| 2     | 0x5B     | 0101 1011  |
| 3     | 0x4F     | 0100 1111  |
| 4     | 0x66     | 0110 0110  |
| 5     | 0x6D     | 0110 1101  |
| 6     | 0x7D     | 0111 1101  |
| 7     | 0x07     | 0000 0111  |
| 8     | 0x7F     | 0111 1111  |
| 9     | 0x67     | 0110 0111  |

## 📸 Project Media

![7_segment_display_output](https://github.com/user-attachments/assets/1a396c0f-4f51-4dc7-9958-8dce5d1e89e9)


## 🔄 Future Enhancements

- Loop the counter continuously using `while(1)` block.
- Add button-controlled increment/decrement.
- Interface multiple 7-segment displays for multi-digit output.

## 👨‍💻 Developed By

Vamsi T 
Graduate Engineer (ECE) 
vamsithummaluri@gmail.com 

---

## 🛠 License

This project is licensed under the MIT License - feel free to use and modify as needed.

