`timescale 1ns / 1ps


module tb_edge_detector();
reg clk, reset, data_in;
wire edge_out;
always #5 clk = ~clk;
initial
begin
clk = 0;
reset = 1;
data_in = 0;
#4;
#20 reset = 0;
#30 data_in = 1;
#40 data_in = 0;
#30 data_in = 1;
#40 data_in = 0;
#30 data_in = 1;
#40 data_in = 0;
#30 data_in = 1;
#40 data_in = 0;
end
edge_detector dut(
.clk(clk),
.reset(reset),
.data_in(data_in),
.edge_out(edge_out));

endmodule
