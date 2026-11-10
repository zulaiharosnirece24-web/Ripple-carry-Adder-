module rca(s,carry,a,b,c);
input [7:0]a,b;
input c;
output [7:0]s;
output carry;
wire w1,w2,w3,w4,w5,w6,w7;
adder adder1(s[0],w1,a[0],b[0],1'b0);
adder adder2(s[1],w2,a[1],b[1],w1);
adder adder3(s[2],w3,a[2],b[2],w2);
adder adder4(s[3],w4,a[3],b[3],w3);
adder adder5(s[4],w5,a[4],b[4],w4);
adder adder6(s[5],w6,a[5],b[5],w5);
adder adder7(s[6],w7,a[6],b[6],w6);
adder adder8(s[7],carry,a[7],b[7],w7);
endmodule

module adder(sum,carry,a,b,c);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=(a&b)|(b&c)|(c&a);
endmodule
