# Ben Eater 8-Bit Computer Replica

This repository contains all documentation, source code, schematics, and media related to our team's build of the [Ben Eater 8-bit computer](https://eater.net/8bit). The project is based on TTL logic and demonstrates the foundational principles of computer architecture, from logic gates and registers to control logic and instruction execution.

---

## 🔧 Project Scope

Our goal is to fully recreate Ben Eater's 8-bit computer from scratch using breadboards, 74LS series chips, and other discrete components. The project involves:

- ✅ Building core CPU components (registers, ALU, program counter, clock, etc.)
- ✅ Creating and flashing custom microcode and machine code using EEPROMs
- ✅ Developing a simple instruction set architecture (ISA)
- ✅ Assembling programs in machine code to run on the computer
- ✅ Documenting the entire build process with photos, diagrams, and explanations

---

## 📁 Repository Structure

-  Domucmentation
    --> skematics
    --> logical design
-  Eprom code
-  pictures
    --> individual modules
    --> general pictures
    --> demo video

---

## 🧠 Instruction Set Architecture (ISA)

Our machine supports a minimal instruction set, similar to Ben's, including:

- `LDA` – Load A register
- `ADD` – Add to A register
- `OUT` – Output to bus
- `HLT` – Halt execution

(See `docs/instruction-set.md` for the full list and details.)

---

## 💾 EEPROM Programming

We are using the AT28C256 EEPROMs. The EEPROM code in `eprom-code/` includes:

- `microcode.bin` – EEPROM contents defining control signals for each instruction cycle
- `program1.bin` – Example program to perform addition and output result
- Assembly source files used to generate the binaries

See [docs/programming.md](docs/programming.md) for instructions on how to write to the EEPROM using an Arduino or EEPROM programmer.

---

## 📷 Build Documentation

In the `images/` and `docs/` folders, we are keeping:

- Breadboard layouts and annotated schematics
- Step-by-step hardware assembly photos
- Notes about bugs, troubleshooting, and lessons learned

---

## ⚙️ Tools and Components

We are using the following:

- Breadboards, jumper wires, LEDs
- 74LS series logic chips (e.g. 74LS245, 74LS173, 74LS08, 74LS138, etc.)
- AT28C256 EEPROMs
- Arduino Uno for EEPROM programming
- Ben Eater's clock module (or a custom version)
- Optional: oscilloscope or logic analyzer

---

## 📚 References

- [Ben Eater’s 8-bit computer series](https://eater.net/8bit)
- [Ben Eater's GitHub](https://github.com/beneater)
- [Datasheets for 74LS series chips](http://www.ti.com/)
- [EEPROM Programmer Guide](https://github.com/dmadison/AT28C-Programmer)

---

## 🤝 Contributing

This is a group project for educational purposes. If you'd like to contribute improvements, fixes, or additional programs, feel free to fork and make a pull request — or just raise an issue to suggest an idea!

---

## 📜 License

This project is open source and educational. Schematics and code are available under the MIT License. See `LICENSE` for more.

