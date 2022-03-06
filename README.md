# CNC-2417-PCB-Maker

I've been looking for a way to create cheap, custom PCBs at home for prototyping. This is the process that i came up with.

# Requirements
- A CNC machine, i bought the 2417 from ebay (for about 220€). I am not sure how this is going to workout for other machines. but its probably gonna work.
- Copper clad boards (ebay). Single sided will work
- 2 mill cutters (i bought mine from sorotec.de)

# How to

1- I use EasyEDA to design the PCB. As the CNC is not as accurate as the usual pcb-creating-machine. we will have to thicken all our lines. Right click on your pcb designer screen, click design rule and use the following settings: 
|           Config           |   Setting   |
|:--------------------------:|:-----------:|
| Track Width                | 0.6 mm        |
| Clearence                  | 0.6 mm        |
| Via Diameter               | 1 mm      |
| Via Drill Diameter         | 0.8 mm        |

I use the auto router. Press Route --> Auto Route
Make sure only TopLayer is selected as we only want to create one layer. I havent experimented with two layers and maybe it will work, but requires more work as you would manually have to flip the pcb and make sure its aligned, then run the job again.

2- Once your PCB design is finished, export as GERBER
