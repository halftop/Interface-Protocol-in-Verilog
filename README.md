# Interface Protocol in Verilog Readme

- General Uart:For more information in Chinese and advice: https://halftop.github.io/post/Verilog-Uart

- General SPI:For more information in Chinese and advice: https://halftop.github.io/post/Verilog_SPI

## Introduction

This is a repository that contains some Interface_Protocols written in Verilog.

There is a basic UART that support optional parity,settable baud and data width,written in Verilog with testbenches.

There is a basic SPI(Master and Slave) with settable frequence,data width and SPI mode,written in Verilog with testbenches.

### Source Files

```
\---Interface-Protocol-in-Verilog
    │  README.md
    │  
    ├─general_SPI
    │  ├─rtl
    │  │      SPI_Master.v  :   SPI_Master implementation
    │  │      SPI_Slave.v   :   SPI_Slave implementation
    │  │      
    │  └─tb
    │          SPI_Master_tb.v      :   testbench for SPI_Master
    │          SPI_loopback.v       :   Wrapper for all to test,it’s a source file
    │          SPI_loopback_tb.v    :   testbench for SPI_loopback
    │          SPI_loopback_tb.vcd  :   
    │          
    └─general_uart
        │  README.md
        │  
        ├─rtl
        │      rx_clk_gen.v     :	UART receiver_sample_clk implementation
        │      tx_clk_gen.v     :	UART transmitter_baud_rate_clk implementation
        │      uart_frame_rx.v  :	UART receiver implementation
        │      uart_frame_tx.v  :	UART transmitter implementation
        │      
        └─tb
                uart_frame_tx_tb.v	:	testbench for uart_rx
                uart_loop.v	:	Wrapper for all to test,it’s a source file
                uart_loop_tb.v	:	testbench for uart_loop
                uart_loop_tb.vcd
                 
    └─SCCB
        │  README.md
        │  
        └─rtl
                OV9650_SXGA_Config.mif
                OV_CAM.v
                OV_CAM_Capture.v
                OV_CAM_Ctrl.v
                OV_CAM_SCCB.v
```