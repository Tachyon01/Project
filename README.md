# Project
SCOAP analysis

Step1: Get the Json
Use Yosys http://www.clifford.at/yosys/ and enter following Commands
read_verilog myfiles.v

hierarchy -check -top mytop

proc; opt; fsm; opt; memory; opt

techmap; opt

write_json out.txt

  
Use filenames and topmodule name as required


Step2: Parse it, You may need to update name of top module, input file and Output file

Run Draft2.Py


Step3: Get SCOAP
Use https://sourceforge.net/projects/testabilitymeasurementtool/

Enter the input file and get output generated
