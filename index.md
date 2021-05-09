## Thermocouple Vacuum Gauge.

This page details a small microcontroller project that reads a vacuum thermocouple gauge. At its completion it will include all the necessary kicad files to create or modify your own pcb, a bill of materials (BOM) for the components necessary to assemble the pcb and the program to run the whole thing. It's core design is based on a circuit from [The Bell Jar](http://www.belljar.net/tcgauge.htm). However my design uses a non-inverting amplifier to simplify the power supply.

![Image of Assembled PCB](https://raw.githubusercontent.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/gh-pages/IMG_1578.JPG)


### The PCB
The PCB connects a [TI Tiva C Launchpad](https://www.ti.com/tool/EK-TM4C123GXL) to a [SparkFun LCD display](https://www.sparkfun.com/products/16397) and a non-inverting op-amp that amplifies the signal from the vacuum thermocouple gauge. It was designed in KiCad and the boards themselves were manufactured by [OSH Park](https://oshpark.com/), though of course you are able to use whichever manufacturer you prefer. A third revision of the board was completed to correct some mistakes identified in the second revision. All of the necessary files (including gerbers) are included in the [Thermocouple Gauge folder](https://github.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/tree/main/Thermocouple%20Gauge). 

![Image of PCB](https://raw.githubusercontent.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/gh-pages/IMG_1577.png) 
### The BOM
The BOM is an excel file with a listing of all the required components for the PCB, certain components have the Digikey link included directly, but for generic components such as resistors or pin headers there is no Digikey link. It shouldn't be too difficult to select those components yourself.
### The Program
The program is written in [Mecrisp Stellaris](https://mecrisp-stellaris-folkdoc.sourceforge.io/) a dialect of Forth. The process for setting up Mecrisp Stellaris on a TI Tiva C Launchpad is as follows.
1.	Download Mecrisp-Stellaris
2.	Download TI's Uniflash
3.	Connect the Tiva C series board via usb and the debug port
4.	Load mecrisp-stellaris-lm4f120.bin using Uniflash on to the board
5.	Make a connection at 115200 baud rate via TeraTerm to the launchpad board.
6.	Reset the board and the welcome message for mecrisp stellaris should appear.


```markdown
Syntax highlighted code block

# Header 1
## Header 2b 
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).



You can use the [editor on GitHub](https://github.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.
