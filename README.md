#LPL

Language and Platform independent libraries

##Key features:
* Platform independent
* Language Independent
* General function language
* Translation of code module to any platform or language defined
* Use one language syntax for e.g. Ruby

##Eg:
```ruby
use SPI
SPI.Write(0xFF1020);
```
##Translates to:
```C
Chip_SPI_Write(SPI1, 0xFF);
Chip_SPI_Write(SPI1, 0x10);
Chip_SPI_Write(SPI1, 0x20);
```
##Or 
```C
SPI.begin();
SPI.transfer(0xFF);
SPI.transfer(0x10);
SPI.transfer(0x20);
```
