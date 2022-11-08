# Websockets Setup

_**Private using.**_


## boost library installation

Instruction source: https://blog.csdn.net/wzwpy99/article/details/122542585

(1) download boost libraries

   https://www.boost.org/

(2) open "bootstrap.bat"

(3) run "b2.exe" as administrator



## Visual Studio

Make sure that truly adding the library path both for x86 and x64!!!

(4) add the path into "VC++ Catalogue" (both for x86 and x64!!!)

    1) "include catalogue" = ".../boots_1_7xx_0"
    
    2) "library catalogue" = ".../boots_1_7xx_0/stage/lib"


## Linux Install Websockets

use 'apt search websockets' to find out the specific name of library!!!!

reference blog: https://blog.csdn.net/chile19/article/details/80520704


## Linux Multi-PC Communicate

Python Server, Python Client

reference blog: https://stackoverflow.com/questions/45944199/python-websockets-cant-connect-over-internet

Python Server: 

start_server = websockets.serve(handel, host = None, port = 8081)

(set host as 'None' to listen all possible IP address!!!!!!!!!)

Python Client:

async with websockets.connect('ws://172.31.13.230:8081') as websocket

(set the uri as server's IP address, such as 172.31.13.230)



<!-- 
Wen Fan -->

