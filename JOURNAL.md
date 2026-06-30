---
Title: Unwired
Author: NoxAevi
Description: A small battery-powered device that turns wired peripherals (mainly keyboard/mouse) to wireless, including a toggle between 2.4 GHz proprietary and Bluetooth
Created: 2/27/26
---

# 6/30/26: Learned basic C syntax

I haven't really coded in C before at all, so the pretty obvious thing to do before starting on firmware would be to start learning the basic syntax of C

I followed along with this video: https://www.youtube.com/watch?v=GqEeOrDk5DI, which involves creating the ls command from scratch and looked up other videos when necessary to understand what was going on, such as [what are pointers](https://www.youtube.com/watch?v=2ybLD6_2gKM&t=438s) and how they work

This wasn't too bad, and I feel like I should be ready to start working on the firmware tomorrow

What was unexpected however, was that there were a couple similarities between C and Verilog, such as the bitwise operators, ternary, and switch statements

**Total Time Spent**: 1.5 hours

# 6/29/26: Enclosure done

I immediately realized I forgot to include a part for the screw heads to catch onto on the face plate, so I quickly added those in (so the screws would actually work)

<img width="865" height="399" alt="image" src="https://github.com/user-attachments/assets/6106a3f5-7731-4256-b8b0-dc7d62e40162" />

After I started the top part of the enclosure, I realized that this part on the bottom would be unneccessary because there would be a plate instead

<img width="469" height="82" alt="image" src="https://github.com/user-attachments/assets/8b7876af-c442-4460-99a7-0b1b1764b882" />

Since I would also a palces to put a screw hole later, I also extended the part holding up the PCB

<img width="672" height="324" alt="image" src="https://github.com/user-attachments/assets/8e08de69-e6ad-4f61-93c5-af32b650ddf8" />

After double checking the hackclub [stasis FAQ](https://stasis.hackclub.com/docs/design-resources) i found out that the 4.7mm hole diameter for the heatset insert was actually the OD on the insert itself, so I did some research on what size the hole should be

I found [this](https://www.reddit.com/r/3Dprinting/comments/1pco9ah/heat_set_insert_question/) thread on reddit and noticed that the heatset inserts I sourced do not have the "pilot" side and that it might be better to use [these](https://www.aliexpress.us/item/3256806910034634.html) instead

<img width="249" height="285" alt="image" src="https://github.com/user-attachments/assets/25c7d7d7-f078-4fa2-8120-71c58445c41d" />

I resized the hole diameters (which broke some references that I had to go in and redo) and added counterbores to give room for the melted plastic to flow

<img width="784" height="696" alt="image" src="https://github.com/user-attachments/assets/0b7f5342-71ac-4ef3-9ccf-695a041afca2" />

I then changed some stuff to account for the bigger OD, and this kinda ruined the alignment of the top and bottom

<img width="447" height="420" alt="image" src="https://github.com/user-attachments/assets/0d1cea76-6385-4790-99ea-c90418537193" />

Thus, I had to use the rollback bar and go through each change and refit the dimensions

<img width="304" height="177" alt="image" src="https://github.com/user-attachments/assets/62d4346f-b232-4b0f-9e57-15fcf1758f68" />

This allowed me to get a perfect fit

<img width="559" height="477" alt="image" src="https://github.com/user-attachments/assets/12e8a622-3615-4644-8fdd-44a7d03a4b20" />

I then added the screw holes to match up with the top and bottom, which was pretty quick since i'd already done it quite a bit to get to this point

<img width="574" height="505" alt="image" src="https://github.com/user-attachments/assets/ecb0dd6c-f133-421f-aa05-0dbfe7ee0bd5" />

<img width="304" height="249" alt="image" src="https://github.com/user-attachments/assets/0a5449b8-33f7-48cb-9e40-f46107846070" />

Now all that's left is stuff for the button, and a tiny hole for the LED

Although I initially believed that putting the hole in the direct center would look better, I feel that it's nicer with the hole in line with the USB C hole

<img width="525" height="493" alt="image" src="https://github.com/user-attachments/assets/699fa47c-3b4a-4ae2-96de-458326989756" />

<img width="877" height="723" alt="image" src="https://github.com/user-attachments/assets/5ef16f31-1465-4a21-8034-f7e2909da146" />

Then, I made the button and polished everything up with fillets

When making the button, I added extra material so it would be able to stay in the enclosure & be firm/not have too much tilting, but this was really annoying to add because of how the U shaped case makes it difficult to see the gap in some areas (on the right in the picture below mainly)

<img width="775" height="361" alt="image" src="https://github.com/user-attachments/assets/ca976218-d906-4032-8d73-6f5174076f70" />

Anyways these two are the final pictures for the enclosure


<img width="537" height="517" alt="image" src="https://github.com/user-attachments/assets/851cfb79-b26b-45c5-a845-a2076ae8da58" />

<img width="735" height="600" alt="image" src="https://github.com/user-attachments/assets/069ad737-3915-4dcc-bf48-e9bc4cd9256c" />

**Total Time Spent:** 2.5 hours

# 6/28/26: Enclosure bottom Modeled

I decided to use onshape to do this because it was what I was most familiar with (after using it for the local science olympiad comp)

After importing the STEP of the PCB, I had a bunch of sub-parts cluttering the bar, so I first had to put these all into a folder to make it neater

<img width="1254" height="70" alt="image" src="https://github.com/user-attachments/assets/cb2b3fa6-241f-49ba-aa44-7f29413d983c" />

Before starting, I wanted an idea of how tight stuff should be to stay compact while having a relatively loose fit (making it easy to assemble), so I found [this article](https://3dchimera.com/blogs/connecting-the-dots/3d-printing-tolerances-fits) which gave some guidelines

<img width="1054" height="451" alt="image" src="https://github.com/user-attachments/assets/8c288b1d-7181-4bf8-9b65-de7f08b665f7" />

I also realized that some of these parts that stick out might be a pain, so I plan to only add extra material where needed (for the screw holes)

<img width="541" height="583" alt="image" src="https://github.com/user-attachments/assets/cb3747c0-8b0b-403f-9295-ff7bfebbeace" />

So far, this leaves me with this, but afterwards I decided to have another square on the bottom right corner because it would probably be easier when screwing the pcb in/stability

<img width="715" height="598" alt="image" src="https://github.com/user-attachments/assets/77a054a4-d22a-48a5-9901-6baec237bc53" />

Unfortunately, I had a bit of trouble lining up the holes properly, using measurements from the sides of the PCB and a construction rectangle of the PCB

<img width="483" height="786" alt="image" src="https://github.com/user-attachments/assets/555d6f5f-16e2-4f2a-ba42-97e4c7f26671" />

Then I realized I was being stupid and using min-dist instead of dist to center (because obviously the holes would be different sizes from the PCB and where the heatset inserts would be places)

This allowed me to easily line up the stuff, but when checking if there would be enough room for a screwhead, it wasn't looking too great (just this one spot, so all I had to do was resize a bit)

<img width="1366" height="679" alt="image" src="https://github.com/user-attachments/assets/b75c9ddb-66a6-45bd-a68f-beb293dd25bd" />

Then, to make sure that these dimensions would be good I sourced both the [heatset inserts](https://www.aliexpress.us/item/3256811859908423.html) (G3-L4-OD4.2) and the [screws](https://www.aliexpress.us/item/2251832857570651.html) (M3 5mm pan head) I would be using

Following this, I tried to make the hole for the USB receptacle, but because of how cluttered this diagram was, it took a while to understand

<img width="1167" height="889" alt="image" src="https://github.com/user-attachments/assets/fb92f5cb-0ce8-4033-a053-f8ed0faff503" />

I was eventually able to get it looking pretty good

<img width="739" height="391" alt="image" src="https://github.com/user-attachments/assets/298d193f-c891-4fd0-9585-ce7b8c337266" />

But I was concerned that the connector would not be able to go through the wall thickness

<img width="300" height="187" alt="image" src="https://github.com/user-attachments/assets/60ee994b-1f9d-4693-86ef-bffb392c8ccd" />

So I changed the distance from the connector to the edge on the PCB and re-exported as a step file (and also had to rearrange some traces, unfortunately(

<img width="685" height="343" alt="image" src="https://github.com/user-attachments/assets/2849e39d-d5d8-4e77-af58-c0102ef19216" />


This helped, but it still needed to be moved up more

<img width="643" height="787" alt="image" src="https://github.com/user-attachments/assets/46380abf-9636-406a-a581-1280b80afa3f" />

After trying to move the PCB, the components on it didn't move along, so I tried reimporting the PCB, but that didn't fix it, so I decided that I'd have to only move the container instead

<img width="889" height="363" alt="image" src="https://github.com/user-attachments/assets/cc5aaaa4-1f59-4f06-9af5-aab04f26720f" />

Even after all this, there was still too much of a distance, so I had to shorten it

<img width="679" height="406" alt="image" src="https://github.com/user-attachments/assets/df53fc2c-82ac-479e-87a5-e9834b3b066f" />

I then finished the bottom part of the enclosure by adding holes for the screw head

<img width="820" height="594" alt="image" src="https://github.com/user-attachments/assets/ec8643e9-e960-49ed-8d09-9d32f67f8797" />

However, I was a bit concerned about how this might not necessarily be printable because of how there would be overhangs no matter which orientation (especially considering the USBC port, which should be printed face down, which would leave overhangs on the parts holding up the PCB)

<img width="1146" height="763" alt="image" src="https://github.com/user-attachments/assets/396e9ed8-6593-435f-8d42-774d7fe188c4" />

I decided to added another screw hole and have the front with the USB hole be a face plate

<img width="540" height="342" alt="image" src="https://github.com/user-attachments/assets/c2c9f564-c5e6-400f-9060-10f05aae387d" />

This does create one overhang on the bottom, but I believe it's fine since it's a circle (so less aggressive), and it's a heatset insert, so it really doesn't matter if it's precise at all

I'll probably replicate the plate on the back as well to keep a consistent design, but that's a problem for tomorrow

Overall, I realized how washed I am at CAD (it's been way too long) and also how difficult it is to come up with a custom design compared to following a diagram of somebody else's design (I had to thin way too long on how I would break up the enclosure)

**Total Time Spent:** 3.5 hours





# 6/27/26: Renders!

Turns out on many linux distros (like arch) blender is packaged to use the system python rather than the python blender comes with, causing the version discrepency. Thus, I reinstalled blender-bin via the AUR and was able to successfully render the PCB (took a LONG time to render, but not that long to find the AUR version)

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fded75e2-3c77-4cf9-a25c-e5565074e2a7" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e96b981c-7f1b-40cf-91c3-314434b981da" />


**Total Time Spent:** 10 minutes

# 6/26/26: Silkscreen & etc done

So... turns out that the impedance is actually affected by stuff being coplanar, which is an option not in digikey's calculator

This means that I would have to redo the impedance matched traces that have ground planes surrounding them, which means this one

<img width="586" height="444" alt="image" src="https://github.com/user-attachments/assets/8fedaf29-cbdb-4e9b-ae06-c25597d23ce2" />

and this one

<img width="283" height="609" alt="image" src="https://github.com/user-attachments/assets/2e1e7926-85bf-4d2b-91ea-6696657939a1" />

This means I need a MUCH smaller trace for both of these

<img width="1828" height="726" alt="image" src="https://github.com/user-attachments/assets/bb9900f7-421f-4f10-916b-63cf71cdb8f6" />

<img width="468" height="666" alt="image" src="https://github.com/user-attachments/assets/dc71ad48-f6c7-4b97-b34e-e38b0e5110a8" />

<img width="766" height="540" alt="image" src="https://github.com/user-attachments/assets/5b26956f-496b-4ff6-bd6f-bb692aa16f6c" />

Now it's time for the ~~not so~~ fun part of resolving all of these warnings and errors!

<img width="1113" height="690" alt="image" src="https://github.com/user-attachments/assets/b8a4c0d5-a52f-47f5-bb4a-29862037bc48" />

When there wasn't enough thermal spokes, I used traces to try and replace them because both of them are just copper

<img width="376" height="448" alt="image" src="https://github.com/user-attachments/assets/1d59295f-524a-46ff-859d-c908aac89846" />


As you can tell, a lot of the reference silk screen had to be deleted due to there just not being enough room

<img width="636" height="474" alt="image" src="https://github.com/user-attachments/assets/158ce8bf-7449-4a92-9ea0-fc5ece433ee5" />

And this is the finished product

<img width="702" height="712" alt="image" src="https://github.com/user-attachments/assets/e6ff9ed4-747f-4c03-a494-ca7bbda3a574" />

I then wanted to make a render, so I had to find these missing 3d models

<img width="555" height="717" alt="image" src="https://github.com/user-attachments/assets/2cf71957-178f-4a7d-8306-2918f44888bf" />

For some reason, the button manufacturer's website provides a model where the colors are all wack

<img width="492" height="444" alt="image" src="https://github.com/user-attachments/assets/8d5a5e16-8068-4ed4-a115-d8665a1e1320" />

In the end, mouser ended up being the goat for finding these models, and they made it really easy to download them right after searching for the part

<img width="694" height="216" alt="image" src="https://github.com/user-attachments/assets/739bb7ef-a759-4095-96e3-c9e4b286f86c" />

Anyways this is how it looks fully populated

<img width="502" height="690" alt="image" src="https://github.com/user-attachments/assets/50d44fa8-9cfc-4128-8962-ce9f84d4ffc2" />

And finally, I did some silkscreen decor

<img width="675" height="447" alt="image" src="https://github.com/user-attachments/assets/88b6f0e6-ca82-4962-b449-3555efa542b9" />

<img width="642" height="447" alt="image" src="https://github.com/user-attachments/assets/4bd01b0d-1b43-4939-b6fb-d7941eb936a1" />

I wanted to render this in blender using a plugin, but unfortunately the python versions don't match up

<img width="996" height="87" alt="image" src="https://github.com/user-attachments/assets/1634313a-61a9-4a67-97eb-9868fade9a1f" />

**Total Time Spent:** 1.5 hours


# 6/25/26: Done with PCB completely (excluding silkscreen)

I first started by finishing up all the connections for the remaining stuff that I set aside a while back

<img width="558" height="708" alt="image" src="https://github.com/user-attachments/assets/ef025e38-51df-4d17-abbf-a8581eebf2c7" />

When routing, this took quite a bit of time because there were multiple spots that were really conjested, like this

<img width="891" height="562" alt="image" src="https://github.com/user-attachments/assets/3d92e8e2-7af7-40e2-b0da-47ff8d686400" />

Following this, I used the DRC to mae sure I didn't miss anything major, and saw that there was an unconnected ground somewhere, but since the lines were really faint, it was difficult to see which spots specifically weren't connected

<img width="519" height="123" alt="image" src="https://github.com/user-attachments/assets/05bf90d9-b46d-4ea5-a0e6-285193fb9af1" />

<img width="466" height="339" alt="image" src="https://github.com/user-attachments/assets/f18b2975-824e-41ce-a23c-e8c11b1230ef" />

Then, I added teardrops, and there were multiple instances of it being really weird, so I had to go in and fix that

<img width="442" height="352" alt="image" src="https://github.com/user-attachments/assets/2a902d9a-8dc1-43de-971d-69b04ab49d1b" />

The next step would be to add screw holes, which were WAY bigger than I was expecting, meaning that I had to do a bit of restructuring on the top right one, but unfortunately I don't believe I would be able to fit one on the bottom part at all without having some of the screw head hang off to the side

<img width="985" height="591" alt="image" src="https://github.com/user-attachments/assets/fc656a72-0686-45e6-a9a9-3c8512281bfc" />
<img width="337" height="328" alt="image" src="https://github.com/user-attachments/assets/9b95edf5-d296-4f69-b654-e2152887cb5f" />

Finally, I decided to move the antenna way, way up because the battery is going to require about this much space (18500 li-ion w/ JST connector), making it probably better to have the antenna closer to the edge rather than in the middle ish

<img width="522" height="723" alt="image" src="https://github.com/user-attachments/assets/c3e81102-ef2e-4079-8ae7-2e6c560d9ddd" />


**Total Time Spent:** 1.75 hours


# 6/24/26: Nearly Finishing routing

First I realized that I didn't really add a button required to control between on/off and the two modes of operation nor did I add status LEDs, so I first did that before continuing to route

After I sourced my LEDs, I was having a bit of trouble about what resistor values I should use (and how close to the maximum I should get)

I then remembered this convo from a while back:

<img width="1312" height="654" alt="image" src="https://github.com/user-attachments/assets/7ab6ba3c-2df4-468b-86df-415c6131df09" />

So I'm probably just going to stick with 10k resistors

<img width="339" height="505" alt="image" src="https://github.com/user-attachments/assets/791b8bc8-546c-4791-94e3-75fa6b0197ec" />

I also wanted to find another footprint for the button (because THT 6mmx6mm is lowk pretty big, and I might as well go SMD)

Though, I think I'd also need to have a vertical button (this might have to be THT for more strength) because of how I want the final thing to look like


<img width="339" height="505" alt="image" src="https://cdn.hackclub.com/019efb62-fbb8-7a97-8816-002697022b45/20260624_164619.jpg" />

At least for the reset button I wanted it to look like the normal thin rectangular reset buttons that you'd see on something like an arduino nano, but even after adjusting the footprint parameters i kinda had difficulty finding the ones that looked like them and instead found stuff like this

<img width="417" height="570" alt="image" src="https://github.com/user-attachments/assets/de0e9372-4dea-414b-b49a-cb0f5567844b" />

<img width="181" height="198" alt="image" src="https://github.com/user-attachments/assets/446386ac-cd78-4351-a31d-e47bb9837341" />

In the end I figured it didn't matter too much and just ended up choosing to use the THT button for reset and a normal vertical one for the user input

And then immediately after I went to search for vertical button footprints already existing in kicad, I found footprints for exactly what I was looking for before, and used them to search for SMD buttons

<img width="976" height="871" alt="image" src="https://github.com/user-attachments/assets/c2f18547-1982-47d7-8f26-4775e23931bb" />

I then did the same with vertical buttons

As it turns out, they're actually called right-angled buttons, which helped speed up the search

I probably wouldn't have had an easy time searching for footprints for stuff like these if I started looking on JLC instead of on kicad

<img width="259" height="180" alt="image" src="https://github.com/user-attachments/assets/5f0f7962-0204-4ea8-872f-81b3f14b4615" />

It was pretty easy to then add these in to the PCB

<img width="649" height="352" alt="image" src="https://github.com/user-attachments/assets/485bb888-4db4-4a8e-a77d-e6c902fc77a6" />

<img width="541" height="382" alt="image" src="https://github.com/user-attachments/assets/13a80e6e-4894-44e8-9db7-ee37ca9a00e6" />

Then, I worked on finishing the antenna, starting with the layout of the capacitors and inductors before calcuating the width needed to get a 50 ohm impedance

The width needed ended up being insanely high, which was disappointing

<img width="1284" height="702" alt="image" src="https://github.com/user-attachments/assets/d2757b67-c02f-487c-a5f9-a3361790cbc3" />

It also resulted in it being pretty difficult to route (I ended up having to do dots as traces)

<img width="513" height="556" alt="image" src="https://github.com/user-attachments/assets/9f0d9c02-c7e3-4602-81fd-437393ecd573" />

After messing around a bit on the digikey calculator, ( found how why having more layers can be so important in a PCB (it makes it much, much easier to get lower impedances with a ground plane both above and below the trace)

Anyways, I nearly finished everything and resized edge.cuts to match the actual shape of the board

All that's left for the PCB is polishing (teardrops, screw holes, silkscreen [the front is gonna be a pain :C]) and the final connections (stuff like the LEDs and interrupts)

<img width="591" height="664" alt="image" src="https://github.com/user-attachments/assets/664aca9e-8c03-4a6c-a7c2-e27a9cdd73ab" />

**Total Time Spent:** 1.5 hours


# 6/21/26: Routed nRF52840 ('cept antenna)

I figured that the current spot would be a bit awkward to have a battery connector, so I decided to move it more towards the USB edge

I did have to reshuffle a bit though because of a small amount of overlap


![image](https://stasis.hackclub-assets.com/images/1782066295408-uy8ooj.png)

When rerouting, I noticed that this did interrupt the ground plane for pin 19 on the BQ25890H (the blue being the battery trace)


![image](https://stasis.hackclub-assets.com/images/1782067010655-k4ps6a.png),

But when I checked the datasheet, this pin didn't really require no noise to function (it's a switching node), so I just left it as is

Then, when working with the MAX chip, I realized that I forgot to add one of the capacitors in the schematic, so I quickly did so before moving on


![image](https://stasis.hackclub-assets.com/images/1782067553912-qgc8wy.png)

Other than that, routing this part was relatively simple


![image](https://stasis.hackclub-assets.com/images/1782067720717-pimcts.png)

And it also seems that it fits in just like a puzzle piece (which was pretty satisfying)


![image](https://stasis.hackclub-assets.com/images/1782067750855-5qd9v3.png)


The nRF posed no difficulty and it was pretty easy getting it done. However, it was really annoying having to go back and forth from the data sheet to check which pin has which capacitor (since some VDD pins have a different amount compared to the others)


![image](https://stasis.hackclub-assets.com/images/1782069364215-qdc9a8.png)

I can already tell that this part is going to be pretty difficult to route because of the small space, but it should be doable


![image](https://stasis.hackclub-assets.com/images/1782069694485-4fim9z.png)

To make this take less time, I decided that I would start by fanning out the connections, but alas, I had to move some stuff


![image](https://stasis.hackclub-assets.com/images/1782070943866-px78f4.png)

Before continuing, I had to check the nRF datasheet to see which pins could be used for what functions, but they seem completely flexible


![image](https://stasis.hackclub-assets.com/images/1782071841093-7h44gm.png)

However, upon looking further, it seems some pins are better suited for stuff like SPI than others


![image](https://stasis.hackclub-assets.com/images/1782072094320-z5fasu.png)

While routing, I decided to add these little ground paths to make sure that the traces aren't coupled (shouldn't be a problem either way since it isn't that high speed, but whatever)


![image](https://stasis.hackclub-assets.com/images/1782074417499-zghgao.png)


...and after doing this i realized that I forgot to move the nRF down (look at all this extra space!)


![image](https://stasis.hackclub-assets.com/images/1782074728866-z212wd.png)

Anyways, this is how it looks once I moved it down (and squeezed everything in there)


![image](https://stasis.hackclub-assets.com/images/1782075736629-nc2c25.png)

**Total Time Spent:** 2 hours

# 6/20/26: More Routing ([mostly] everything power is done)

Looking back at yesterday, I noticed that the distance between the groundplane/traces was really big, and I believed JLC could handle higher precision, so I went on their website to see if it was possible


![image](https://stasis.hackclub-assets.com/images/1781977509373-zedutv.png)


![image](https://stasis.hackclub-assets.com/images/1781977624054-p66xqa.png)

What was kinda weird was having to go into the GND plane settings instead of going into board settings to change this clearence, which took a while to find

As I continued, I noticed that the battery and mux have swapped USB pins, but it should be fine to use a via and cross them because of the short distance & relatively low speed


![image](https://stasis.hackclub-assets.com/images/1781978833087-ofrxwe.png)

However, it was really annoying to get around kicad telling me I can't start a trace here

![image](https://stasis.hackclub-assets.com/images/1781979282271-lm4nuf.png)

After finally being able to make the trace (and with some goofy length matching) this is the result


![image](https://stasis.hackclub-assets.com/images/1781979800529-7ewrz1.png)



Since this design needs to be able of handling up to three amps... enjoy the very big power trace


![image](https://stasis.hackclub-assets.com/images/1781980142096-dbz9rw.png)

Then I did a lot of the stuff related to power

Since this is all DC stuff, I didn't really worry too much about signal n stuff and instead focused on trying to make it as compact as possible


![image](https://stasis.hackclub-assets.com/images/1781982241550-uz3xpj.png)


![image](https://stasis.hackclub-assets.com/images/1781983528571-5gfwn0.png)

I decided to add a power branch to the right side whenever I needed power to avoid having to go all the way back to the vreg


![image](https://stasis.hackclub-assets.com/images/1781983904230-rhjmli.png)

Doing the CC control part was pretty straightforward


![image](https://stasis.hackclub-assets.com/images/1781984465430-jg8d0e.png)

Though I really love how compact this is going to be


![image](https://stasis.hackclub-assets.com/images/1781984515962-94xep7.png)

**Total Time Spent:** 2 hours

# 6/19/26: Started Routing

First, I cleaned up my schematic based on various feedback to make it easier to read/look nicer

This took a while, but it 100% made some parts of the schematic look much neater


![image](https://stasis.hackclub-assets.com/images/1781896143438-tduwn5.png)

Then, when I moved on to routing, I noticed that the ground pad for the nRF showed that it wasn't part of a net, so I went on to check the custom symbol I made

I didn't see how there was any problem at first, but turns out for two different pins to be a part of the same net, having the same name isn't enough and they have to be overlapping


![image](https://stasis.hackclub-assets.com/images/1781898253962-es0a7p.png)

As I was setting up a vague layout for the PCB, I discovered that the footprint for the USB mux really sucks, making it difficult to route the two USB pairs


![image](https://stasis.hackclub-assets.com/images/1781899109291-pqvm4f.png)

So... I had to find a new one before moving on

I quickly found the TMUXHS221, and decided to use it since it had a really similar symbol (so I could copy and paste essentially)


![image](https://stasis.hackclub-assets.com/images/1781900709879-e1x86h.png)


Then, I found out that the D+ and D- input were swapped on the footprints, which makes this a lot more painful


![image](https://stasis.hackclub-assets.com/images/1781900975842-e7mc0j.png)

This also means that I have to redo this process again...

I found the TS3USB3031, made it's symbol, and replaced it in the schematic


![image](https://stasis.hackclub-assets.com/images/1781902153647-7ybdb2.png)

I started making a draft layout, and then started with the USB differential pairs... and yeah this width is pretty unreasonable to do in a tight space (and I rather not use 1.1mm trace width)


![image](https://stasis.hackclub-assets.com/images/1781905121085-pay6q7.png)

Since for the small distance I'm using, however, I'm just going to make the trace as big as I can without worrying about it too much

Also did a bit of the other parts for the routing, making it as compact as possible

![image](https://stasis.hackclub-assets.com/images/1781906784036-n03kx9.png)

And this is the general draft layout (will squish together by the end)


![image](https://stasis.hackclub-assets.com/images/1781906851518-1hf6e5.png)

**Total Time Spent:** 1.75 hours

# 6/18/26: Finished Schematic!!!!!!!

School is finally over, so I have a lot of more time to dedicate to finishing this project.

First thing's first, I looked over the previous journal entry and rediscovered that I wanted to add ESD and short protection.

However, the part I chose last time did not have a footprint in kicad, so i did a very quick search and ended up finding the TPD6S300A, which is also available on JLC


![image](https://stasis.hackclub-assets.com/images/1781810606425-pv9wai.png)

When looking at its documentation, I got a bit confused because of the mention of a "dead battery" mode


![image](https://stasis.hackclub-assets.com/images/1781810654847-go56vl.png)

But it turns out that this is just to allow charging when the battery is completely discharged

It did require dead battery support on the CC controller, so I went back and double checked the documentation on that end, and it turns out that it does have it (so no more reworking for me!)


![image](https://stasis.hackclub-assets.com/images/1781810720950-fcu6uh.png)

Anyways, it was pretty quick in adding connections after that and there weren't any difficulties


![image](https://stasis.hackclub-assets.com/images/1781810863144-set0b6.png)

Although, I did almost forget the ESD protection on the VBUS pin, so i just used the recommended part from the USB protection article by TI from before for 20V


![image](https://stasis.hackclub-assets.com/images/1781811364522-oiv7km.png)


Now for the final part, the MAX usb host controller (and then I think that should be it for this board)

Since there was no pre-existing symbol I could use, I ended up making my own, which was pretty straightforward


![image](https://stasis.hackclub-assets.com/images/1781813201408-dkh3ri.png)

As I was adding the connections, I had to source a 33 ohm resistor for the USB data pins, which was no problem

When getting to the crystal, there was not enough space towards the left to add the capacitors, so I spent a bit of time shuffling around the components for the nRF to get a bit more space

Anyways, this is the final result:


![image](https://stasis.hackclub-assets.com/images/1781815630893-symkpm.png)

And this is the entire schematic (I added the SWD pins, but not significant enough to really mention):


![image](https://stasis.hackclub-assets.com/images/1781816795024-akkc29.png)

**Total Time Spent:** 1.75 hours

# 5/16/26: CC control

I first refreshed myself with the previous journal entry (it's been a while, but now im back!) and reskimmed through the documentation quickly to refamiliarize myself with what I need to do

I then started the schematic part on the CC controller, which luckily already had a kicad sym built in


![image](https://stasis.hackclub-assets.com/images/1778980330754-pd7qd1.png)

Do gotta source a 900K ohm resistor for the VBUS_DET to VBUS, but that shouldn't take long at all

Turns out there isn't an exact 900k option, so when going to the electrical characteristics, I found that 887k is what's usually used instead


![image](https://stasis.hackclub-assets.com/images/1778980531268-6whko0.png)

As I was finishing up the part of the schematic for the CC controller, I decided to rename the I2C and int pins to be more unique, so I would be able to tell then apart


![image](https://stasis.hackclub-assets.com/images/1778981777577-6znh4p.png)


![image](https://stasis.hackclub-assets.com/images/1778981801854-zermxg.png)

ANYWAYS... I believe all that's left for the schematic is the USB host controller and the actual USB port itself

I was getting kinda tight on space, so I cleaned up my schematic a lot and made it look actually good & organized


![image](https://stasis.hackclub-assets.com/images/1778982398272-huejwi.png)


I went to source the USB C receptacle, and started by looking at the JLC parts library

This turned out to be a mistake because it's 100x better to start by looking at the footprints given in kicad and going from there (to avoid having to potentially make my own)

I ended up going with this guy:


![image](https://stasis.hackclub-assets.com/images/1778983826584-tn0g0a.png)

which came with a pre-existing footprint


![image](https://stasis.hackclub-assets.com/images/1778983850941-4xahed.png)


I then researched on what the SBU pins were for


![image](https://stasis.hackclub-assets.com/images/1778984019142-nvmkk8.png)

It seems that they're for USB alt mode, which I won't be needing in this project

![image](https://stasis.hackclub-assets.com/images/1778984129906-ga1da1.png)

When doing the connections for the ground/shield portion, I do remember something about some people using a ferrite bead, but I don't remember why, so I went ahead and researched what people do with shield

According to a hackaday article I found, it turns out that it should just be connected to ground, so that's what I'll be doing


![image](https://stasis.hackclub-assets.com/images/1778984509625-xk3iab.png)

Before I forget, I wanted to make sure to add ESD protection. While I already know that TVS diodes are usually used, I wanted to make sure that's all I needed (since it's been a while since I made my last PCB) and found this [article by TI](https://www.ti.com/lit/an/slvaf82b/slvaf82b.pdf?ts=1778898998494&ref_url=https%253A%252F%252Fwww.ti.com%252Fproduct%252FTPD2EUSB30)


![image](https://stasis.hackclub-assets.com/images/1778986570572-uwunfl.png)


This part was a bit confusing, but I believe it's telling me to use a diode that will not break down at the voltages from VBUS

The problem with this is that it seems the TVS diode won't breakdown until that voltage under a normal ESD event (and I don't think they're meant for longer duration spikes)

I decided to get a TI part to resolve this problem and sourced the TPD4S201, especially since it also allows me to have ESD protection for the data lines (since I don't need SBU)


![image](https://stasis.hackclub-assets.com/images/1778987656344-pgrsr4.png)

**Total Time Spent:** 1.75 hours


# 5/5/26: schematic, post-nRF

So, regarding planning for how I'm going to do the two boards (since one for tx, one for rx):

I was initially going to use a vcut or mousebites, but this constitutes as multiple designs according to JLCPCB and costs extra

I also realized that if I were to do this, I would have to switch over the nRF that I would be using to the aqfn footprint, which is much harder to route (to save on another $3 extended parts fee)


![image](https://stasis.hackclub-assets.com/images/1778029677128-o41lk1.png)


In the end, I decided that I would just do the boards separately, and cuz why not, I'll be manually soldering the tx board (and maybe fail?)

This also means that I'm no longer limited to basic/preferred parts, so I started by replacing the parts that could've been better selected (and 0402 package size cuz i already have a hotplate)

Anyways this took a while since I also changed the footprints on the existing components (though I guess next time it might be better to just assign the footprints and labels for part # afterwords, contrary to what I thought before; it'd be helpful if I ever need to change stuff)


![image](https://stasis.hackclub-assets.com/images/1778031953922-s8ryn7.png)


![image](https://stasis.hackclub-assets.com/images/1778031975541-bdohe9.png)


![image](https://stasis.hackclub-assets.com/images/1778031986863-ww3005.png)

Also, when looking at the nRF documentation, the pins for i2c are able to be changed in the registers thingy


![image](https://stasis.hackclub-assets.com/images/1778032225020-gwn9nm.png)

This means that it'd be best to choose which pins these guys route to afterwards (though I'll keep labels near the nRF to remind me later)


![image](https://stasis.hackclub-assets.com/images/1778032538297-j71wr6.png)

Now onto the MAX usb host controller!!! (and the final step of this board!!!)

I actually didn't check completely if this would be able to support having different voltage inputs in USB charging (idk if the CC pins must be configured correctly for that) or if it says it'll only be able to provide 5V via CC pin pulldowns, so that's what I did first

When I saw this:


![image](https://stasis.hackclub-assets.com/images/1778033054401-4glv1p.png)

I thought it'd be a good idea to check if the PMIC i'm using has a way to limit the output current during usb OTG mode (and it ended up having one, with the min being 500mA)


![image](https://stasis.hackclub-assets.com/images/1778033102991-5nyc45.png)

Anyways, the MAX chip appears to have to connections to the CC pins, so I'm going to have to research how a host/charging device would use them (if at all?)


![image](https://stasis.hackclub-assets.com/images/1778033527053-suw3jc.png)

I then learned that I should most likely include something to manage this after reading: https://nodeloop.org/guides/usb-c-pd-hardware-design/


![image](https://stasis.hackclub-assets.com/images/1778033916182-ykts7m.png)

![image](https://stasis.hackclub-assets.com/images/1778033842858-halxdf.png)

So time to find another part!!!

I came across the TUSB320LAI, which only handles CC control, which seems perfect for incorporating with the MAX chip

![image](https://stasis.hackclub-assets.com/images/1778034271615-jgzvjr.png)

Also skimmed through the document, and it doesn't seem too complicated to use, at least compared to the other register stuff I've seen already from other components in this project (what truly scares me is programming the nRF & the MAX chip)


**Total Time Spent:** 1.5 hours

# 5/4/26: Finished nRF (independant of other parts)

Turns out a crystal is a passive component while an oscillator builds upon that and is an active component. For the nRF I'll be using a crystal

Sourcing it took a bit of time, especially because of the parameters I had to check, such as maximum shunt capacitance, ESR, etc., but I was able to find one

I also looked through the documentation to see what would happen if I don't use an external ~32kHz crystal for the timing, and it seems that it can be more efficient with power (sacrificing accuracy)


![image](https://stasis.hackclub-assets.com/images/1777944680377-q7ykm6.png)

The only thing I am a bit concerned about is parasitic capacitances in the traces, so I started doing some research on how I would be able to account for it, but the best way to do so seems to be acknowledging it during the routing process

After I looked a bit closer at the reference schematic though, I saw that nordic gives 2pF lower load capacitance to compensate, so I'll be doing the same


![image](https://stasis.hackclub-assets.com/images/1777945335469-y7thrv.png)

Now for the antenna, there were two types of symbols that I might choose, either dipole or just the antenna symbol. I also decided that I would look at the antenna footprints now, so I'd know what I'm doing somewhat later down the road.

Since I've never really done an on-board antenna, this is where I turned to the internet.

I looked at https://jlcpcb.com/blog/pcb-antenna-design-guide

However, I was still a bit confused on how I would get the antenna to to properly matched to the frequency I want (2.4GHz)

I then realized that there was already a footprint for 2.4GHz, meaning I don't really have to do much work


![image](https://stasis.hackclub-assets.com/images/1777946394836-ozkwzt.png)

When trying to source the 1.2pF capacitor required, there was none under basic/extended preferred, so I just plugged in numbers to see if I could make one using two other ones in series. I would be able to use both the 1.5 and 6 pF capacitors to get the 1.2 pF required


![image](https://stasis.hackclub-assets.com/images/1777946888352-nkij09.png)


When sourcing the inductors required, I saw that the JLC basic/extended preferred parts for inductors at the nH range were just crap, so I'm basically forced to use extended

![image](https://stasis.hackclub-assets.com/images/1777947159215-9bbz8e.png)

Anyways, that took a while, but here we are! Hopefully I remember to impedance match the trace going to the antenna later on


![image](https://stasis.hackclub-assets.com/images/1777947740690-3ro78o.png)

This honestly took way longer than expected, but at least I'm now set up for adding connections to other components now. (All that's left after that is to add the USB host controller/USB-C and practically copy/paste the nRF circuit on a board attached with a vcut to get the USB dongle)

**Total Time Spent:** 1.25 hours

# 5/4/26: Started on the nRF

First I checked over my symbol for the nRF52840 to make sure everything was good (I did not trust the me who made the symbol way back when). Luckily everything seemed to be fine


![image](https://stasis.hackclub-assets.com/images/1777933231363-5xvkp9.png)

I started with all the VDD pins and their decoupling caps, having to source 100nF


![image](https://stasis.hackclub-assets.com/images/1777933767295-wutuwv.png)

Then I moved on to all of the caps for the DEC pins, deciding to put them near the decoupling caps for the VDD pins to make the schematic neater

During this process I had to source a 100pF cap

Some of the DEC pins were missing, causing me to double check with the documentation, but the pins weren't there either, so I'm assuming it has to do with the lower pin count of the footprint I'm using

Anyways here is the nRF with the DEC pins done


![image](https://stasis.hackclub-assets.com/images/1777934313043-8w3cbv.png)


![image](https://stasis.hackclub-assets.com/images/1777934324745-om5j8r.png)


I then focused on the DCC pin, which required a lot of inductance (and required me to source two inductors)

Unfortunately the 10uH inductor must be able to handle 50mA, and JLCPCB doesn't have those under extended preferred or basic components

Either way, this didn't take too much time, and I was able to easily finish


![image](https://stasis.hackclub-assets.com/images/1777935233877-9w65ak.png)

At this point, I believe all that's left for the nRF is the antenna, XTAL, and the routing to the other components for control

I was going to start sourcing the mandatory crystal on JLC, but I then say that there were two categories, one called crystals and the other called crystal oscillators

I don't know the difference yet, but that'll be for the beginning of next time


![image](https://stasis.hackclub-assets.com/images/1777935699890-qby5zv.png)

**Total Time Spent:** 50 minutes

# 5/1/26: Voltage regulator schematic

First, I made a symbol for the voltage regulator. This was real fast, especially compared to the other symbols because of a small number of pins and due to already having lots of practice


![image](https://stasis.hackclub-assets.com/images/1777674394746-wt00y5.png)

Also had to do some calculations to determine what value of resistors to use
![image](https://stasis.hackclub-assets.com/images/1777674988413-roc8kb.png)

I initially decided to use a 91k and 510k ohm resistor, but the only 91k ohm resistor requires a minimum purchase of 5,000 of them, so I had to choose different values


![image](https://stasis.hackclub-assets.com/images/1777675435366-bs5oi4.png)

I then decided to go with 82k and 430k + 30k series (460k) to get 3v3 since there's a minimum of only 1

After doing a bit of part sourcing for the resistors and a capacitor, I quickly finished this part of the schematic (luckily was able to copy and paste some components I already used in the schematic)


![image](https://stasis.hackclub-assets.com/images/1777676891632-a7y7sk.png)

![image](https://stasis.hackclub-assets.com/images/1777676907818-71ffxc.png)


![image](https://stasis.hackclub-assets.com/images/1777676921948-lcyhzj.png)

**Total Time Spent:** 53 minutes

# 4/24/26: Actually started the schematic
I decided that I would go along with using the BQ25890H because after asking around yesterday, it seemed that the "minimum" amps referred to the minimum that would be supplied given a certain charge.

So I created a symbol and started the routing for it


![image](https://stasis.hackclub-assets.com/images/1777037849148-6r0gbw.png)

After getting to the ILIM pin, I had to do some research on what is a safe current to charge a lithium ion battery at, determining that it should be at most the capacity in amps


![image](https://stasis.hackclub-assets.com/images/1777039139546-26vkb0.png)


Since this could vary depending on the lithium ion battery I eventually choose, I decided to be very lenient, giving the near the maximum allowable current (since I could always limit it in firmware with the registers). After doing the simple calculation, this meant I had to use a 100 ohm resistor

As I continued, I realized that I don't know whether the part footprints are in metric or imperial, so I went back and double checked, and it seemed that they were in imperial, so I had to go back and change the footprints of the parts already placed

As I was sourcing a 4.7 uF capacitor, I had to decide whether I should accept a 20% tolerance or a 10% tolerance (with 20% tolerance being a smaller capacitor). I eventually decided to go with 10% for stability


![image](https://stasis.hackclub-assets.com/images/1777041418584-8wehdq.png)

I then got to the part with the thermistor pin, and I looked to see if there was a way to disable it since it is very unlikely for the battery to get to high enough temperatures for it to be dangerous. However, there was not, so I had to find the part where I do the calculations to set the temperature range.

The problem here is that I had to know what type of thermistor the battery would be using. After scrolling on aliexpress for a while, I found that vendors don't typically list this information

After spending some more time looking, I still couldn't really find anything, so I decided that an external thermistor close to the battery would have to do and copied the resistor values that TI used (0 to 60 degree c range)


![image](https://stasis.hackclub-assets.com/images/1777043513914-cn9eks.png)


![image](https://stasis.hackclub-assets.com/images/1777044037184-f0a6hf.png)

Then, I finished up the schematic for the PMIC and found a USB mux that I'd be able to use


![image](https://stasis.hackclub-assets.com/images/1777045134335-mulzbv.png)

I quickly found the TS3USB30ERSWR, and luckily it already has a symbol in kicad for me to use, allowing me to quickly finish routing this part


![image](https://stasis.hackclub-assets.com/images/1777045667426-bz2fkt.png)


![image](https://stasis.hackclub-assets.com/images/1777046039086-1t4qwq.png)


And here is the parts list that I've been maintaining


![image](https://stasis.hackclub-assets.com/images/1777046065962-a14i9e.png)


![image](https://stasis.hackclub-assets.com/images/1777046078384-zumwmz.png)

**Total Time Spent:** 3 hours


# 4/23/26: symbol for PMIC

Now that I knew what to look for (the application guide), making a symbol was going much faster


![image](https://stasis.hackclub-assets.com/images/1776952251702-nlyn8y.png)

However, I got a bit confused when seeing that the PGND pin seemed to have two different grounds. Even though I haven't started the schematic yet, I decided it was still something good to know


![image](https://stasis.hackclub-assets.com/images/1776952308326-ksved4.png)

So I asked around on the kicad discord, and finished up the symbol while I was waiting, eventually learning that the difference is between analog ground and power ground, where power ground is usually more noisy than the analog ground used as a reference point


![image](https://stasis.hackclub-assets.com/images/1776954120120-4xbx2z.png)

I started the routing and initially put the pull-ups and pull-downs near the schematic, but I decided that it would look cleaner to separate them


![image](https://stasis.hackclub-assets.com/images/1776956558699-oaxfri.png)


When working on the SDA, SCL, INT pins, I realized that there was no symbol for Vref, so I went through to find what voltage the nRF chip communicated in I2C, which turned out to be whatever voltage I would be supplying it (3v3)


![image](https://stasis.hackclub-assets.com/images/1776956815408-817b5b.png)

I then got confused on what the PHY meant

![image](https://stasis.hackclub-assets.com/images/1776957559513-1rucil.png)

Turns out that it's the part that communicates with the USB power supply, and I figured that i could use the MAX3421E for that rather than keeping it off during charging. After trying to confirm with the datasheet, there wasn't anything I found relating to PHY/selecting for power. This meant that I'd need two more chips (USB mux & usb phy). 

After searching for a new PMIC, i found the bq24295, but strangely, there's a minimum current, which doesn't really work well with wired peripherals that are generally designed to be low power.

![image](https://stasis.hackclub-assets.com/images/1776958633121-0fh4ze.png)

I then found the bq25890h which is quite literally perfect in pretty much every single way (USB implementation, can supply SYS with only a battery, it even has a pin to control a USB mux), BUT it still has the weird minimum current thing at a smaller 500mA (but still pretty big)


![image](https://stasis.hackclub-assets.com/images/1776959769222-s3yxi4.png)

However, there's still hope since it does say typical range, so I'm going to ask around to see what happens if a device would demand less current than the typical minimum

P.S. because of all these changes I did decided to completely scrap the routing I already had

**Total Time Spent:** 2.5 hours

# 4/22/26: Power IC

A kind soul in the Kicad discord server drew me a diagram of how the boost mode would work, sending current through the charging port.


![image](https://stasis.hackclub-assets.com/images/1776867001648-gqpvxb.png)

The fun part is I can't really use this PMIC. In the process of trying to learn the power path, I stumbled upon this part of the documentation


![image](https://stasis.hackclub-assets.com/images/1776867041987-wdh1da.png)

This means that just having a charged battery does not mean i can get 3V3 (or really close to it for efficiency) power, which kind of defeats a large point of having a battery

I then stumbled upon bq25898D which has all the same features BUT with only the battery being enough


![image](https://stasis.hackclub-assets.com/images/1776867387796-d6ktqr.png)


Unfortunately, the part isn't really in great stock for JLCPCB and is quite expensive


![image](https://stasis.hackclub-assets.com/images/1776867439207-ja02ft.png)


The awesome part, however, is that i then found the bq24259 chip, which, again has all the requirements---but also for a much cheaper price with a lot more availability


![image](https://stasis.hackclub-assets.com/images/1776867705688-qnwf1f.png)

What's even better is that I don't need a USB mux anymore for identification between the PMIC and the nRF chip

Overall this search took about an hour, looking through many TI parts and analog devices parts, but now I'm finally ready to move on and continue the schematic

**Total Time Spent:** 1 hour

# 4/20/26: Refreshed myself over the documentation/pinout

So it's been a while because I've been busy recently, so I decided to make sure I wasn't being stupid earlier, and turns out I was.

I didn't have a proper connection to a 5V OTG output, so I looked at the datasheet and had trouble determining what pin would be getting the 5V when in boost mode


![image](https://stasis.hackclub-assets.com/images/1776694411764-ac25zy.png)

So I asked around on the kicad discord for help

I also double checked some some of the components to make sure they could actually handle the voltage the pins could have, and I decided to assign the footprints/add a part number to the parts now


![image](https://stasis.hackclub-assets.com/images/1776694523787-vrvfb8.png)

**Total Time Spent:** 35 minutes


# 3/7/26: Completed nRF symbol, started routing

I finished the symbol for the nRF52840 varient that I would be using pretty quickly, and then started routing.

<img width="813" height="663" alt="image" src="https://github.com/user-attachments/assets/b78b24f4-3fde-4473-b57b-5aca48c47306" />

However, after I double checked to make sure that the power from the battery would be adequate, I realized that the nRF QFN variant does not have the VDDH pin (so I would be limited to 3V3 rather than being able to supply 4.2V at full charge from the battery)

This meant I unfortunately had to restart the routing that I did start, and use the built-in symbol, and I was able to finish routing the power.

<img width="1008" height="437" alt="image" src="https://github.com/user-attachments/assets/8aa37fbd-7c76-40fb-ba99-4dbc7364dd45" />


I then double checked to make sure that the MAX usb host controller would be able to handle up to 4.2V, but then saw that it could only handle from 3.0-3.6V. I did some thinking to determine what would be the best path moving forward. I came to the conclusion that it would be best to either scrap the PMIC circuit entirely, or instead use an LDO to drop the voltage to 3V3, depending on which would be cheaper or more efficient. Right now I believe that adding an LDO would be the best option, especially since the $3 extra loading fee for having 3 components (charge [might need an LDO], boost to 5V, drop to 3V3) would probably add up to be more.

However, I'll be reusing my own symbol for the nRF52840 variant because it has a footprint that's easier to route, and I wouldn't really need the VDDH pin if I could directly supply 3V3.

**Total Time Spent:** 1.3 hours



# 3/4/26: Started work on the nRF

I started with importing the nRF52840 chip (which had a given footprint and symbol), and then I proceeded to look at the documentation for the nRF52 chip. What surprised me however was how there was 600+ pages of documentation all for this one chip (I only read the description before). Most of it seems to just be on the firmware implementation for the chip, luckily (for now).

What I did find surprising though was how Nordic Semicon gives a full copy of the PCB implementation, with all the values for external components neatly in one place (which should make making the schematic a breeze, I hope)

<img width="1115" height="806" alt="image" src="https://github.com/user-attachments/assets/53bb78ea-1d3a-4563-b090-6e7db4b9fc7f" />

However, I then realized that the different packages for the nRF52840 have different numbers of pins. Unfortunately, the footprint for the nRF52840 was a different one than the one I would be using (QFN for ease of routing). Additionally, the pin numbers were wrong, which meant that I wouldn't really be able to use it and the QFN footprint together. Thus, I decided that I would just have to make my own symbol.

With the rest of the time in this session, I started adding all the pins (and their corresponding pin numbers) as well as double checking them to make sure they were correct and then sorting them based on function. At this point, I realized that I forgot to double check the pins on the PMIC symbol I made, so I quickly did that as well this session.

<img width="862" height="633" alt="image" src="https://github.com/user-attachments/assets/e2584047-a0ce-49b1-add1-0e0bfb08dd01" />

**Total Time Spent:** 1.1 hours



# 3/3/26: Found USB mux, other components, and finished connections for power

Started off this session with finding a USB mux as I said I would yesterday, and I settled on the FSUSB42

Luckily, this datasheet was ***so much easier to read*** so I was able to integrate it into what I previous had without any difficulties.

<img width="442" height="393" alt="image" src="https://github.com/user-attachments/assets/ab54d715-cf22-4c23-9f11-6d536d012f54" />

As usual, the TI PMIC was still pretty confusing, but since I've read it multiple times through at this point, I feel like it's a lot more understandable. What took me the most time to figure out while routing the power for this chip was whether the VBUS pin can both be used as an input (for charging the battery) and as an output (at 5V to supply the device)

Anyways, I was able to completely finish routing the power portion of the PMIC, and I'll be able to start routing the nRF chip soon (which would also be when I route the I2C and the rest of the pins for the PMIC that relate to CTR)

<img width="636" height="612" alt="image" src="https://github.com/user-attachments/assets/a0faa2eb-44fe-42a2-b2ad-9151c26d1c3a" />

Finally, I sourced all the components that I used on the JLC parts library (making sure to use basic/extended preferred to avoid the loading fee)

<img width="268" height="200" alt="image" src="https://github.com/user-attachments/assets/9094d7ce-3a02-4469-b296-0c9402cbbe0b" />

**Total Time Spent:** 1 hour

# 3/2/26: Made symbol and started schematic portion for PMIC

I decided a better way to go about things rather than just jumping in, which would be to start from the source of power and work my way outwards from that. This meant I would start from the battery connector and then work my way through the system (where the natural next step would be the PMIC circuit).

Since there was no symbol for the PMIC I'm using in Kicad, I had to make my own one. Learning from yesterday's failure, I made a footprint that looked much nicer (but took quite a bit more time to create)

There were still some parts that I didn't fully understand about the PMIC chip, but I was still able to generally group pins based on their functions.

<img width="577" height="368" alt="image" src="https://github.com/user-attachments/assets/cc0506ca-0adb-43b9-b9fc-f8bf34abf97b" />

Afterwards I got started on the routing part, starting with the power. When I ran into the D- and D+ pins, I got a bit confused on how I would route them to both the MAX host controller and the PMIC while avoiding both of them using the lines at the same time. However, I realized that the battery would only be charging when not in use, and I could just keep the MAX chip off by default. (Though I would still have to find a MUX)

<img width="976" height="709" alt="image" src="https://github.com/user-attachments/assets/ad48248c-9d76-47b8-9b0e-3798007aee96" />

**Total Time Spent:** 1.2 hours



# 3/1/26: Chose a PMIC & began schematic

Obviously the first thing to do for this session would be to finish up what I was working on yesterday, which was sourcing a PMIC for the project. After reading the documentation for BQ25611D, I looked at other options on the JLCPCB parts library, and most of the documentation there was pretty mid compared to TI. 

Then, I started gathering the part numbers for the parts I'd be using

And finally, finally started the schematic

The only problem was I couldn't really find a premade symbol and footprint for the MAX3421E, so I decided I'd make my own. Since I hadn't made anything PCB related since summer, I was quite rusty. I literally put the pins inside out, then painstakingly flipped each of them, only to forget that making pins that aren't needed (like the thermal pad underneath the chip) invisible was a feature. This resulted in a symbol that looks pretty horrendous 



<img width="429" height="411" alt="image" src="https://github.com/user-attachments/assets/53cbe568-47fa-4e93-b277-bb2ce8d16c56" />


I finally decided to search online, and lo and behold, the [first result](https://www.snapeda.com/) was the footprint and symbol I needed. 

Well lesson learned for next time... I guess

P.S. Just decided this after posting this journal entry. I guess I'll practice making symbols since it's good for experience, but I'll 100% start from scratch to avoid this mess

**Total Time Spent:** 1.4 hours



# 2/28/26: Tightened design goals & research battery circuits

So... I may have wanted to include both a USB C and USB A receptacle on the receiver, but I decided that [this](https://www.youtube.com/watch?v=Fj0XuYiE7HU) would be against making the device user friendly by suggesting that both ports would be able to work at once (which wouldn't be the case). I decided to just go with USBC because USB-C to A dongles aren't too uncommon.

Following this, I watched this video to learn a bit about battery management circuits and what I need to create something safe. I stumbled upon a TI PMIC, and then skimmed through the datasheet

<img width="722" height="398" alt="image" src="https://github.com/user-attachments/assets/f6bf59b1-8655-481a-8e2e-7ab5aad05650" />

(Also found a suitable USB host)

**Total Time Spent:** 1.2 hours


# 2/27/26: Came up with the idea & initial research

**Man, don't you just hate how so many devices are wired instead of wireless? Well, I sure do.**

The idea is simple in concept, have two separate modules: one for acting as the host and one as the dongle while keeping optional BT LE support.

For the most part this session was just fleshing out the idea to the features that I want to include. After I created a general map, I did quite a bit of research on decent 2.4GHz+BT LE MCUs, and I found that the nRF52840 would work the best. However, there needs to be a USB host controller because as far as I know, the nRF52840 can only act as a USB device.

<img width="765" height="713" alt="image" src="https://github.com/user-attachments/assets/3a91d6bb-35e5-4b2c-9949-a1f43d2ddd46" />

**Total Time Spent:** 1 hour
