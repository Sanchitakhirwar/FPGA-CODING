module CPU(
  input clk,
  input reset,
  output [18;0] pc_out,
  output [18:0] mem_addr,
  input [18:0] mem_data_in,
  output reg[18:0] mem_data_out,
  output reg mem_read,
  output reg mem_write
  );
// define registers
reg [18:0] reg_file[0:7]; // r0 - r7
reg [18:0] pc;
reg [18:0] sp;
reg [18:0] ir; // instruction register
// ALU operations
reg [18:0] alu_result;
always @(posedge clk or posedge reset)
begin
if (reset) begin
pc<= 19'b0;
sp<= 19'h1FF; // initializing stack pointer
end else begin
// fetch-decode-execute pipeline stages
here
end
end
endmodule
