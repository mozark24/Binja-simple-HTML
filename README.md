# Binja-simple-HTML
1. Load Binary Ninja
2. Verify no errors in start-up
3. Open executable for analysis
4. Tools > Start server
5. View > Script console  (Ctrl + `)

Open browser > http://localhost:1337
Enter in commands to Binja.

To manually command Binja from the command line:
1. Enter in command line:
import xmlrpclib

s = xmlrpclib.ServerProxy('http://localhost:1337')

2. Access commands:

s.SetColor('0x0040101b','0xfff000')

s.Jump('0x0040101b')

s.MakeComm('0x0040101b','Test Comment')

s.version()

s.shutdown()

s.system.listMethods()

['Jump', 'MakeComm', 'SetColor', 'Sync', 'shutdown', 'system.listMethods', 'system.methodHelp', 'system.methodSignature', 'version']
