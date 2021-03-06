# VBAStopWatch
# This repository contains the files necessary to follow the tutorial on making an Excel VBA stopwatch.
The stopwatch is a VBA form driven application that simply records elapsed time since the start button was pressed. Before starting the lesson, the student launches the stopwatch and presses the Start button. The Stop button is pressed at the end of the lesson. Elapsed time can then be logged into the workbook. It's designed to measure speed improvement when building the workbooks found in the https://www.sharexl.com Extreme Excel lessons. With practice, you'll develop Excel shortcut finger memory, as well as speed ehancements provided by your game mouse (if using one). This exercise is not only about building a stopwatch, it's about following instructions to the letter. (I'm assuming that my instructions are clear and correct)
# Prerequisites:
1. The Developer tab must be visible in Excel. <br>
  Expose Excel Developer tab on Ribbon. Youtube: (https://www.youtube.com/watch?v=JLQ8OuW0FlY)
2. A trusted folder where VBA code can be run in Excel.<br>
  Add the folder where you want to build and run this exercise to Excel's Trusted Location list. Youtube: (https://www.youtube.com/watch?v=t5OcD1bk7Ek)
# Steps for Building the project
1. Download "SWVBA_GitFiles.zip" from "Code" button on Github.
2. Open “SWVBA_GitFiles.zip” and save the files to your local pc (place in Excel Trusted folder).
3. Rename "mod_Stopwatch.txt" to "mod_Stopwatch.bas"
4. Create SWEEWB1.xlsx workbook an "Save As" SWEEWB1.xlsm (macro enabled workbook type)
5. Rename "Sheet1" to "Log"
6. Click on the “Developer” tab to access the “Visual Basic” code window. Click on the “Visual Basic” icon. (the “Microsoft Visual Basic for Applications” window appears).
7. Create a userform and name it: frmStopwatch (click on the form and hit F4 button to change properties)</br>
  (note: it is important that you name the form and controls as defined in these instructions, otherwise the code won't match with your controls and will never be executed.) 
The form should look like this:
![Form Stop Watch](FrmStopwatch2.png)
8. Having the form properties windows open, set the frmStopwatch (the userform) ShowModal property to false. (note: When ShowModal = false, the user can interact with the workbook. Otherwise, the form must be dismissed to access the workbook.).This is also a good time to set the form's caption to read "Stop Watch".
9. Add 5 command buttons to the form (frmStopwatch). Shown above in red above. Name them as follows:</br>
cmdStart</br>
cmdStop</br>
cmdLog</br>
cmdClear</br>
cmdClose
9. Add 3 labels to the form (frmStopwatch). Add borders to labels and remove any caption. Name the controls as follows:</br>
lblTime1</br>
lblTime2</br>
lblEtime
10. Change captions on the userform and command buttons:</br>
frmStopwatch = Stop Watch</br>
cmdStart = Start</br>
cmdStop = Stop</br>
cmdLog = Log Time</br>
cmdClear = Clear</br>
cmdClose = Close</br>
11. Import the "mod_Stopwatch.bas" file.
12. Run the "Test" subroutine in the module and repair any naming errors that might occur.
13. Open the text file SWFormCode.txt in a text editor and copy all contents into the clipboard 
14. In VBA project explorer, right click on Forms | FrmStopwatch and select View Code
15. Delete all existing code in the form and paste the contents from SWFormCode.txt in its place
16. Go to the workbook and run the macro "ShowSW". 
17. Test the form by clicking the Start button, waiting a few seconds then clicking the Stop button. Click the Log button to pass the values in the Log worksheet. 

