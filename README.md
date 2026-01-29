# string2unicode

## Overview

**string2unicode** is a lightweight GUI tool built with Python and Tkinter that converts **Traditional Chinese characters** into **Unicode escape sequences** and **U8G2-compatible hexadecimal format**.

This tool is designed for embedded systems (such as OLED displays using the **u8g2** library) where Traditional Chinese characters are not supported by default and must be manually defined in a custom font table.

## Motivation

Most OLED libraries do not natively support Traditional Chinese characters. To render Chinese text, developers typically need to:

1. Extract each character’s Unicode code point  
2. Convert it into a machine-readable hexadecimal format  
3. Use the result to build a custom font or glyph table  

This project automates the conversion process through a simple GUI, reducing manual effort and potential errors.

## Features

- Simple and intuitive GUI
- Direct input of Traditional Chinese characters
- Automatic input validation
- Converts characters into:
  - Unicode escape format (`\u4e2d`)
  - U8G2 hexadecimal format (`$4e2d`)
- Comma-separated output for easy copy and integration

## Example

### Input
中,文,測,試


### Unicode Output


\u4e2d,\u6587,\u6e2c,\u8a66中,文,測,試


### Unicode Output


\u4e2d,\u6587,\u6e2c,\u8a66
