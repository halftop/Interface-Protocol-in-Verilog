# Verilog UART Readme

For more information in Chinese and advice: https://halftop.github.io/post/Verilog-Uart

## Introduction

This is a basic UART that support optional parity,settable baud and data width,written in Verilog with testbenches.

### Source Files

```
\---general_uart
    |   README.md
    |   
    +---rtl
    |       rx_clk_gen.v	:	UART receiver_sample_clk implementation
    |       tx_clk_gen.v	:	UART transmitter_baud_rate_clk implementation
    |       uart_frame_rx.v	:	UART receiver implementation
    |       uart_frame_tx.v	:	UART transmitter implementation
    |       
    \---tb
            uart_frame_tx_tb.v	:	testbench for uart_rx
            uart_loop.v	:	Wrapper for all to test,it’s a source file
            uart_loop_tb.v	:	testbench for uart_loop
```