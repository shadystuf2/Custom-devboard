---
Title: "Fancy Devboard"
Author: "Nomeda"
Description: "A custom PCB that has an RP2040 and an accelerometer"
Created at: "2026-06-21"
---

THIS PROJECT IS FOR HORIZONS EUROPA

## June 11th: Got schematics done and started the layout
I got the inspiration for this from one of the starter projects in STASIS but decided to add some sensors and designs. I followed the tutorial for schematics on KiCad. Honestly, I struggled with I/O labels a bit, since the
shapes sometimes don't make sense. Also, dealing with the crystal oscillator was funny, since we thought that we had the wrong schematic,
since it had only 3 pins. Turns out the 4th one was hidding under one of the other pins and we had to modify the schema manually. 
Then we were looking for footprints which was a very tedious job. I also helped out my friend, as he was struggling with the overall 
logic of the schematic.  

Finished schematic:
<img width="976" height="676" alt="Screenshot 2026-07-18 at 22 55 03" src="https://github.com/user-attachments/assets/d4dd15f3-1c01-44c5-8fca-5dad9026533c" />

**Total time spent: 4h**


## June 18th: Finished layout and routing
This is where I stopped following the tutorial. The layout and routing is completely my own. I arranged the componenets on a basic rectangle, since I want the devboard to be compact and usable. Then (very convinient timing) I decided,
that I want to add a sensor and chose an accelerometer and gyroscope MPU-6050. I noticed that a switch that was in the schematic was 
missing, so I had to reload and delete and add it several times. Then I started routing and had to rearrange the components so that 
everything would fit. Many hours later, I added ground fill, saw the number of errors that popped up and closed my PC immedietly.  

Layout:  
<img width="348" height="755" alt="Screenshot 2026-07-18 at 23 33 20" src="https://github.com/user-attachments/assets/587ba0c6-4ff1-4306-9492-95cab58a76d5" />  

Routed version:  
<img width="326" height="635" alt="Screenshot 2026-07-18 at 23 34 42" src="https://github.com/user-attachments/assets/dec5a915-c1f4-40a5-b830-78281262bd3a" />

**Total time spent: 4h**

## July 7th: Ground fill and Debugging
Finally, the much dreader debugging session. Apparently, my wiring was a bit too random with too many vias so making space for ground fill 
was quite time consuming. After that I just went through the errors in the design rules checker one by one and cleared them. It finally looked
polished and I was very happy with how it turend out. The only thing that I wanted to add was a design.  
Also, later I realized that I can do ground fill on both layers, but I somehowd managed and did my whole routing with only the front filled. 
And I cleared all errors. No wonder it took so long. But lesson learnt.  

Devboard with ground fill: 
<img width="368" height="785" alt="Screenshot 2026-07-18 at 23 45 42" src="https://github.com/user-attachments/assets/18c73ce8-c2f7-4616-9616-29335a0e7d82" />

**Total time spent: 3h**

## July 15th: Design  

I removed all the component labels. Initially, I wanted to do a constelation of stars, then star people, but it was not very
visible so I ended up adding just these giant stars. I did not really know what would be a convenient software that could 
export .SVG files so I used Boxy SVG for my designs and drew them.  

Star people design (not mine, credits to artist but I don't know who they are beacuse the person who posted this on pinterest doesn't say):  

<img width="736" height="736" alt="image" src="https://github.com/user-attachments/assets/0874ff09-79df-4b94-8a74-d4ac53bdcba8" />  

Final product:  

<img width="803" height="612" alt="Screenshot 2026-07-18 at 23 51 29" src="https://github.com/user-attachments/assets/77796cf6-e2eb-4c8d-bf60-939614b0ba01" />


**Total time spent: 2h**
