# EVM-LPC1768
# Electronic Voting Machine (EVM) using LPC1768

This project is a secure and interactive *Electronic Voting Machine (EVM)* implemented using the *LPC1768 ARM Cortex-M3* microcontroller. Developed during my *SSIT Summer Internship*, it demonstrates the real-world application of embedded systems in designing reliable and user-friendly voting solutions.

## Features

- *Three voting inputs* for candidates A, B, and C via GPIO buttons.
- *Admin-controlled voting sessions* using separate enable and result buttons.
- *LCD (16x2)* display for user instructions and vote confirmation.
- *LED indicators and buzzer* to give visual and audio confirmation of votes.
- *One vote per session* logic to prevent multiple voting.
- *UART communication* for real-time result display on a connected PC.
- *Software debouncing* using Timer0.

## Components Used

- LPC1768 Microcontroller
- Push Buttons (5 total)
- LEDs (3)
- Buzzer
- 16x2 LCD (4-bit mode)
- UART to USB Module
- Power Supply (3.3V)

## Project Structure
## How It Works

1. Admin presses the *Enable button* to unlock voting mode.
2. Voter presses one of three *candidate buttons* to vote.
3. System:
   - Confirms vote with *LED + buzzer*
   - Displays message on LCD
   - Logs data to PC via UART
4. System *locks voting* until admin re-enables.
5. Admin can press the *Result button* at any time to view total votes via UART.

## Output Example (UART)
