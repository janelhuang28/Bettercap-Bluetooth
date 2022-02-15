# Haunting-Computers-using-SSH

To show that access can be granted to a victim, different messages can be displayed to the victim. 

## Linux

1. To say something to the victim: ``sudo modprobe pcspkr`` and then type: ``say "<Item>"``
2. To make beeping sounds: ``beep -f 5000 -D 500 -l 1000 -r 10``
3. To make Warnings: ``notify-send 'WARNING` '<Message>'``
4. To make pop up messages: ``xterm -maximized -fullscreen -fa 'Monospace' -fs 19.31 -e whiptail --title "<title>" --msgbox "<Message>" --topleft 23 79``
5. To open a new firefox browser: ``firefox -new-window "<site>"``


## Windows
1. To open a chrome tab: ``start Chrome <Site>``
2. TO notify a user of a message: ``PowerShell -Command "Add-Type -AssemblyName PresentationFramework;[System.Windows.MessageBox]::Show('<Message>', '<Title>', 1, 48)"``
3. To say something to a user: PowerShell -Command "Add-Type -AssemblyName System.Speech; (New-Object System.Speech.Synthesis.SpeechSynthesizer).Speak('<Message>');"
4. To make beeping sounds: ``powershell "[console]::beep(<Frequency>,<Duration>)"`` E.g., ``powershell "[console]::beep(500,700)"``
