# Timer
A simple timer for FPGA
<br><br>
Time can be set within a range from 00:00 to 59:59. One button sets seconds, the other one sets minutes. Toggle button switches between set and countdown mode.
<br><br>
The project consists of four blocks:<br>
1. Clock divider. A block that divides the input frequency of 50MHz to get 2Hz and 1Hz.
2. Mux. A block that really is a multiplexer responsible for choosing which clock frequency to pass to the timer block (depending on current mode – set or countdown).<br>
3. Timer. A block used for processing the flow of time in countdown mode and setting time in set mode.<br>
4. BCDto7SEGconverter. A four-input-and-four-output block that converts the BCD numbers processed in timer block to seven-segment display numbers.
<br><br>
A university project made in collaboration with <a href="https://github.com/suchydariusz/">Dariusz Suchy</a>
