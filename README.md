# AVR BASIC Computer v0.2

### Work based on:
- https://github.com/BleuLlama/TinyBasicPlus
- https://github.com/fuzzymannerz/AVR-BASIC-Computer and 
- https://github.com/Volhout/TinyBasicPlus
- PCB - https://easyeda.com/tazyman/avr-basic by https://hackaday.io/hacker/342571-razvanclontea

---

### Changes:
- Added MIN, MAX, VARS, HELP commands (Volhout)
- Added CLS - clear screen
- Added FONT X - switch to diffrent font:
    - 0 - 4x6
    - 1 - 6x8
    - 2 - 8x8
    - 3 - 8x8ext
- Fixed backspace on TV
- Various fixes in Tiby Basic Code (some from Volhout)
- ESC to break running program

---

### Port breakout vs Arduino Pin numbers (reading from left to right, assumed MightyCore DIP40 Standard pinout):

| Port / # | 1  | 2  |       3          | 4  | 5  |       6          | 7  | 8  |
|:--------:|:--:|:--:|:----------------:|:--:|:--:|:----------------:|:--:|:--:|
|    A     | 24 | 25 |       26         | 27 | 28 |       29         | 30 |    |
|    B     |  1 |  2 |        3         | 4* | 5* |        6*        | 7* |    |
|    C     | 23 | 22 | 21, 15, Port D6* | 20 | 19 |       18         | 17 | 16 |
|    D     |  9 | 10 |       11         | 12 | 14 | 15, 21, Port C3* |    |    |

```* - connected to something else on the board, use with caution```

# MIT License

Copyright (c) 2020

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.