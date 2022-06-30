How To Install:
1. Run DDEPrinterServer.exe into Server PC
2. Open "Setting" Tab and Create Admin Password for the firs time
3. Select the IP Server that will be used to connect with the client,
4. Input port (Default: 11111)
5. Press the "Create Client App" button and copy client app that was created (DDEPrinterClient.exe) to the computer where the print request will be sent (Client PC)
6. On the client computer, run DDEPrinterClient.exe which has been copied from the server for the first time, if the client computer has not been installed an old version of DDEPrinter, then do the Install Protocol handler by pressing the "install" button in the message box that appears. The location where you run DDEPrinterClient.exe will be recorded as the DDEPrinter path.
7. To make sure the DDEPrinter Protocol Handler is installed, please do the testing by typing "ddeprinter:test" in the addressbar of browser on the client computer or clicking on the shortcut provided (Command-Test)

*The api key is an encrypted code that is set on the client app so that the client app can be connected to the server where it was created, the admin doesn't need to configure anything in the client app, just create a client app and distribute it directly to the client computer

Available Command:
1. ddeprinter:[base64_encode] -> without brackets
	base64_encode contains: "PDFFileName|PrinterName|LinkOfPDFFile|PaperSize|Copies"
2. ddeprinter:resumePrinter:PrinterName
3. ddeprinter:pausePrinter:PrinterName
4. ddeprinter:clearSpooling:PrinterName
5. ddeprinter:test

How to Use Command:
To run DDEPrinter on web apps you can use the html tag "a" 
for example:
	<a href="ddeprinter:command_here">
or you can call it using javascript:
	window.location.href ="ddeprinter:command_here";
You can also call it by accessing directly from the adressbar of browser on the client computer

Document support:
Only PDF file

Limitation:
For evaluation purposes, the server can only print 50 times, after the counter has been reached, the application must be activated to use it again.

Contact Us:
If you are interested in this application, you can contact us directly via Whatsapp or Telegram at +6282350550603
