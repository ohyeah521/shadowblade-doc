DataPack, Format of byte transfer pack
=========

Struct
------

`0X00-0X01:` DE AD <br>
>//signature, -8531 in demical

`0X02-0X09:` XX XX XX XX XX XX XX XX  <br>
>// 8 bytes `length` value, in big endian, `long long` in C++, `long` in Java

`0XA0-(0XA0+length)`:  <br>
>//Raw data, `0X02-0X09` value as length
