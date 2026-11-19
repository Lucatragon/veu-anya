# Update History
#### Marked with 
<ol>🟢 is completed,</ol>
<ol>🔵 is current,</ol>
<ol>🟠 is not released yet or unstable,</ol>
<ol>🔴 is not worked on.</ol> <br><br>

## 🔵 Alpha (Mars)
#### 🔵 Alpha 0 (pending update confirmation)
* Introduced commands
* Introduced license VFL2 and deprecated license AZGLv1
* Made a wiki for organization
* Renamed Artzenith Sound to Veu Demeteria
* (0.2) Renamed Veu Demeteria to Veu Kiri
* (0.8) Renamed Veu Kiri to Veu Anya
#### 🔴 Alpha 1 (Mars 1) (pending update initialization)
* Prototyping in Turbowarp
  * This involves getting the ``.aso`` and ``.asn`` files put in place for first initialization
  * Will utilize PCM WAV Audio and a MIDI-like file format system to host audio files to try to make a song
  * Watchdog needs developing
    * Will attempt to complete in a later update
    * Watchdog does not need developing yet until I can confirm ``.aso`` and ``.asn`` file initialization.
  * Idea:
    * ``.asp`` (Anya Sound Pack) could be a file format that allows ``!Instrument`` labels to be hosted separately, and the ASP code could be in a function call (e.g. soon, there would be a way to go inside of ``.aso`` and ``.asn`` files and make the ``!Instrument`` label call a ``.asp`` file with a specific ``.asp`` code, and then ``Factors`` (``F0``, ``F1``, etc, inside of ``!Chart``) could be any number possible because instruments could just require an ID, the ID could get called, and if the ID cannot be found, a fallback ``Factor`` could be implemented.
    * Example given in Figure 1.
   
Figure 1: Tadashii (C/Ruby hybrid) code that could be an example function for calling an ``.asp`` file.
```tadashii
!Instrument
    Instrument Flute fn[a](require asp flute.e359) : iF
    Instrument Drums fn[a](require asp drums_synth.e359): dS
```
### Naming convention for Non-Alpha, such as Beta, Centuri, Fault, and Ignis
```
00           000
Major        Minor
Release      Release

Example: 00010 = Saturn (00, 01) + Minor Release Code 0010 (Beginning of
repo, bug fixes are similar in number but major releases involve higher
number jumps, so 06225 to 06331 is a bigger jump in changes than 06225 to
06278).
```

## 🔴 Beta (Saturn)
#### 🔴 Beta 00010 (Pending completion of tasks instructed by Mars 1.0; requires Watchdog completion for Windows or Linux systems {WSL might have support, research further})
