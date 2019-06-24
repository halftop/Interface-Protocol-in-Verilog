# Type 'make' to run the sim and then view the results by running the
# command 'gtkwave gray_count.lxt'
#
# This runs the simulation using icarus verilog.  'yum install iverilog'
#

SOURCES=SPI_Master.v SPI_loopback.v SPI_loopback_tb.v SPI_Slave.v

tb: $(SOURCES)
	iverilog -o tb $(SOURCES)
	vvp tb 

clean:
	-rm -rf *~ *.vcd tb

wave:
	gtkwave *.vcd