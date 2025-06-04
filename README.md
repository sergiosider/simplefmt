
# simplefmt
  
A very simple data formatter.
I use the SAELIG simple 8 channel analyzer, and it's a very simple 
and wonderfull tool.
I need it to check 4 serial links (modems, microcontrollers) in one design.
The problem is I need to format non-printable characters to hex, and avoid letting other
control codes to mess with the terminal, so this program:

converts \r to "[0D]\n",
converts \n to "[0A]\n",
converts " " (space) to iso-8859 \xb7 (a single and small "dot" centered (so i can check where a space was sent by the modem
converts everything from 0..31 and 127..255 to the hex representation [xx]
and let all printable characters go

