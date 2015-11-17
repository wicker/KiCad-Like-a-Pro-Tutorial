#### Notes in the KiCAD Like a Pro Tutorial

This is super accessible and I really like it.

Things with * are suggestions for him to add to the tutorial.  

I use hotkeys and the touchpad mouse. 
Hovering and hotkeys is awesome.

Might be worth mapping hotkeys to be entirely left hand

#### Schematic Hotkeys

Have to explicitly add wires/connections. Can't just move parts and overlap them and pull them away. 

Best practices: I like labels on my wires. I don't find the defaults helpful when you go to lay things out. Do the labels not stick?

Can't just grab labels off a set of wires by themselves? I want wires to grab on to pins and hold. Use control! 

- `a`		adds a part
- `m`		moves a part
- `r`		rotates a part
- `w`		adds a wire
- `x`		flips part across x axis (up/down)
- `y`		flips part across y axis (left/right)

*Hitting Ctrl before selecting will let you drag and keep wires attached. 

*To move a wire, right click and hit 'break wire' and then use Ctrl to select and drag that wire. 

*Labels are not obviously attached to wires in EESChema but it might turn out OK in the layout. 

Open the Part Library Editor from inside EESchema. Flow is a good thing. 

#### Schematic Parts Editor

It says no active library; that's OK. 

`g` grabs and lets you move the side of a box
`m` moves things
`p` adds pins
`r` rotates things

Any hotkeys to draw boxes? Any hotkeys for the Parts Library Editor? `m`, `r` still work. 

Can we batch import pins?

- [ ] Make a Wickerbox template

#### CvPCB to associate components and footprints

Associate the parts to the footprint. 
Save and you're back in EESchema.

#### Footprint Editor

It says no active library; that's OK. 

Open Footprint Editor for EESChema. I suspect you could just skip using the Project level view at all.

- [ ] Draw the workflow

Hotkey to set the grid?

`m` still works
`r` still works

Switch KiCAD to inches all over.

Explicitly use the rule of thumb for hole sizing. 0.762mm hole for a 0.64mm circumference of nRF24 pins. Check diameter vs circumference. ** I think your language is incorrect here. p34. 

Instead of linking pads and pin names, we have to make the footprint pad numbers match the pin numbers. ** REALLY?

Click and dragging to select seems to work for moving, though it doesn't grab.

Holding shift or control while clicking and dragging makes a copy of the whole group.

Holding shift and control while clicking and dragging deletes everything that was selected.

I use 'd' for delete, because it lets me move with the right hand on the mousepad and use the left hand. All my hotkeys should be like this.

Would like to just hit enter from anywhere in the Footprint Editor Footprint Text Editor window.

Text: 0.5 width and 0.5 height ** square this away with the OSH Park guidelines

This workflow sucks:
Create a new library
Use the Footprint Library Wizard to find the library
Select active library
Save footprint in active library

#### Netlist! from EESchema

#### PCBNew

Global spread and place might be useful, but my workflow is often to grab individual sets of components. I like `t` to get and move a particular component. 

Intelligent placement: http://electronics.stackexchange.com/questions/81415/can-i-make-kicad-pcbnew-not-place-all-components-at-0-0


