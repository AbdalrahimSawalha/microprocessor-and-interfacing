# Microprocessor Interfacing System using 8085 🔧

---

## 1. Overview 📘

- This project presents a complete hardware interfacing system based on the Intel 8085 Microprocessor.

- The system integrates memory components and input/output devices using proper address decoding and control logic.

- The project demonstrates practical implementation of memory mapping, hardware interfacing, and bus control.

- All hardware connections, address allocation, and decoding logic were designed and verified using schematic diagrams and memory mapping analysis.

---

## 2. System Components 🧩

Microprocessor

- Intel 8085 Microprocessor

- Provides address bus, data bus, and control signals

Memory Units

- One 4K EPROM for program storage

- Two 4K RAM modules for data storage

- Memory chips connected using address decoding logic

Input Device

- DIP Switch

- Used to provide input data to the system

Output Device

- Seven Segment Display

- Used to display output data

Address Latching and Buffering

- SN74LS373 Address Latch

- Used to separate address and data from multiplexed bus

Address Decoding Components

- SN74LS138 Decoder

- 74HC154 Decoder

- SN74LS244 Buffer

- Used to generate chip select signals

---

## 3. Memory Map Design 🧠

- Memory map was designed starting from address 0000H.

- Each memory chip was assigned a unique address range.

- Address decoding logic ensures proper memory selection.

- Memory foldback was avoided by assigning non-overlapping address ranges.

Memory allocation includes:

- EPROM address range

- RAM 1 address range

- RAM 2 address range

- Address ranges defined using address lines A0–A15

---

## 4. Hardware Interfacing Design ⚙️

- Address bus A0–A15 used for memory selection

- Data bus used for data transfer between processor and devices

Control signals used include:

- RD# (Read)

- WR# (Write)

- ALE (Address Latch Enable)

- IO/M# (Memory or I/O select)

- Address latch separates multiplexed address/data bus

- Decoders generate chip select signals

- Buffers ensure signal stability

---

## 5. Address Decoding Logic 🔍

- Address lines connected to decoders

- Decoders generate unique chip select signals

- Each memory and I/O device activated only within its address range

- Prevents memory conflicts and ensures correct operation

---

## 6. System Operation 🔄

- Processor sends address through address bus

- Address latch captures lower address bits

- Decoder determines selected device

- Control signals initiate read or write operation

- Data transferred between processor and selected device

---

## 7. Project Files Structure 📁

Diagram

- Hardware schematic diagram

- Shows connections between processor and components

Memory Map

- Address allocation for EPROM and RAM

- Shows address ranges

Documentation

- Complete project design explanation

- Hardware implementation details

---

## 8. Technical Concepts Demonstrated 🧠

- Microprocessor architecture

- Memory interfacing

- Address decoding

- Bus organization

- Hardware interfacing

- Digital system design

---

## 9. Tools and Components 🛠️

- Intel 8085 Microprocessor

- EPROM and RAM chips

- Logic decoders and buffers

- Digital hardware schematic tools

---

## 10. Author 👨‍💻

Abdalrahim Sawalha

---

## 11. Course 

Microprocessor and Interfacing

---
