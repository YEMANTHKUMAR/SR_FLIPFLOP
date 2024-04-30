# SR_FLIPFLOP
![image](https://github.com/RESMIRNAIR/SR_FLIPFLOP/assets/154305926/c17acfa3-84d9-4ef6-99ab-d36655169f63)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/SR_FLIPFLOP/assets/154305926/51cb1738-6112-466e-a1b0-f9dd9f2e9d25)
# Truth Table
![image](https://github.com/RESMIRNAIR/SR_FLIPFLOP/assets/154305926/0946849a-bd0a-445b-b27e-0833dee20e51)

VERILOG CODE
```````````````````````````````````````````````````````````````````````````````````
module sr_ff(clk,q,rst,s,r);
input s,r,clk,rst;
output reg q;
always@(posedge clk)
begin
if(rst==1)
q=1'b0;
else
begin
case({s,r})
2'b00:q=q;
2'b01:q=1'b0;
2'b10:q=1'b1;
2'b11:q=1'bx;
endcase
end
end

```````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````````
OUTPUT



![image](https://github.com/YEMANTHKUMAR/SR_FLIPFLOP/assets/160569469/3ecd712f-39dc-4f09-91ad-8efb9c16a2ec)
