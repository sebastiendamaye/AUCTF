# Pretty Ridiculous (50)

## Instructions

Eve discovered that a piece of paper had been shoved into her pocket.. what could it be? The message she found can be downloaded at the following link:

(n,e) = (627585038806247, 65537)

https://drive.google.com/file/d/17z7C5i_TOx_838QNPbZvNCKW4DcPCaEF/view?usp=sharing

Author: c

## Solution

Let's use RsaCtfTool to solve this:

~~~
(RsaCtfTool) $ n=627585038806247
(RsaCtfTool) $ e=65537
(RsaCtfTool) $ msg="145213650433152, 4562349440334, 24272724667960, 598242834066721, 89584939111364, 426756492371444, 511701778613016, 551732685650248, 296367799892003, 63113462897284, 198510931603899, 321201931522255, 401044612595398, 542697603423052, 213898535689643, 275839755798105, 185841409622217, 551732685650248, 121188708737752, 401044612595398, 512808963720303, 275839755798105, 198510931603899, 275839755798105, 401044612595398, 174484844253615, 551732685650248, 174486913717420, 575163265381617, 213898535689643, 401044612595398, 49103824223436, 551732685650248, 401044612595398, 598242834066721, 202722428784490, 306606077829794, 53801100921263, 401044612595398, 184805755675232, 405971446461049, 296367799892003, 275839755798105, 275839755798105, 401044612595398, 358054299396778, 4562349440334, 320837325468842, 401044612595398, 202722428784490, 551732685650248, 321201931522255, 228350651363859"
(RsaCtfTool) unknown@localhost:/data/src/RsaCtfTool$ for i in $(echo $msg | sed "s/,//g");do ./RsaCtfTool.py -n $n -e $e --uncipher $i;done
[+] Clear text : b'\x00\x00\x00\x00\x00\x00a'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00u'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00c'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00t'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00f'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00{'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00R'
[+] Clear text : b'\x00\x00\x00\x00\x00\x003'
[+] Clear text : b'\x00\x00\x00\x00\x00\x004'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00l'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00L'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00y'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00P'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00r'
[+] Clear text : b'\x00\x00\x00\x00\x00\x001'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00M'
[+] Clear text : b'\x00\x00\x00\x00\x00\x003'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00s'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00w'
[+] Clear text : b'\x00\x00\x00\x00\x00\x001'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00L'
[+] Clear text : b'\x00\x00\x00\x00\x00\x001'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00n'
[+] Clear text : b'\x00\x00\x00\x00\x00\x003'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00v'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00E'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00r'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00b'
[+] Clear text : b'\x00\x00\x00\x00\x00\x003'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00t'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00h'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00I'
[+] Clear text : b'\x00\x00\x00\x00\x00\x005'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00S'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00m'
[+] Clear text : b'\x00\x00\x00\x00\x00\x004'
[+] Clear text : b'\x00\x00\x00\x00\x00\x001'
[+] Clear text : b'\x00\x00\x00\x00\x00\x001'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00B'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00u'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00T'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00_'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00h'
[+] Clear text : b'\x00\x00\x00\x00\x00\x003'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00y'
[+] Clear text : b'\x00\x00\x00\x00\x00\x00}'
~~~

## Flag
~~~
auctf{R34lLy_Pr1M3s_w1L1_n3vEr_b3_thI5_Sm411_BuT_h3y}
~~~
