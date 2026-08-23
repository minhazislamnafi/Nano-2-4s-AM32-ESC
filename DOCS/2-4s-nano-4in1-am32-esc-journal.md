# 2-4s Nano 4in1 AM32 ESC  — Journal Export

- Exported at: 2026-08-23T20:19:46Z
- Project ID: 1885
- Entries: 22

## Entry 1
- ID: 1891
- Author: NAFI
- Created At: 2026-04-12T09:48:39Z

### Content

I started this project, but don't dont know why ;) This will be a 4-in-1 esc. oh! I can use this in my HACK FLY drone. The drone will be fully custom-made.

First, I go to the AM32 documentation and find that it works with many MCUs. So I need to select one.
![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyNywicHVyIjoiYmxvYl9pZCJ9fQ==--408ef51c4233c931afef680a6b71de65fa554c8b/image.png)

After some research, I chose AT32F421G8U7 because it comes with a QFN-24 package. the smallest of them. 

I also need all of the components to be as small as possible. My PCB size budget is only 25*25mm.

At first, I want to use a 2*2mm size n-channel MOSFET, but those are not available on Aliexpress. So I switched to 3*3mm
![Screenshot 2026-04-12 152702.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyOCwicHVyIjoiYmxvYl9pZCJ9fQ==--8b2c469fa369779855d54bd8a8c0ab7faceb6cd9/Screenshot 2026-04-12 152702.png)
 I also used a very small gate driver, DVR8300N(also QFN-24)
![Screenshot 2026-04-12 152627.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAyOSwicHVyIjoiYmxvYl9pZCJ9fQ==--9c7a23fecbb319b5e72996c8b44b6af77c76fefc/Screenshot 2026-04-12 152627.png)
After placing the main ICs, I routed some connections in the schematic. That's it.
![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDAzMCwicHVyIjoiYmxvYl9pZCJ9fQ==--de187f309a13e24c6b2c5d031433fabaa065bc49/image.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/Joe-1cWgr59x/timelapse-Joe-1cWgr59x.mp4

## Entry 2
- ID: 1953
- Author: NAFI
- Created At: 2026-04-12T20:36:31Z

### Content

Just completed the schematic single ESC. 
![Screenshot 2026-04-12 152613.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2MiwicHVyIjoiYmxvYl9pZCJ9fQ==--355f9686e31fe2644b21c4045ebc6ba821de8386/Screenshot 2026-04-12 152613.png)
Also, fix a big problem, at first I chose drv8300n QFN-24, which does not come with bootstrap diode. I thought there was no D version of the qfn-24 package. But after searching on Google, I found out that Ti has a version of drv8300D. And it is also available on AliExpress :)

![image.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2NCwicHVyIjoiYmxvYl9pZCJ9fQ==--1e055f8fa908650f08dfb76cf023a7a1c444ba4f/image.png)
![Screenshot 2026-04-12 165951.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDE2NSwicHVyIjoiYmxvYl9pZCJ9fQ==--5569a5994207e54ada6b8ceb0665bd8d318d099c/Screenshot 2026-04-12 165951.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/6GfyzV2vDIhM/timelapse-6GfyzV2vDIhM.mp4

## Entry 3
- ID: 2207
- Author: NAFI
- Created At: 2026-04-14T17:34:22Z

### Content

Today I did something very frustrating. Adding 4 same circuit schematics to take u 4in1 ESC.

![Screenshot 2026-04-12 232327.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY3OSwicHVyIjoiYmxvYl9pZCJ9fQ==--03c617e3eef739847820117ab6326634a1e6fb11/Screenshot 2026-04-12 232327.png)

But here is the catch: I have to manually type and edit every single net pad to its corresponding ESC number (like sda1, sda2, sda3 ...).

![Screenshot 2026-04-12 231841.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY4MCwicHVyIjoiYmxvYl9pZCJ9fQ==--68f07b1aee05c0cc49387392cf52684844cb782b/Screenshot 2026-04-12 231841.png) 

![Screenshot 2026-04-12 232309.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDY4MSwicHVyIjoiYmxvYl9pZCJ9fQ==--dbccd4061d45e703162e581c4ae425872d42babe/Screenshot 2026-04-12 232309.png)

It took me more than 1 hour to do ;(
But after all the work is done.



### Recording Links

- https://public.lapse-hackclub.link/timelapses/en4dqctDFa-q/timelapse-en4dqctDFa-q.mp4

## Entry 4
- ID: 2354
- Author: NAFI
- Created At: 2026-04-15T18:27:51Z

### Content

So there are too many resistors and capacitors to place in a 2 sided PCB, only 30*30mm. 
![Screenshot 2026-04-12 234142.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDkzMiwicHVyIjoiYmxvYl9pZCJ9fQ==--94a0737f586f5eb01936e47a6dd0c8ed39e53aad/Screenshot 2026-04-12 234142.png)
But somehow I need to do it, so begin with gate drivers and MCUs in diffarent side of the PCB. MCUs on top and gate drivers at the bottom.
![Screenshot 2026-04-13 003505.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDkzNCwicHVyIjoiYmxvYl9pZCJ9fQ==--2775d7c71fa99d0066b990122357b0c423ee6209/Screenshot 2026-04-13 003505.png)
then i stared placing feedback resistors...........


### Recording Links

- https://public.lapse-hackclub.link/timelapses/904tiRd4TA7I/timelapse-904tiRd4TA7I.mp4

## Entry 5
- ID: 2358
- Author: NAFI
- Created At: 2026-04-15T18:43:39Z

### Content

So I started placing gate resistors yesterday, and today it's complete. 


But here is a catch: I placed all gate drivers on one side. For that, all the gate resistors should be on that side too. And for this reason, I created this resistor mesh.
![Screenshot 2026-04-13 180920.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDk0MywicHVyIjoiYmxvYl9pZCJ9fQ==--969a294786c5c6e83d1a3a139c347cf43f45e60f/Screenshot 2026-04-13 180920.png)

Now there is too little space to route all the traces. If I use too many vias, the trace resistance will be greater than the actual resistor value. So I need an efficient way to place all the components........

### Recording Links

- https://public.lapse-hackclub.link/timelapses/mJ234j6gotP4/timelapse-mJ234j6gotP4.mp4

## Entry 6
- ID: 2477
- Author: NAFI
- Created At: 2026-04-16T19:34:21Z

### Content

I switched the placement strategy. 

Instead of placing gate drivers on one side and MCUs on the other, I placed 2 MCUs and 2 gate drivers on one side and the other 2 on the other side.
![Screenshot 2026-04-14 124223.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTE4OCwicHVyIjoiYmxvYl9pZCJ9fQ==--01994eba90963c1cec0e7b20a2947525702ddbf9/Screenshot 2026-04-14 124223.png)


It will significantly reduce the use of more vias and save some space. Accually i got this idea from Kiss Ultra v3 esc.

Also i moved the phase output pad to the edge for edge plating. For this, it can now output more current than a normal multilayer pad.


![Screenshot 2026-04-14 133220.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTE4NywicHVyIjoiYmxvYl9pZCJ9fQ==--97f27e1296822db1e0af18aafb8eab1151b58405/Screenshot 2026-04-14 133220.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/D78rtctXlnH5/timelapse-D78rtctXlnH5.mp4

## Entry 7
- ID: 2741
- Author: NAFI
- Created At: 2026-04-18T17:15:43Z

### Content

Just add the multi layer pads for motor phase output and 2 big pads for power input. And placed them at the board outline for making them castellated holes. I also extend the board outline by 1mm at the pads.
![1000040280.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc0NCwicHVyIjoiYmxvYl9pZCJ9fQ==--23c94b4bd2d889461b7fbf4f46a6741572d3d1f6/1000040280.png)

And add many vias for high corrent flow.
![1000040282.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc0OCwicHVyIjoiYmxvYl9pZCJ9fQ==--d9d2a9bf8110f59063407d786d3a40f16fa121d2/1000040282.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/qbsJZ9rIreRg/timelapse-qbsJZ9rIreRg.mp4

## Entry 8
- ID: 2745
- Author: NAFI
- Created At: 2026-04-18T17:39:50Z

### Content

After placing all the pads for castellated holes, I started routing traces. i used 0.18mm trace for all the signal connections. and some 0.2mm.
![Screenshot 2026-04-14 173357.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NTc1MywicHVyIjoiYmxvYl9pZCJ9fQ==--6f703c2d31f18603d6cf7ee2cc0c6e5df262895c/Screenshot 2026-04-14 173357.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/uukYo2lN7eIS/timelapse-uukYo2lN7eIS.mp4

## Entry 9
- ID: 2931
- Author: NAFI
- Created At: 2026-04-19T18:57:41Z

### Content

Tracing the 106 signal and the back EMF line is a little bit tricky. But somehow I pulled them off.

![Screenshot 2026-04-20 005207.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjExMiwicHVyIjoiYmxvYl9pZCJ9fQ==--81688ab64eb48c62890bfc3add05b2f21763113a/Screenshot 2026-04-20 005207.png)

I placed lots of vias of 0.3mm drill hole and 0.5mm diameter, because JLCPCB didn't charge extra for epoxy filled via s if via>0.5mm.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/J-ME_Ey1Y9RK/timelapse-J-ME_Ey1Y9RK.mp4

## Entry 10
- ID: 3239
- Author: NAFI
- Created At: 2026-04-21T17:23:45Z

### Content

Ahh! After many days of work, the PCB routing is finally done (Almost).
![Screenshot 2026-04-17 003909.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjczNywicHVyIjoiYmxvYl9pZCJ9fQ==--457f48b69e117af58f0583978d9510206b1ab8ab/Screenshot 2026-04-17 003909.png)

The only thing left is to connect some gnd pad to gnd and 3.3v to the main 3.3v pad. But there is no free space left for it.
![Screenshot 2026-04-21 232250.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NjczOCwicHVyIjoiYmxvYl9pZCJ9fQ==--8064693ff0e512f25ccf7be36d65bdd6b732933f/Screenshot 2026-04-21 232250.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/Z7C_Ijw4qDf0/timelapse-Z7C_Ijw4qDf0.mp4

## Entry 11
- ID: 8162
- Author: NAFI
- Created At: 2026-05-20T14:55:40Z

### Content

I just don't have enough space in the PCB to place the 3.3v vias. So i just unrouted the existing routes and created some space to place some 3.3v vias.
![Screenshot 2026-05-19 010940.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTc4NDUsInB1ciI6ImJsb2JfaWQifX0=--c9c2daa076832f5f490210280cda219407c68ce0/Screenshot 2026-05-19 010940.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/LJ-o1sSxgkMX/timelapse-LJ-o1sSxgkMX.mp4

## Entry 12
- ID: 8335
- Author: NAFI
- Created At: 2026-05-21T17:19:05Z

### Content

Finally, I figured out how to place 3.3V vias and route the V+ bus to the DRV8300 gate driver.

![Screenshot 2026-05-20 212708.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMzEsInB1ciI6ImJsb2JfaWQifX0=--1a67eed05e2fdcecdac839cdc9fe3c6b62076174/Screenshot 2026-05-20 212708.png)

![Screenshot 2026-05-20 212723.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMzIsInB1ciI6ImJsb2JfaWQifX0=--4ef7f5c44eed66ccb8f1a9870878d6f292eba02f/Screenshot 2026-05-20 212723.png)

Also added Current sensing, i sued a 2512 size 1mohm sunt resistor and INA180A.

![Screenshot 2026-05-21 090557.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTgyMjksInB1ciI6ImJsb2JfaWQifX0=--99a2e4c0ad3361595722344801a0e7e5e580e82a/Screenshot 2026-05-21 090557.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/t9gTDaKhCvt0/timelapse-t9gTDaKhCvt0.mp4

## Entry 13
- ID: 8481
- Author: NAFI
- Created At: 2026-05-22T15:24:24Z

### Content

Re-configured some connections. Also added some power vias for each phase output and routed some un-routed traces
![Screenshot 2026-05-21 032839.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MTg1MzksInB1ciI6ImJsb2JfaWQifX0=--0537a05731e68a41418d4392211a0bc112991b84/Screenshot 2026-05-21 032839.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/GTc06x4hLAUN/timelapse-GTc06x4hLAUN.mp4

## Entry 14
- ID: 9669
- Author: NAFI
- Created At: 2026-05-27T15:28:11Z

### Content

I just need to add some finishing touches. the the pcb design will be completed. 
![Screenshot 2026-05-21 140224.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjE0NTcsInB1ciI6ImJsb2JfaWQifX0=--49a98a4eb590395fd5df7ba74c3de5f6f497284d/Screenshot 2026-05-21 140224.png) i also run some drc cheack in jlcpcb fabricalion web.
![Screenshot 2026-05-21 144235.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjE0NTgsInB1ciI6ImJsb2JfaWQifX0=--2ae39c485cf06991b3194cbc1f02ea74f8dff460/Screenshot 2026-05-21 144235.png)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/egjknMwtG9es/timelapse-egjknMwtG9es.mp4

## Entry 15
- ID: 10268
- Author: NAFI
- Created At: 2026-05-29T22:53:52Z

### Content

Added the last finishing touch before exporting the production files. Here's the final result
![Screenshot 2026-05-21 110434.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMyODgsInB1ciI6ImJsb2JfaWQifX0=--f3033cdf4a72822a64dddc63452068848993aeaf/Screenshot 2026-05-21 110434.png)
I tried to make a heat sink CAD model in Onshape, but my pc cant handel the pcb 3d file that why the lapse is 70% blank.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/uD8Hmfb5TllP/timelapse-uD8Hmfb5TllP.mp4

## Entry 16
- ID: 10280
- Author: NAFI
- Created At: 2026-05-30T00:30:34Z

### Content

Completed the Zine design. I'm just out of creativity for designing the zine. 
![Your paragraph text.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMDksInB1ciI6ImJsb2JfaWQifX0=--d8e306e512f59d607a34015ac4411f8cb6b62fd8/Your paragraph text.png)
also 70% completed editing the repo. The only left is to finish making the BOM file. Then the project will be ready to ship.


### Recording Links

- https://public.lapse-hackclub.link/timelapses/k5HC4egpIGsT/timelapse-k5HC4egpIGsT.mp4

## Entry 17
- ID: 10291
- Author: NAFI
- Created At: 2026-05-30T02:07:23Z

### Content

Finally, all done. This will be the lowest cost project i ever done. especially the MCU at32f421 5pcs only cost 3$ thats only 0.75$ each. 
![Screenshot 2026-05-29 205400.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMjUsInB1ciI6ImJsb2JfaWQifX0=--b2d4707d22279af00bc0eafaeac785e2c7f59d2b/Screenshot 2026-05-29 205400.png) Also, the 6-layer PCB with 1u gold plating+ via in pad only 2.45$ beacuse jlcpcb give free epoxy capped via, it via size> 0.5mm.
![Screenshot 2026-05-29 204812.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6MjMzMjcsInB1ciI6ImJsb2JfaWQifX0=--0350e30e3f5b3982194b0b7c4e4a5de9f8324aea/Screenshot 2026-05-29 204812.png)
I forgot to journal a lapse before, so I am attaching that with it:)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/TJhr2Z3ZKI5y/timelapse-TJhr2Z3ZKI5y.mp4
- https://public.lapse-hackclub.link/timelapses/v6uv_6NIaZKS/timelapse-v6uv_6NIaZKS.mp4

## Entry 18
- ID: 17251
- Author: NAFI
- Created At: 2026-08-16T20:14:56Z

### Content

After so many days, all the components and PCB + stencil arrived.



![PXL_20260809_051220095.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0ODYsInB1ciI6ImJsb2JfaWQifX0=--85c01e78364827a2254527bebcb3abea401dd470/PXL_20260809_051220095.jpg)
![PXL_20260809_054121715.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0ODcsInB1ciI6ImJsb2JfaWQifX0=--cf5d31318dc5b95dfb6d556e815b70f022df4402/PXL_20260809_054121715.jpg)
![PXL_20260809_053734679.MP.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0ODgsInB1ciI6ImJsb2JfaWQifX0=--ae31ac925bfababeb60def49b1bc58b9917db491/PXL_20260809_053734679.MP.jpg)

So I started making the esc.

I placed the stencil and applied solder paste.
![Screenshot 2026-08-17 015630.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0ODksInB1ciI6ImJsb2JfaWQifX0=--663cc4aa90f28c2266222c117dc9d2a8ba10c907/Screenshot 2026-08-17 015630.png)

 Then, placed all components for one side.

![PXL_20260811_221930700.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0OTAsInB1ciI6ImJsb2JfaWQifX0=--a5eeea4985ca215c13ba04c4e2df1e8469654f0d/PXL_20260811_221930700.jpg)

After that i reflow soldered it with a hot plate. and this is the result. 
![PXL_20260814_115539102 (1).jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0OTIsInB1ciI6ImJsb2JfaWQifX0=--86846444ffde00a6712503a82f96775764cd0031/PXL_20260814_115539102 (1).jpg)

As I don't have access to a hot air gun. and I need one for soldering the other side. i placed the components by myself, then took this to a phone repair shop to solder by them.
![PXL_20260812_073923188.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0OTMsInB1ciI6ImJsb2JfaWQifX0=--b8eff59d08575913b64d5952e1f941b2d304fc35/PXL_20260812_073923188.jpg)


### Recording Links

- https://lookout.hackclub.com/api/media/66791229-2c6a-4c68-ad70-b972edcd42f4/video.mp4
- https://lookout.hackclub.com/api/media/0d1d8485-7f1d-48e6-97a5-1089f8826083/video.mp4

## Entry 19
- ID: 17252
- Author: NAFI
- Created At: 2026-08-16T20:23:22Z

### Content

After some solder joint fixing.

i tried to build my own custom AM32 firmware. And I'm ready to upload the firmware using two little jumper wires.
![PXL_20260812_143122904 (1).jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM0OTQsInB1ciI6ImJsb2JfaWQifX0=--b1f89e48ecb3f262a09df390f146ece7308c3c80/PXL_20260812_143122904 (1).jpg)

But unfortunately, after spending 2 hours, I couldn't compile the firmware.hex file. At the end, I'm not a programming guy.

### Recording Links

- https://lookout.hackclub.com/api/media/eaaac81c-e9b0-475a-adb0-42c5a4cbebb7/video.mp4
- https://lookout.hackclub.com/api/media/21130647-3cbb-4cd7-a864-d257e629799e/video.mp4

## Entry 20
- ID: 17253
- Author: NAFI
- Created At: 2026-08-16T21:41:46Z

### Content

Attempt 2 of building firmware.

After downloading and setting uping Keli uvision mdk.
![Screenshot 2026-08-17 033122.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MDEsInB1ciI6ImJsb2JfaWQifX0=--4309d448cde4a9b650722428a18d2037b7c9c8a9/Screenshot 2026-08-17 033122.png)

Then, uploading the At32F421 bootloader to the spare ESC.
i again couldn't figure out how to flash AM32 firmware to the ESC. beacuse its just showing some random errors
![Screenshot 2026-08-17 033208.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MDIsInB1ciI6ImJsb2JfaWQifX0=--a6ea72dc69143a2356393e617c16cffa4926f9d7/Screenshot 2026-08-17 033208.png)

in attempt 3 i made a progress. i flashed am32 f421dev build using Keli uvision. but the official am32 says only use arduino 1 wire flash protocol.
![Screenshot 2026-08-17 034008.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MDMsInB1ciI6ImJsb2JfaWQifX0=--d3f9b35b7bb087e3276b9b7e87609fc720236702/Screenshot 2026-08-17 034008.png)
thats why its also didn't work either. i think i need to buy an Arduino Nano.

### Recording Links

- https://lookout.hackclub.com/api/media/760cfc4d-572a-4ec9-8d76-82ccc080b26f/video.mp4
- https://lookout.hackclub.com/api/media/6def7daa-74b1-43f3-bec1-15b4d9c75cc1/video.mp4

## Entry 21
- ID: 17259
- Author: NAFI
- Created At: 2026-08-17T07:54:22Z

### Content

Journaled all the previous work.
![Screenshot 2026-08-17 134922.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MjAsInB1ciI6ImJsb2JfaWQifX0=--ef18315c70813f85167bb7b1d0f747d2f894cef8/Screenshot 2026-08-17 134922.png)

Finished designing the zine for build using Canva.
![Screenshot 2026-08-17 133041.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MjEsInB1ciI6ImJsb2JfaWQifX0=--68857085c14a1d8d2b61cd8d6acdc069499324b8/Screenshot 2026-08-17 133041.png)

Also finished working on the GitHub repository.
![Screenshot 2026-08-17 134459.png](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1MjIsInB1ciI6ImJsb2JfaWQifX0=--f0238f618d7e06695ed26c2950dc969057dad037/Screenshot 2026-08-17 134459.png)

Now time to submit this project for build review.

### Recording Links

- https://lookout.hackclub.com/api/media/8f5b73c0-55d0-41f8-903d-b57b314d2581/video.mp4
- https://lookout.hackclub.com/api/media/5e3d6b19-0197-40bb-9c76-5221f2926feb/video.mp4

## Entry 22
- ID: 17269
- Author: NAFI
- Created At: 2026-08-17T17:21:39Z

### Content

Forgot to add this previously. So, attaching a random picture........................................
![PXL_20260815_044052728.jpg](/user-attachments/blobs/redirect/eyJfcmFpbHMiOnsiZGF0YSI6NDM1OTUsInB1ciI6ImJsb2JfaWQifX0=--c380e7f6a4ca2af171c35e054e8a40abf860658d/PXL_20260815_044052728.jpg)


### Recording Links

- https://public.lapse-hackclub.link/timelapses/oIWHnh7_g0_t/timelapse-oIWHnh7_g0_t.mp4
- https://lookout.hackclub.com/api/media/f74ac76c-4a12-47b6-ad84-983a83ecedd6/video.mp4
