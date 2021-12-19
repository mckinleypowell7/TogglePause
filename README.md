# TogglePause
   ; Wait 10 seconds for the Notepad window to appear.    WinWait("[CLASS:Notepad]", "", 10) EndFunc ;==>OpenNotepad  Func StartCount()    ;Start writing 1 to 100 in Notepad    For $i=1 to 100 Step +1       Send ( $i &amp; Chr(10) )       Sleep( 300 )    Next EndFunc ;==> StartCount  Func TogglePause()    $g_bPaused = Not $g_bPaused    While $g_bPaused       Sleep(100)    WEnd
