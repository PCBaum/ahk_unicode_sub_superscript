## Autohotkey for ℝℤℂℚ

This AHK script lets you use all the Unicode sub and superscripts I could find

for Superscript use Backslash '\' circumflex '^' and your desired character. Afterwards you will also need to type a Space, since i couldn't get rid of the circumflex in any more elegant fashion. 

Unicode only has Numbers {0,1,...,9,0}, Operators {+,-,=,),(} and the letter "n" as a superscript (as fa as i could tell
```
\^1 → ¹, \^2 → ², etc.
```
for Superscript use Backslash '\' underscore '_' and your desired character.

Unicode only has Numbers {0,1,...,9,0}, Operators {+,-,=,),(} and the letters {a,e,o,x,h,k,l,m,l,n,p,s,t} as a subscript (as fa as i could tell
```
\_1 → ₁, \_2 → ₂, etc.
```


## AHK Installation

  1. Download [Autohotkey](https://www.autohotkey.com/download/) and install it. 
  2. Download the script [Sub_Super.ahk](https://github.com/PCBaum/ahk_unicode_sub_superscript/blob/main/Sub_Super.ahk)
   or create a new script with your prefered Name and copy paste the Key Mapping into it.
  3. Put the script into a folder of your choice. 
  4. Start the script Sub_Super.ahk 
  
  Optional: 
  
  5. Compile your Script with rightclick → compile script (shoud be somewhere around the the second row)
  
  6. Put the executable ("YOUR_SCRIPT_NAME".exe) in your Startup Folder "C:\Users\"USERNAME"\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup" to have the script automatically start on Startup.
  
  
# Whithout installing AHK on Windows

  1. Download the compiled [Sub_Super.exe](https://github.com/PCBaum/ahk_unicode_sub_superscript/blob/main/Sub_Super.exe) File
  2. Put the script into a folder of your choice.
  3. Start the script Sub_Super.exe
  
  Optional:
  
  4.  Put the executable in your Startup Folder "C:\Users\"USERNAME"\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup" to have the script automatically start on Startup.

## Key Mapping 

how this AHK script maps input to output: 
::input::output   output is given as the Unicode code.

```

#NoEnv  ; Recommended for performance and compatibility with future AutoHotkey releases.
; #Warn  ; Enable warnings to assist with detecting common errors.
SendMode Input  ; Recommended for new scripts due to its superior speed and reliability.
SetWorkingDir %A_ScriptDir%  ; Ensures a consistent starting directory.
#Hotstring C * ?
::\^0::{U+2070}
::\^i::{U+2071}
::\^1::{U+00B9}
::\^2::{U+00B2}
::\^3::{U+00B3}
::\^4::{U+2074}
::\^5::{U+2075}
::\^6::{U+2076}
::\^7::{U+2077}
::\^8::{U+2078}
::\^9::{U+2079}
::\^+::{U+207A}
::\^-::{U+207B}
::\^=::{U+207C}
::\^(::{U+207D}
::\^)::{U+207E}
::\^n::{U+207F}




::\_1::{U+2081}
::\_2::{U+2082}
::\_3::{U+2083}
::\_4::{U+2084}
::\_5::{U+2085}
::\_6::{U+2086}
::\_7::{U+2087}
::\_8::{U+2088}
::\_9::{U+2089}
::\_+::{U+208A}
::\_-::{U+208B}
::\_=::{U+208C}
::\_(::{U+208D}
::\_)::{U+208E}

::\_a::{U+2090}
::\_e::{U+2091}
::\_o::{U+2092}
::\_x::{U+2093}
::\_h::{U+2095}
::\_k::{U+2096}
::\_l::{U+2097}
::\_m::{U+2098}
::\_n::{U+2099}
::\_p::{U+209A}
::\_s::{U+209B}
::\_t::{U+209C}
#Hotstring *0 ?0 C0

```

## Credits

Template for AHK Script: was a some time ago and I don't remember. Also, the beginning seems to be standard, and is the only not heavily changed part.
