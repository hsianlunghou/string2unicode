# String To Unicode

## Overview

**The string2unicode** is a lightweight GUI tool built with Python and Tkinter that converts **Traditional Chinese Characters** into **Unicode Sequences** and **U8G2 Hexadecimal Format**.

This tool is designed for embedded systems (such as OLED displays using the **u8g2** library) where **Traditional Chinese Characters** are not supported by default and must be defined in font table manually.

## Motivation

Most OLED libraries do not support **Traditional Chinese Characters** natively. To render chinese text, developers typically need to:

1. Extract each character’s unicode code  
2. Convert it into hexadecimal format  
3. Use the result to build a custom font table  

This project automates the conversion process through a simple GUI, reducing manual effort and potential errors.

## System Description

- Simple GUI
- Input of **Traditional Chinese Characters**
- Automatic validation
- Converts characters into:
  - Unicode escape format (`\u4e2d`)
  - U8G2 hexadecimal format (`$4e2d`)
- Separated the output by comma for easy copy

## Example

### Input
```shell
中,文,測,試
```

### Output
```shell
\u4e2d,\u6587,\u6e2c,\u8a66
```

## Requirements

- Python
- Tkinter

## Start environment

1. Clone this repository:
   ```bash
   git clone https://github.com/Jaigeng/string2unicode.git
   ```
2. Run the program:
    ```bash
    python string2unicode.py
    ```
