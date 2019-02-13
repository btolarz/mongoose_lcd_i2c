# Mongoose OS library for HD44780 i2c LCD
Mongoose lib for i2c hd44780 LCD


## Overview

This is early version of this lib.

## Usage

Make sure

This lib use `mgos_i2c_get_global()` so make sure:
- you have `- ["i2c.enable", true]` in `config_schema`
- don't use in `mgos_app_init_result`, create timer, or event handler

- `LCD_Init()` - init display
- `LCD_Clear()` - clear display
- `LCD_Set_Position(0,0)` - set cursor position
- `LCD_Send_String('test string')` - send string

### Sources
- https://github.com/fdebrabander/Arduino-LiquidCrystal-I2C-library/
- https://elektronika327.blogspot.com/2017/01/9-stm32f4-cubemx-wyswietlacz-hd44780-z.html