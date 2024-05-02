# Input-Macro-Library
Simple Input macro library currently made for both Windows and MacOS, multiple different version to choose from based on preference, the C header variant would be the best option 
and most viable for most projects, assembly language variants are still viable for assembly only projects and as a simple showcase of what assembly syntax Is like for beginners.
Listed down below Is some brainstorming of my future ideas for this project as well as a short description of each variant of the library and a table for those who want only a few
specific macro's without having to download the library.

# What Is planned for the future
- Expanding input.h
- Rewriting It In assembly language for Windows x86 and x64, ARM64 (MacOS) and linux x86 and x64
- Rewriting It In Python
- Adding extra functionality to the libraries rather than only Including convenient key macros
- Using It In a project myself to verify that It works as It should, there are no errors within the code but it's best to be sure

# input.h
A single header library for made for C and C++, Includes Virtual keycodes of all the common keys as well as the ones that can't be used
without virtual keycodes and macros.

# x86_win_input_macro.inc
Translated Into x86 assembly for Windows, compiles with the <i>MASM32</i> assembler on <i>Visual Studio 2022</i>.

# x64_win_input_macro.inc
Translated Into x64 assembly for Windows, compiles with the <i>MASM64</i> assembler on <i>Visual Studio 2022</i>

# ARM64_MacOS_input_library.s
Translated Into ARM64 assembly for <i>Apple Silicon</i> devices (<i>MacOS</i>)

# Special key table
| Key  | Macro name | Virtual Keycode WIN32  | Virtual Keycode (MacOS) |
| ------------- | ------------- |----------------|--------------|
| Left Mouse Button  | KEY_LMB  | 0x01 |  |
| Right Mouse Button  | KEY_RMB  | 0x02 |  |
| Escape | KEY_ESC | 0x1B | 0x35 |
| Return/enter | KEY_RTN | 0x0D | 0x24 |
| Control | KEY_CTRL | 0x11 | 0x3B |
| Alt | KEY_ALT | 0xA3 |  |
| Spacebar | KEY_SPC | 0x20 | 0x31 |
| Backspace | KEY_BKSPC | 0x08 |  |
| Left shift | KEY_LSHFT | 0xA0 | 0x38 |
| Right shift | KEY_RSHFT | 0xA1 | 0x3C |
| Function | KEY_FN |  | 0x3F |
| Numpad 0 | KEY_N0 | 0x60 | 0x52 |
| Numpad 1 | KEY_N1 | 0x61 | 0x53 |
| Numpad 2 | KEY_N2 | 0x62 | 0x54 |
| Numpad 3 | KEY_N3 | 0x63 | 0x55 |
| Numpad 4 | KEY_N4 | 0x64 | 0x56 |
| Numpad 5 | KEY_N5 | 0x65 | 0x57 |
| Numpad 6 | KEY_N6 | 0x66 | 0x58 |
| Numpad 7 | KEY_N7 | 0x67 | 0x59 |
| Numpad 8 | KEY_N8 | 0x68 | 0x5B |
| Numpad 9 | KEY_N9 | 0x69 | 0x5C |
| Left arrow | KEY_LAK | 0x25 | 0x7B |
| Up arrow | KEY_UAK | 0x26 | 0x7C |
| Down arrow | KEY_DAK | 0x27 | 0x7D |
| Right arrow | KEY_RAK | 0x28 | 0x7E |


<i>Only virtual keycodes of keys that can't be typed Into code have been added to this list, the full list of macro's are In the header file</i>
