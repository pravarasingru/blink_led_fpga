blink_led_fpga
TASK-1 of VSD FPGA Mini using Verilog, PCF file, and RGB LED.
Project Description
This project uses Verilog to blink an onboard RGB LED on the VSDSquadron FPGA Mini (FM) board using its internal oscillator and a frequency divider. The project includes a Verilog design, PCF file for pin mapping, and Makefile for build and flashing.

Files Included
- `top.v` – Verilog code for the LED blinking logic
- `VSDSquadronFM.pcf` – Pin mapping file
- `Makefile` – Automates build and flashing
- `Blink_LED_Report.docx` – Project report documentation

 Tools Used
- Yosys (for synthesis)
- nextpnr (for place-and-route)
- icepack, iceprog (for bitstream creation and flashing)

 How to Run
```bash
make clean      # optional: clean previous build
make build      # synthesize and place & route
sudo make flash # flash bitstream to FPGA
