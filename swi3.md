# SWI 3

## data units

- all data is stored in bits
- bits make up bytes
- every single data type is somehow saved in bytes
	- `int` or `double` is a bunch of bytes, `string` is a series of `char` which are also numbers, etc.

![[Pasted image 20260507162717.png]]

## dates

- standardized by the **ISO 8601** format: `YYYY-MM-DD`
- or **DateTime (ISO):** `YYYY-MM-DDTHH:mm:ssZ`
- americans are fuckwits and have `MM/DD/YYYY`


## numeral systems

- decimal - 0-9; the one we use
- binary - 0-1; the one computers use
- hexadecimal - 0-F; very useful for representing data - a byte in binary is two digits in hexadecimal
- octal - 0-7; more niche, but still has its use

## characters

- first main system was ASCII - 7 bits per character
	- didnt include any international characters
- ISO-8859-2 was the eastern european equivalent used by czechs, poles etc.
- unicode then showed up
	- UTF-8 uses a full byte, allowing more accessibility for other langs but still is compatible with ASCII
	- then here is UTF-16 and UTF-32
	- we dont talk about UTF-64

![[Pasted image 20260507205300.png]]

## primitive vs composite types

- primitive data types are a singular value (number, character, boolean, etc.)
- composite types are complex structures composed of primitive types (string, array, dictionary, object, etc.)