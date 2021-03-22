## Thermocouple Vacuum Gauge.

This page details a small microcontroller project that reads a vacuum thermocouple gauge. At its completion it will include all the necessary kicad files to create or modify your own pcb, a bill of materials (BOM) for the components necessary to assemble the pcb and the program to run the whole thing. It's core design is based on a circuit from [The Bell Jar](http://www.belljar.net/tcgauge.htm). 

![Image of Assembled PCB](https://github.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/blob/gh-pages/IMG_1577.JPG)


### The PCB
The PCB connects a [TI Tiva C Launchpad](https://www.ti.com/tool/EK-TM4C123GXL) to a [SparkFun LCD display](https://www.sparkfun.com/products/16397) and a non-inverting op-amp that amplifies the signal from the vacuum thermocouple gauge. It was designed in KiCad and the boards themselves were manufactured by OSH Park, though of course you are able to use whichever manufacturer you prefer. You can see the bare board below. All of the necessary files (including gerbers) are included in the [Thermocouple Gauge folder](https://github.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/tree/main/Thermocouple%20Gauge). 

![Image of PCB](https://github.com/FuzzyBunnys/Thermocouple-Gauge-Sensor/blob/main/Thermocouple%20Gauge/IMG_1577.JPG) 
### The BOM
The BOM is an excel file with a listing of all the required components for the PCB, certain components have the Digikey link included directly, but for generic components such as resistors or pin headers there is no Digikey link. It shouldn't be too difficult to select those components yourself.
### The Program
The program is written in [Mecrisp Stellaris](https://mecrisp-stellaris-folkdoc.sourceforge.io/) a dialect of Forth. The process for setting up Mecrisp Stellaris on a TI Tiva C Launchpad is as follows.


```markdown
Syntax highlighted code block

# Header 1
## Header 2
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
