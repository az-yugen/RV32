# yugen RV32I Processor

A simple implementation of a 32-bit pipelined RISC-V processor on an FPGA, written in SystemVerilog.

<div align="center">
    <img width="400" alt="homepage" src="./imgs/fpga_yugen.png">
</div>


## Specifications
- RV32I: 32-bit base integer.
- classic 5-stage pipelined datapath
- Harvard memory organization
- Little-endian data format
- Memory-mapped on-board LED's UART and SPI I/O peripherals
- synthesized on Tang Nano 20k Gowin FPGA

<!--Organizational Structure -->



## Programs
Some programs written in RISC-V assembly and bare-metal C:

- nth Fibonacci calculator on on-board LED and terminal
- Mandelbrot set grapher in the terminal over UART
- listing prime numbers upto 10,000 over UART


<div align="center">
    <img width="350" alt="primes" src="./imgs/GIF_MANDELBROT.gif">
	<img width="350" alt="primes" src="./imgs/GIF_PRIMES.gif">
</div>



## Logisim

RV32IM variant simulation on logisim with some programs.

<div align="center">
    <img width="400" alt="logisim rv32im" src="./imgs/YUGEN_GIF.gif">
</div>

<div>
    <img width="200" alt="logisim primes" src="./imgs/PRIMES_GIF.gif">
    <img width="200" alt="logisim primes" src="./imgs/MANDELBROT_GIF.gif">
    <img width="200" alt="logisim primes" src="./imgs/PONG_GIF.gif">
</div>



## Resource Utilization

|     | Total  | Used  | %   |
| --- | ------ | ----- | --- |
| LUT | 20,736 | 1,721 | 8   |
| FF  | 15,750 | 481   | 4   |
| BSRAM | 46   | 46    | 100 |

<div>
    <img width="250" alt="resources" src="./imgs/resources.jpg">
</div>