# covert-radio

## This is a Covert Radio disguised in a binder. The parts are as follows:


-Raspberry Pi 3 B v2, Running OpenWebRx+

-Dipole Antenna w/ Coaxial Connector

-Anker Powercore 10000mAh Portable Battery

-Anker 4 Port USB Dock (Not strictly necessary but to allow for ethernet to be used easily without an obvious cable snaking out, and to also allow the Radio to be situated inside the binder it was the best choice)

-RTL SDR Blog v4 (avoid counterfits!)


## Pictures:

![IMG_7880](https://github.com/user-attachments/assets/7895d0c5-9cde-409c-a398-afd0be1f3a95)

![IMG_7884](https://github.com/user-attachments/assets/12b47bc4-19df-4b32-993d-a1d5cac0c55a)

![IMG_7892](https://github.com/user-attachments/assets/34bf9b7c-f6c5-4bf9-9925-1afd7ea93a69)

![IMG_7899](https://github.com/user-attachments/assets/4ee049a3-da2c-4436-91f3-e4725dec950b)

![IMG_7898](https://github.com/user-attachments/assets/bbf02d41-1670-4a97-9551-3ff2c6dd83db)

![Screen Shot 2025-04-13 at 12 54 52 PM](https://github.com/user-attachments/assets/5ef5d11b-4fd1-48be-8696-dfd52e064367)


## Build Instructions:

1. First I harvested a binder. Breaking off the Rings was trivial, using pliers. Designing this with my backpack in mind, I cut the sides of it to allow it to squeeze into a laptop slot in the bag.

2. To make it look clean, I painted over the cut edges with white paint.

3. To conceal the device further I cut pieces of scrap paper to the size of the binder allowing room for them to stick out. I did it in three sections for the top, bottom and side. By cutting tons of paper and then glueing the far side of it, it would make the paper look like it was springing out of the binder.
   - A thing to note is to vary the size of the papers so they look natural
   - After doing this three times I split the long side horizontally on the top and bottom just enough for them to slide in, so it wouldnt be obvious and then glued them along the edges of the binder as shown.

4. The Next step is to measure your components and hot glue them down.
   - I made a simple 3d Model using the scales of the parts and then printed a dimensionally accurate 2d version out and traced it, then glued cardboard on the traced lines.
   - The 3d Model blueprint of where the components go is attached at the very end of this document.

5. Now above i glued some cardboard to the top panel of the binder to securely hold the battery and dock in place so when it shakes it will not rattle around.

6. Now we must harvest some magnets. If you already own strong magnets use those
   - Since I did I opened up old broken hard drives and extracted them from there. (The 3.5 inch HDD magnets are bigger so that is preferred, but the 2.5 inch "laptop" size also will work.)
     
7. Then in the divots on the cardboard glue down magents covering them with another glued piece of cardboard so they are very secure.
   - To make sure they align on the top I put a small amount of glue on the top of the other magnets and then closed the binder to see where it was on the top. With that placement glue in the other two magnets.

8. Next we will install OpenWebRX+ on the rPi. By flashing luarvique's prebuilt images using any flashing software (Balena Etcher for example) it is plug and play to install and with the RTL-SDR 4.
   - Download the image from here: https://github.com/luarvique/openwebrx/releases/latest

9. Once Flashed insert into the Pi and do inital setup with a keyboard.
   - Here you can connect to wifi or ethernet, by entering ***sudo raspi-config***
   - After network is set up and the PI is rebooted, above the terminal input section the IP address of the device is shown which should be recorded somewhere.

10. Now placing in the components is fairly easy, one thing to note is to plug in the RTL SDR 4 before putting in the dock, and sliding them in together so they fit well otherwise they will not fit.

11. Any spots where there is a cut in the cardboard for a cable as shown in the 3d model where there is paper interfering, by cutting with a razor horizontally on the back of the paper where the cable needs to go, it can be slotted in easily.

12. When all is done plug in your power cable to the Pi and Battery, wait for it to boot for a few seconds then browse to the PI's IP address and enjoy surfing the waterfall!


## Blueprint of supports for hardware

```stl
solid 
facet normal 1.0 0.0 0.0
    outer loop
        vertex 150.0 -100.0 2.5
        vertex 150.0 -100.0 0.0
        vertex 150.0 100.0 0.0
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 150.0 -100.0 2.5
        vertex 150.0 100.0 0.0
        vertex 150.0 100.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 92.0 19.0 2.5999999046325684
        vertex 93.0 19.0 2.5999999046325684
        vertex 92.0 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 94.5 13.003000259399414 2.5999999046325684
        vertex 92.0 13.003000259399414 2.5999999046325684
        vertex 93.0 19.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 92.0 -8.5 2.5999999046325684
        vertex 92.0 -1.003000020980835 2.5999999046325684
        vertex 93.0 -8.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 94.5 -1.003000020980835 2.5999999046325684
        vertex 93.0 -8.5 2.5999999046325684
        vertex 92.0 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 92.0 13.003000259399414 32.5
        vertex 92.0 13.003000259399414 2.5999999046325684
        vertex 94.5 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 92.0 13.003000259399414 32.5
        vertex 94.5 13.003000259399414 2.5999999046325684
        vertex 94.5 13.003000259399414 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -150.0 100.0 2.5
        vertex -150.0 100.0 0.0
        vertex -150.0 -100.0 0.0
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -150.0 100.0 2.5
        vertex -150.0 -100.0 0.0
        vertex -150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 94.5 -1.003000020980835 32.5
        vertex 94.5 -1.003000020980835 2.5999999046325684
        vertex 92.0 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 94.5 -1.003000020980835 32.5
        vertex 92.0 -1.003000020980835 2.5999999046325684
        vertex 92.0 -1.003000020980835 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 70.0 2.5999999046325684
        vertex 110.0 70.0 17.49799919128418
        vertex 110.0 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -20.5 2.5
        vertex 32.000999450683594 -20.5 2.5
        vertex 32.0 -11.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 93.0 -11.0 2.5
        vertex 32.0 -11.0 2.5
        vertex 32.000999450683594 -20.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -20.5 2.5
        vertex 93.0 -11.0 2.5
        vertex 32.000999450683594 -20.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 0.0 19.0 2.5
        vertex 92.0 19.0 2.5999999046325684
        vertex 0.0 19.0 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 92.0 19.0 32.5
        vertex 0.0 19.0 32.5
        vertex 92.0 19.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 93.0 19.0 2.5
        vertex 92.0 19.0 2.5999999046325684
        vertex 0.0 19.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 94.5 -11.0 32.5
        vertex 92.0 -8.5 32.5
        vertex 32.0 -11.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 29.5 -8.5 32.5
        vertex 32.0 -11.0 32.5
        vertex 92.0 -8.5 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 70.0 17.49799919128418
        vertex 107.5 70.0 2.5999999046325684
        vertex 107.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 93.0 19.0 2.5
        vertex 93.0 19.0 2.5999999046325684
        vertex 92.0 19.0 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 0.0 -79.9990005493164 2.5
        vertex 0.0 -80.0 2.5
        vertex 0.0 -80.0 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 0.0 -79.9990005493164 2.5
        vertex 0.0 -80.0 32.5
        vertex 0.0 -79.9990005493164 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -77.5 32.5
        vertex 0.0 19.0 32.5
        vertex -2.5 -79.9990005493164 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -79.9990005493164 32.5
        vertex 0.0 -77.5 32.5
        vertex -2.5 -79.9990005493164 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 41.99800109863281 32.599998474121094
        vertex 110.0 -20.5 32.599998474121094
        vertex 110.0 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -2.5 -79.9990005493164 32.5
        vertex -2.5 -79.9990005493164 2.5
        vertex 0.0 -79.9990005493164 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 70.0 2.5999999046325684
        vertex 107.5 13.003000259399414 2.5999999046325684
        vertex 107.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 0.0 -79.9990005493164 32.5
        vertex -2.5 -79.9990005493164 2.5
        vertex 0.0 -79.9990005493164 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 70.0 17.49799919128418
        vertex 110.0 70.0 17.49799919128418
        vertex 110.0 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 70.0 17.49799919128418
        vertex 110.0 70.0 2.5999999046325684
        vertex 107.5 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 110.0 41.99800109863281 32.599998474121094
        vertex 110.0 41.99800109863281 17.49799919128418
        vertex 107.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 110.0 41.99800109863281 32.599998474121094
        vertex 107.5 41.99800109863281 17.49799919128418
        vertex 107.5 41.99800109863281 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 94.5 -11.0 32.5
        vertex 94.5 -11.0 2.5999999046325684
        vertex 94.5 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 94.5 -11.0 2.5999999046325684
        vertex 93.0 -11.0 2.5999999046325684
        vertex 93.0 -8.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 94.5 -11.0 2.5999999046325684
        vertex 93.0 -8.5 2.5999999046325684
        vertex 94.5 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 41.99800109863281 17.49799919128418
        vertex 110.0 41.99800109863281 17.49799919128418
        vertex 110.0 70.0 17.49799919128418
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 41.99800109863281 17.49799919128418
        vertex 110.0 70.0 17.49799919128418
        vertex 107.5 70.0 17.49799919128418
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 93.0 -8.5 2.5999999046325684
        vertex 93.0 -11.0 2.5999999046325684
        vertex 93.0 -11.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 93.0 -8.5 2.5999999046325684
        vertex 93.0 -11.0 2.5
        vertex 93.0 -8.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 94.5 21.5 2.5999999046325684
        vertex 93.0 21.5 2.5999999046325684
        vertex 94.5 21.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 92.0 19.0 32.5
        vertex 94.5 21.5 32.5
        vertex 0.0 19.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -2.5 21.5 32.5
        vertex 0.0 19.0 32.5
        vertex 94.5 21.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 94.5 21.5 32.5
        vertex 93.0 21.5 2.5999999046325684
        vertex -2.5 21.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 32.0 -79.99800109863281 32.5
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -79.9990005493164 32.5
        vertex 32.0 -79.99800109863281 32.5
        vertex 31.99799919128418 -79.9990005493164 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -79.99800109863281 32.5
        vertex 34.5 -23.0 32.5
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 70.0 2.5999999046325684
        vertex 110.0 41.99800109863281 17.49799919128418
        vertex 110.0 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 41.99800109863281 32.599998474121094
        vertex 110.0 13.003000259399414 17.503000259399414
        vertex 110.0 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 13.003000259399414 2.5999999046325684
        vertex 110.0 41.99800109863281 17.49799919128418
        vertex 110.0 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -2.5 21.5 2.5
        vertex -2.5 21.5 32.5
        vertex 93.0 21.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 32.0 -79.9990005493164 2.5
        vertex 32.0 -79.9990005493164 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 13.003000259399414 17.503000259399414
        vertex 107.5 41.99800109863281 17.49799919128418
        vertex 107.5 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 41.99800109863281 32.599998474121094
        vertex 107.5 41.99800109863281 17.49799919128418
        vertex 107.5 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -2.5 21.5 2.5
        vertex 93.0 21.5 2.5999999046325684
        vertex 93.0 21.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 31.99799919128418 -80.0 32.5
        vertex 22.003000259399414 -80.0 17.503000259399414
        vertex 31.99799919128418 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 13.003000259399414 2.5999999046325684
        vertex 107.5 70.0 2.5999999046325684
        vertex 110.0 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 32.000999450683594 -20.5 2.5
        vertex 32.000999450683594 -20.5 32.5
        vertex 107.5 -20.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -20.5 32.5
        vertex 107.5 -20.5 2.5999999046325684
        vertex 32.000999450683594 -20.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 32.000999450683594 -20.5 2.5
        vertex 107.5 -20.5 2.5999999046325684
        vertex 110.0 -20.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 2.5
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 31.99799919128418 -80.0 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 2.5
        vertex 31.99799919128418 -80.0 32.5
        vertex 31.99799919128418 -80.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 94.5 13.003000259399414 2.5999999046325684
        vertex 94.5 21.5 2.5999999046325684
        vertex 94.5 21.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -20.5 2.5999999046325684
        vertex 110.0 -20.5 2.5999999046325684
        vertex 110.0 -20.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 32.0 -79.9990005493164 2.5
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 31.99799919128418 -79.9990005493164 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 93.0 21.5 2.5999999046325684
        vertex 94.5 21.5 2.5999999046325684
        vertex 93.0 19.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 94.5 13.003000259399414 2.5999999046325684
        vertex 93.0 19.0 2.5999999046325684
        vertex 94.5 21.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -39.0 -54.0 32.099998474121094
        vertex -2.5 -54.0 32.099998474121094
        vertex -2.5 -30.0 32.099998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -39.0 -54.0 32.099998474121094
        vertex -2.5 -30.0 32.099998474121094
        vertex -39.0 -30.0 32.099998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 93.0 21.5 2.5999999046325684
        vertex 93.0 19.0 2.5999999046325684
        vertex 93.0 19.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 93.0 21.5 2.5999999046325684
        vertex 93.0 19.0 2.5
        vertex 93.0 21.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -79.99800109863281 32.5
        vertex 32.0 -79.9990005493164 32.5
        vertex 32.0 -79.9990005493164 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -2.5 -54.0 29.600000381469727
        vertex -39.0 -54.0 29.600000381469727
        vertex -39.0 -30.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -2.5 -54.0 29.600000381469727
        vertex -39.0 -30.0 29.600000381469727
        vertex -2.5 -30.0 29.600000381469727
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -79.9990005493164 2.5
        vertex 32.0 -79.99800109863281 2.5
        vertex 32.0 -79.99800109863281 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -39.0 -54.0 32.099998474121094
        vertex -39.0 -54.0 29.600000381469727
        vertex -2.5 -54.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -39.0 -54.0 32.099998474121094
        vertex -2.5 -54.0 29.600000381469727
        vertex -2.5 -54.0 32.099998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -1.003000020980835 17.503000259399414
        vertex 110.0 13.003000259399414 17.503000259399414
        vertex 110.0 -20.5 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -80.0 2.5999999046325684
        vertex 110.0 -80.0 2.5
        vertex 110.0 -77.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -80.0 2.5999999046325684
        vertex 110.0 -77.5 2.5
        vertex 110.0 -77.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -2.5 -30.0 32.099998474121094
        vertex -2.5 -30.0 29.600000381469727
        vertex -39.0 -30.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -2.5 -30.0 32.099998474121094
        vertex -39.0 -30.0 29.600000381469727
        vertex -39.0 -30.0 32.099998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -54.0 32.099998474121094
        vertex -2.5 -79.9990005493164 32.5
        vertex -2.5 -30.0 32.099998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 21.5 32.5
        vertex -2.5 -30.0 32.099998474121094
        vertex -2.5 -79.9990005493164 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -54.0 32.099998474121094
        vertex -2.5 -54.0 29.600000381469727
        vertex -2.5 -79.9990005493164 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -79.9990005493164 2.5
        vertex -2.5 -54.0 29.600000381469727
        vertex -2.5 -30.0 29.600000381469727
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -30.0 32.099998474121094
        vertex -2.5 21.5 32.5
        vertex -2.5 -30.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 29.5 -8.5 2.5
        vertex 29.5 -8.5 32.5
        vertex 92.0 -8.5 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -38.99800109863281 19.503000259399414
        vertex 110.0 -20.5 32.599998474121094
        vertex 110.0 -53.00299835205078 19.503000259399414
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -79.9990005493164 2.5
        vertex -2.5 -79.9990005493164 32.5
        vertex -2.5 -54.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 92.0 -8.5 32.5
        vertex 92.0 -8.5 2.5999999046325684
        vertex 29.5 -8.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -80.0 2.5999999046325684
        vertex 110.0 -77.5 2.5999999046325684
        vertex 110.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -100.0 2.5999999046325684
        vertex 110.0 -80.0 2.5999999046325684
        vertex 110.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 110.0 -100.0 32.599998474121094
        vertex 110.0 -77.5 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -53.00299835205078 2.5999999046325684
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 110.0 -77.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 92.0 -8.5 2.5999999046325684
        vertex 93.0 -8.5 2.5999999046325684
        vertex 93.0 -8.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 92.0 -8.5 2.5999999046325684
        vertex 93.0 -8.5 2.5
        vertex 29.5 -8.5 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -1.003000020980835 17.503000259399414
        vertex 107.5 -11.0 32.599998474121094
        vertex 107.5 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -38.99800109863281 2.5999999046325684
        vertex 110.0 -23.0 2.5999999046325684
        vertex 110.0 -38.99800109863281 19.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -77.5 32.5
        vertex 67.00299835205078 -77.5 13.503000259399414
        vertex 34.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 34.5 -77.5 32.5
        vertex 47.99800109863281 -77.5 13.503000259399414
        vertex 34.5 -77.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 0.0 -77.5 32.5
        vertex 0.0 19.0 2.5
        vertex 0.0 19.0 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 7.998000144958496 -80.0 17.503000259399414
        vertex 22.003000259399414 -80.0 17.503000259399414
        vertex 0.0 -80.0 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -1.003000020980835 2.5999999046325684
        vertex 107.5 -20.5 2.5999999046325684
        vertex 107.5 -1.003000020980835 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 47.99800109863281 -77.5 13.503000259399414
        vertex 34.5 -77.5 32.5
        vertex 67.00299835205078 -77.5 13.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 31.99799919128418 -80.0 32.5
        vertex 0.0 -80.0 32.5
        vertex 22.003000259399414 -80.0 17.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 22.003000259399414 -80.0 2.5
        vertex 31.99799919128418 -80.0 2.5
        vertex 22.003000259399414 -80.0 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -77.5 32.5
        vertex 107.5 -77.5 2.5999999046325684
        vertex 67.00299835205078 -77.5 13.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 67.00299835205078 -77.5 2.5
        vertex 67.00299835205078 -77.5 13.503000259399414
        vertex 107.5 -77.5 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 29.5 -8.5 2.5
        vertex 29.5 -77.5 2.5
        vertex 29.5 -8.5 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 29.5 -77.5 32.5
        vertex 29.5 -8.5 32.5
        vertex 29.5 -77.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 0.0 -80.0 32.5
        vertex 0.0 -80.0 2.5
        vertex 7.998000144958496 -80.0 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 47.99800109863281 -77.5 2.5
        vertex 34.5 -77.5 2.5
        vertex 47.99800109863281 -77.5 13.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -23.0 2.5999999046325684
        vertex 110.0 -20.5 2.5999999046325684
        vertex 110.0 -20.5 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -1.003000020980835 2.5999999046325684
        vertex 110.0 -1.003000020980835 17.503000259399414
        vertex 110.0 -20.5 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -20.5 32.599998474121094
        vertex 110.0 -20.5 2.5999999046325684
        vertex 110.0 -1.003000020980835 17.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 7.998000144958496 -80.0 2.5
        vertex 7.998000144958496 -80.0 17.503000259399414
        vertex 0.0 -80.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -20.5 32.5
        vertex 107.5 -11.0 32.599998474121094
        vertex 107.5 -20.5 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -11.0 32.599998474121094
        vertex 107.5 -1.003000020980835 17.503000259399414
        vertex 107.5 -20.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 0.0 -77.5 32.5
        vertex 29.5 -77.5 32.5
        vertex 7.998000144958496 -77.5 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 7.998000144958496 -77.5 17.503000259399414
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 29.5 -77.5 32.5
        vertex 29.5 -77.5 2.5
        vertex 22.003000259399414 -77.5 17.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -20.5 2.5999999046325684
        vertex 107.5 -20.5 2.5999999046325684
        vertex 110.0 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 107.5 -80.0 2.5999999046325684
        vertex 107.5 -80.0 32.5
        vertex 67.00299835205078 -80.0 13.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 67.00299835205078 -80.0 2.5
        vertex 107.5 -80.0 2.5999999046325684
        vertex 67.00299835205078 -80.0 13.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 0.0 -77.5 2.5
        vertex 7.998000144958496 -77.5 17.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -11.0 32.5
        vertex 32.0 -20.5 32.5
        vertex 32.0 -20.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -11.0 32.5
        vertex 32.0 -20.5 2.5
        vertex 32.0 -11.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 67.00299835205078 -80.0 13.503000259399414
        vertex 32.000999450683594 -80.0 32.5
        vertex 47.99800109863281 -80.0 13.503000259399414
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 47.99800109863281 -80.0 2.5
        vertex 47.99800109863281 -80.0 13.503000259399414
        vertex 32.000999450683594 -80.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 22.003000259399414 -77.5 2.5
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 29.5 -77.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -11.0 32.5
        vertex 29.5 -8.5 32.5
        vertex 32.0 -20.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 29.5 -77.5 32.5
        vertex 32.0 -21.0 32.5
        vertex 29.5 -8.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 -80.0 32.5
        vertex 107.5 -77.5 32.5
        vertex 34.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 0.0 -77.5 32.5
        vertex 7.998000144958496 -77.5 17.503000259399414
        vertex 0.0 -77.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 93.0 -11.0 2.5999999046325684
        vertex 94.5 -11.0 2.5999999046325684
        vertex 94.5 -11.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 67.00299835205078 -77.5 13.503000259399414
        vertex 67.00299835205078 -80.0 13.503000259399414
        vertex 47.99800109863281 -80.0 13.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 67.00299835205078 -77.5 13.503000259399414
        vertex 47.99800109863281 -80.0 13.503000259399414
        vertex 47.99800109863281 -77.5 13.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 107.5 -20.5 2.5999999046325684
        vertex 107.5 -1.003000020980835 2.5999999046325684
        vertex 110.0 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 67.00299835205078 -80.0 13.503000259399414
        vertex 67.00299835205078 -77.5 13.503000259399414
        vertex 67.00299835205078 -77.5 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 67.00299835205078 -80.0 13.503000259399414
        vertex 67.00299835205078 -77.5 2.5
        vertex 67.00299835205078 -80.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 32.0 -11.0 2.5
        vertex 93.0 -11.0 2.5999999046325684
        vertex 32.0 -11.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 13.003000259399414 2.5999999046325684
        vertex 107.5 13.003000259399414 2.5999999046325684
        vertex 107.5 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -79.9990005493164 32.5
        vertex 0.0 -80.0 32.5
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 31.99799919128418 -80.0 32.5
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 0.0 -80.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -77.5 32.5
        vertex 0.0 -79.9990005493164 32.5
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 47.99800109863281 -77.5 2.5
        vertex 47.99800109863281 -77.5 13.503000259399414
        vertex 47.99800109863281 -80.0 13.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 47.99800109863281 -77.5 2.5
        vertex 47.99800109863281 -80.0 13.503000259399414
        vertex 47.99800109863281 -80.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 94.5 -11.0 32.5
        vertex 32.0 -11.0 32.5
        vertex 93.0 -11.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 93.0 -11.0 2.5
        vertex 93.0 -11.0 2.5999999046325684
        vertex 32.0 -11.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -1.003000020980835 17.503000259399414
        vertex 107.5 -1.003000020980835 17.503000259399414
        vertex 107.5 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -1.003000020980835 17.503000259399414
        vertex 107.5 13.003000259399414 17.503000259399414
        vertex 110.0 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 32.5
        vertex 29.5 -77.5 32.5
        vertex 0.0 -80.0 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -38.99800109863281 19.503000259399414
        vertex 107.5 -53.00299835205078 19.503000259399414
        vertex 107.5 -23.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 22.003000259399414 -80.0 17.503000259399414
        vertex 7.998000144958496 -80.0 17.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 7.998000144958496 -80.0 17.503000259399414
        vertex 7.998000144958496 -77.5 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 110.0 -1.003000020980835 2.5999999046325684
        vertex 107.5 -1.003000020980835 2.5999999046325684
        vertex 110.0 -1.003000020980835 17.503000259399414
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -1.003000020980835 17.503000259399414
        vertex 110.0 -1.003000020980835 17.503000259399414
        vertex 107.5 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -77.5 32.5
        vertex 107.5 -23.0 32.599998474121094
        vertex 107.5 -53.00299835205078 19.503000259399414
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -53.00299835205078 2.5999999046325684
        vertex 107.5 -77.5 2.5999999046325684
        vertex 107.5 -53.00299835205078 19.503000259399414
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 41.99800109863281 32.599998474121094
        vertex 107.5 13.003000259399414 17.503000259399414
        vertex 107.5 -11.0 32.599998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 22.003000259399414 -80.0 17.503000259399414
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 22.003000259399414 -80.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 13.003000259399414 2.5999999046325684
        vertex 110.0 13.003000259399414 17.503000259399414
        vertex 107.5 13.003000259399414 17.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 7.998000144958496 -77.5 17.503000259399414
        vertex 7.998000144958496 -80.0 17.503000259399414
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 7.998000144958496 -80.0 17.503000259399414
        vertex 7.998000144958496 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -20.5 32.599998474121094
        vertex 110.0 41.99800109863281 32.599998474121094
        vertex 107.5 -11.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 41.99800109863281 32.599998474121094
        vertex 107.5 -11.0 32.599998474121094
        vertex 110.0 41.99800109863281 32.599998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -100.0 32.599998474121094
        vertex 107.5 -80.0 32.5
        vertex 107.5 -100.0 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -80.0 2.5999999046325684
        vertex 107.5 -100.0 2.5999999046325684
        vertex 107.5 -80.0 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 22.003000259399414 -77.5 17.503000259399414
        vertex 22.003000259399414 -77.5 2.5
        vertex 22.003000259399414 -80.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -80.0 32.5
        vertex 107.5 -100.0 32.599998474121094
        vertex 107.5 -77.5 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -23.0 32.599998474121094
        vertex 107.5 -77.5 32.5
        vertex 107.5 -100.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 13.003000259399414 2.5999999046325684
        vertex 107.5 13.003000259399414 17.503000259399414
        vertex 107.5 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -23.0 32.599998474121094
        vertex 107.5 -23.0 32.5
        vertex 107.5 -38.99800109863281 19.503000259399414
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -23.0 32.5
        vertex 107.5 -23.0 2.5999999046325684
        vertex 107.5 -38.99800109863281 19.503000259399414
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -38.99800109863281 2.5999999046325684
        vertex 107.5 -38.99800109863281 19.503000259399414
        vertex 107.5 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 94.5 21.5 32.5
        vertex 94.5 13.003000259399414 32.5
        vertex 94.5 13.003000259399414 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -77.5 32.5
        vertex 107.5 -53.00299835205078 19.503000259399414
        vertex 107.5 -77.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 -100.0 32.599998474121094
        vertex 110.0 -100.0 32.599998474121094
        vertex 107.5 -23.0 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 94.5 -1.003000020980835 2.5999999046325684
        vertex 94.5 -1.003000020980835 32.5
        vertex 94.5 -11.0 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -77.5 2.5999999046325684
        vertex 110.0 -77.5 2.5999999046325684
        vertex 110.0 -77.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -77.5 2.5999999046325684
        vertex 110.0 -77.5 2.5
        vertex 67.00299835205078 -77.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 67.00299835205078 -80.0 2.5
        vertex 110.0 -80.0 2.5
        vertex 107.5 -80.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -80.0 2.5999999046325684
        vertex 107.5 -80.0 2.5999999046325684
        vertex 110.0 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -77.5 2.5999999046325684
        vertex 107.5 -77.5 2.5999999046325684
        vertex 107.5 -53.00299835205078 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -77.5 2.5999999046325684
        vertex 107.5 -53.00299835205078 2.5999999046325684
        vertex 110.0 -53.00299835205078 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -100.0 2.5999999046325684
        vertex 107.5 -100.0 2.5999999046325684
        vertex 107.5 -80.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -100.0 2.5999999046325684
        vertex 107.5 -80.0 2.5999999046325684
        vertex 110.0 -80.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -38.99800109863281 2.5999999046325684
        vertex 107.5 -38.99800109863281 2.5999999046325684
        vertex 107.5 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -38.99800109863281 2.5999999046325684
        vertex 107.5 -23.0 2.5999999046325684
        vertex 110.0 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 107.5 -100.0 32.599998474121094
        vertex 107.5 -100.0 2.5999999046325684
        vertex 110.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -100.0 32.599998474121094
        vertex 107.5 -100.0 2.5999999046325684
        vertex 110.0 -100.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -2.5 -79.9990005493164 2.5
        vertex -150.0 -100.0 2.5
        vertex 0.0 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 107.5 -53.00299835205078 19.503000259399414
        vertex 107.5 -38.99800109863281 19.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 107.5 -38.99800109863281 19.503000259399414
        vertex 110.0 -38.99800109863281 19.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 29.5 -77.5 2.5
        vertex 29.5 -8.5 2.5
        vertex 22.003000259399414 -77.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 107.5 -53.00299835205078 19.503000259399414
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 107.5 -53.00299835205078 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 7.998000144958496 -80.0 2.5
        vertex 22.003000259399414 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 22.003000259399414 -80.0 2.5
        vertex 22.003000259399414 -77.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -38.99800109863281 19.503000259399414
        vertex 107.5 -38.99800109863281 19.503000259399414
        vertex 107.5 -38.99800109863281 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -150.0 -100.0 2.5
        vertex 150.0 -100.0 2.5
        vertex 0.0 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -79.9990005493164 2.5
        vertex -2.5 -79.9990005493164 2.5
        vertex 0.0 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -80.0 2.5
        vertex 31.99799919128418 -80.0 2.5
        vertex 150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 110.0 -53.00299835205078 2.5999999046325684
        vertex 107.5 -53.00299835205078 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 22.003000259399414 -80.0 2.5
        vertex 7.998000144958496 -80.0 2.5
        vertex 150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 31.99799919128418 -80.0 2.5
        vertex 22.003000259399414 -80.0 2.5
        vertex 150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 7.998000144958496 -80.0 2.5
        vertex 0.0 -80.0 2.5
        vertex 150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -38.99800109863281 2.5999999046325684
        vertex 110.0 -38.99800109863281 19.503000259399414
        vertex 107.5 -38.99800109863281 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -39.0 -99.0 2.5999999046325684
        vertex -39.0 -99.0 32.599998474121094
        vertex -41.5 -99.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -41.5 -99.0 32.599998474121094
        vertex -41.5 -99.0 2.5999999046325684
        vertex -39.0 -99.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -80.0 2.5
        vertex 32.0 -79.9990005493164 2.5
        vertex 31.99799919128418 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 31.99799919128418 -79.9990005493164 2.5
        vertex 31.99799919128418 -80.0 2.5
        vertex 32.0 -79.9990005493164 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 34.5 -77.5 2.5
        vertex 34.5 -23.0 2.5
        vertex 34.5 -77.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 34.5 -23.0 32.5
        vertex 34.5 -77.5 32.5
        vertex 34.5 -23.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -77.5 2.5
        vertex 150.0 -100.0 2.5
        vertex 110.0 -23.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -80.0 2.5
        vertex 150.0 -100.0 2.5
        vertex 110.0 -77.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 150.0 100.0 2.5
        vertex 110.0 -20.5 2.5
        vertex 150.0 -100.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -39.0 -9.0 2.5999999046325684
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -39.0 -9.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -80.0 32.5
        vertex 107.5 -80.0 32.5
        vertex 32.000999450683594 -79.99800109863281 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 34.5 -77.5 32.5
        vertex 32.000999450683594 -79.99800109863281 32.5
        vertex 107.5 -80.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 67.00299835205078 -77.5 2.5
        vertex 34.5 -23.0 2.5
        vertex 47.99800109863281 -77.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 34.5 -77.5 2.5
        vertex 47.99800109863281 -77.5 2.5
        vertex 34.5 -23.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -108.5 -8.0 32.5
        vertex -108.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 34.5 -23.0 32.5
        vertex 32.0 -79.99800109863281 32.5
        vertex 32.000999450683594 -79.99800109863281 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 34.5 -23.0 32.5
        vertex 32.000999450683594 -79.99800109863281 32.5
        vertex 34.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 47.99800109863281 -80.0 2.5
        vertex 150.0 -100.0 2.5
        vertex 67.00299835205078 -80.0 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 107.5 -80.0 32.5
        vertex 32.000999450683594 -80.0 32.5
        vertex 67.00299835205078 -80.0 13.503000259399414
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 47.99800109863281 -77.5 2.5
        vertex 47.99800109863281 -80.0 2.5
        vertex 67.00299835205078 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 47.99800109863281 -77.5 2.5
        vertex 67.00299835205078 -80.0 2.5
        vertex 67.00299835205078 -77.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -108.5 -100.0 32.599998474121094
        vertex -108.5 -10.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 67.00299835205078 -77.5 2.5
        vertex 110.0 -77.5 2.5
        vertex 110.0 -23.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 34.5 -23.0 2.5
        vertex 67.00299835205078 -77.5 2.5
        vertex 110.0 -23.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -108.5 -10.5 32.5
        vertex -108.5 -8.0 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 70.0 2.5999999046325684
        vertex -108.5 70.0 17.49799919128418
        vertex -108.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 -8.0 32.5
        vertex -108.5 -8.0 2.5999999046325684
        vertex -108.5 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 70.0 2.5999999046325684
        vertex -108.5 41.99800109863281 17.49799919128418
        vertex -108.5 -8.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 150.0 -100.0 2.5
        vertex 110.0 -80.0 2.5
        vertex 67.00299835205078 -80.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 -10.5 2.5999999046325684
        vertex -108.5 -10.5 32.5
        vertex -108.5 -100.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 32.000999450683594 -80.0 2.5
        vertex 47.99800109863281 -80.0 13.503000259399414
        vertex 32.000999450683594 -80.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -80.0 2.5
        vertex 150.0 -100.0 2.5
        vertex 47.99800109863281 -80.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -108.5 -10.5 32.5
        vertex -108.5 -100.0 32.599998474121094
        vertex -108.5 -100.0 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 32.000999450683594 -79.99800109863281 32.5
        vertex 32.000999450683594 -79.99800109863281 2.5
        vertex 32.000999450683594 -80.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 32.000999450683594 -79.99800109863281 32.5
        vertex 32.000999450683594 -80.0 2.5
        vertex 32.000999450683594 -80.0 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -111.0 41.99800109863281 32.599998474121094
        vertex -111.0 41.99800109863281 17.49799919128418
        vertex -111.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 32.000999450683594 -79.99800109863281 2.5
        vertex 32.000999450683594 -79.99800109863281 32.5
        vertex 32.0 -79.99800109863281 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 32.000999450683594 -79.99800109863281 2.5
        vertex 32.0 -79.99800109863281 32.5
        vertex 32.0 -79.99800109863281 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -111.0 70.0 17.49799919128418
        vertex -111.0 70.0 2.5999999046325684
        vertex -111.0 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -111.0 70.0 2.5999999046325684
        vertex -111.0 -100.0 2.5999999046325684
        vertex -111.0 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -111.0 -100.0 32.599998474121094
        vertex -111.0 41.99800109863281 17.49799919128418
        vertex -111.0 -100.0 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 92.0 19.0 32.5
        vertex 92.0 19.0 2.5999999046325684
        vertex 92.0 13.003000259399414 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 92.0 13.003000259399414 2.5999999046325684
        vertex 92.0 13.003000259399414 32.5
        vertex 92.0 19.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -79.99800109863281 2.5
        vertex 32.0 -79.9990005493164 2.5
        vertex 32.000999450683594 -80.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -79.99800109863281 2.5
        vertex 32.0 -79.9990005493164 2.5
        vertex 32.000999450683594 -79.99800109863281 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 34.5 -23.0 2.5
        vertex 107.5 -23.0 2.5999999046325684
        vertex 34.5 -23.0 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 107.5 -23.0 32.5
        vertex 34.5 -23.0 32.5
        vertex 107.5 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -111.0 -100.0 32.599998474121094
        vertex -108.5 -100.0 32.599998474121094
        vertex -111.0 41.99800109863281 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -108.5 -100.0 32.599998474121094
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -111.0 41.99800109863281 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -23.0 2.5
        vertex 150.0 -100.0 2.5
        vertex 110.0 -20.5 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 92.0 -1.003000020980835 2.5999999046325684
        vertex 92.0 -8.5 32.5
        vertex 92.0 -1.003000020980835 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 92.0 -8.5 2.5999999046325684
        vertex 92.0 -8.5 32.5
        vertex 92.0 -1.003000020980835 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -109.99800109863281 -8.0 2.5
        vertex -109.99800109863281 -8.0 2.5999999046325684
        vertex -108.5 -8.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -81.0 -8.0 2.5
        vertex -81.0 -10.5 2.5
        vertex -2.5 21.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -108.5 -10.5 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 92.0 13.003000259399414 32.5
        vertex 94.5 13.003000259399414 32.5
        vertex 92.0 19.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 94.5 21.5 32.5
        vertex 92.0 19.0 32.5
        vertex 94.5 13.003000259399414 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -23.0 2.5
        vertex 110.0 -23.0 2.5999999046325684
        vertex 107.5 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 110.0 -23.0 2.5
        vertex 107.5 -23.0 2.5999999046325684
        vertex 34.5 -23.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -109.99800109863281 -8.0 2.5999999046325684
        vertex -109.99800109863281 -8.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -109.99800109863281 -8.0 2.5
        vertex -109.99800109863281 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 92.0 -1.003000020980835 32.5
        vertex 92.0 -8.5 32.5
        vertex 94.5 -1.003000020980835 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 94.5 -1.003000020980835 32.5
        vertex 92.0 -8.5 32.5
        vertex 94.5 -11.0 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -100.0 32.599998474121094
        vertex 110.0 -53.00299835205078 19.503000259399414
        vertex 110.0 -20.5 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -111.0 70.0 2.5999999046325684
        vertex -108.5 70.0 2.5999999046325684
        vertex -109.99800109863281 -8.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -108.5 -8.0 2.5999999046325684
        vertex -109.99800109863281 -8.0 2.5999999046325684
        vertex -108.5 70.0 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -23.0 32.599998474121094
        vertex 107.5 -11.0 32.599998474121094
        vertex 107.5 -20.5 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 107.5 -23.0 32.599998474121094
        vertex 107.5 -20.5 32.5
        vertex 107.5 -23.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -111.0 70.0 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -111.0 -100.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -108.5 -100.0 2.5999999046325684
        vertex -111.0 -100.0 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -108.5 -100.0 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -108.5 -10.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -21.0 2.5
        vertex 32.000999450683594 -21.0 2.5
        vertex 32.000999450683594 -20.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -21.0 2.5
        vertex 32.000999450683594 -20.5 2.5
        vertex 32.0 -20.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -109.99800109863281 -8.0 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5999999046325684
        vertex -111.0 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -20.5 32.599998474121094
        vertex 107.5 -11.0 32.599998474121094
        vertex 107.5 -23.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -20.5 32.599998474121094
        vertex 107.5 -23.0 32.599998474121094
        vertex 110.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -81.0 -8.0 2.5
        vertex -150.0 100.0 2.5
        vertex -109.99800109863281 -8.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -2.5 21.5 32.5
        vertex -2.5 -79.9990005493164 32.5
        vertex 0.0 19.0 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -21.0 2.5
        vertex 32.0 -20.5 2.5
        vertex 32.0 -21.0 32.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -111.0 -100.0 2.5999999046325684
        vertex -108.5 -100.0 2.5999999046325684
        vertex -111.0 -100.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -108.5 -100.0 32.599998474121094
        vertex -111.0 -100.0 32.599998474121094
        vertex -108.5 -100.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -111.0 70.0 17.49799919128418
        vertex -108.5 70.0 17.49799919128418
        vertex -108.5 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -111.0 70.0 17.49799919128418
        vertex -108.5 70.0 2.5999999046325684
        vertex -111.0 70.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.0 -20.5 32.5
        vertex 29.5 -8.5 32.5
        vertex 32.0 -21.0 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -108.5 41.99800109863281 17.49799919128418
        vertex -111.0 41.99800109863281 17.49799919128418
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -108.5 41.99800109863281 32.599998474121094
        vertex -111.0 41.99800109863281 17.49799919128418
        vertex -111.0 41.99800109863281 32.599998474121094
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 32.0 -21.0 32.5
        vertex 32.000999450683594 -21.0 2.5
        vertex 32.0 -21.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -21.0 32.5
        vertex 32.0 -21.0 32.5
        vertex 29.5 -77.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -111.0 41.99800109863281 17.49799919128418
        vertex -108.5 41.99800109863281 17.49799919128418
        vertex -108.5 70.0 17.49799919128418
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -111.0 41.99800109863281 17.49799919128418
        vertex -108.5 70.0 17.49799919128418
        vertex -111.0 70.0 17.49799919128418
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 32.000999450683594 -20.5 32.5
        vertex 32.000999450683594 -20.5 2.5
        vertex 32.000999450683594 -21.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -21.0 32.5
        vertex 29.5 -77.5 32.5
        vertex 34.5 -23.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -20.5 32.5
        vertex 32.000999450683594 -21.0 32.5
        vertex 34.5 -23.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 107.5 -23.0 32.5
        vertex 107.5 -20.5 32.5
        vertex 34.5 -23.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 32.000999450683594 -20.5 32.5
        vertex 34.5 -23.0 32.5
        vertex 107.5 -20.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -20.5 32.599998474121094
        vertex 110.0 -38.99800109863281 19.503000259399414
        vertex 110.0 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -81.0 -8.0 2.5
        vertex -2.5 21.5 2.5
        vertex -150.0 100.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 150.0 100.0 2.5
        vertex -150.0 100.0 2.5
        vertex -2.5 21.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 150.0 100.0 2.5
        vertex -2.5 21.5 2.5
        vertex 93.0 21.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -23.0 2.5
        vertex 110.0 -20.5 2.5
        vertex 110.0 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 110.0 -20.5 2.5
        vertex 110.0 -20.5 2.5999999046325684
        vertex 110.0 -23.0 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -30.0 32.099998474121094
        vertex -39.0 -30.0 29.600000381469727
        vertex -39.0 -9.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -2.5 -79.9990005493164 2.5
        vertex -2.5 21.5 2.5
        vertex -81.0 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -150.0 -100.0 2.5
        vertex -2.5 -79.9990005493164 2.5
        vertex -81.0 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -150.0 -100.0 2.5
        vertex -109.99800109863281 -8.0 2.5
        vertex -150.0 100.0 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 -79.9990005493164 2.5
        vertex -2.5 -30.0 29.600000381469727
        vertex -2.5 21.5 2.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -2.5 21.5 32.5
        vertex -2.5 21.5 2.5
        vertex -2.5 -30.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 93.0 21.5 2.5
        vertex 93.0 19.0 2.5
        vertex 150.0 100.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 0.0 -77.5 2.5
        vertex 0.0 19.0 2.5
        vertex 0.0 -77.5 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 110.0 -20.5 2.5
        vertex 150.0 100.0 2.5
        vertex 93.0 19.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -109.99800109863281 -8.0 2.5
        vertex -150.0 -100.0 2.5
        vertex -109.99800109863281 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -109.99800109863281 -10.5 2.5
        vertex -150.0 -100.0 2.5
        vertex -81.0 -10.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -30.0 32.099998474121094
        vertex -39.0 -9.0 32.599998474121094
        vertex -39.0 -54.0 32.099998474121094
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 150.0 -100.0 0.0
        vertex -150.0 -100.0 0.0
        vertex -150.0 100.0 0.0
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex 150.0 -100.0 0.0
        vertex -150.0 100.0 0.0
        vertex 150.0 100.0 0.0
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex 32.0 -21.0 32.5
        vertex 32.0 -20.5 2.5
        vertex 32.0 -20.5 32.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -99.0 32.599998474121094
        vertex -39.0 -99.0 2.5999999046325684
        vertex -39.0 -54.0 29.600000381469727
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 32.000999450683594 -21.0 32.5
        vertex 32.000999450683594 -21.0 2.5
        vertex 32.0 -21.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 19.0 2.5
        vertex 0.0 -77.5 2.5
        vertex 29.5 -8.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 93.0 19.0 2.5
        vertex 0.0 19.0 2.5
        vertex 29.5 -8.5 2.5
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex 150.0 -100.0 2.5
        vertex -150.0 -100.0 2.5
        vertex 150.0 -100.0 0.0
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -150.0 -100.0 0.0
        vertex 150.0 -100.0 0.0
        vertex -150.0 -100.0 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -54.0 29.600000381469727
        vertex -39.0 -54.0 32.099998474121094
        vertex -39.0 -99.0 32.599998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex 32.000999450683594 -20.5 32.5
        vertex 32.000999450683594 -21.0 2.5
        vertex 32.000999450683594 -21.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 93.0 19.0 2.5
        vertex 93.0 -8.5 2.5
        vertex 110.0 -20.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 29.5 -8.5 2.5
        vertex 93.0 -8.5 2.5
        vertex 93.0 19.0 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 93.0 -8.5 2.5
        vertex 93.0 -11.0 2.5
        vertex 110.0 -20.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex 150.0 100.0 0.0
        vertex -150.0 100.0 0.0
        vertex -150.0 100.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -150.0 100.0 2.5
        vertex 150.0 100.0 2.5
        vertex 150.0 100.0 0.0
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -99.0 32.599998474121094
        vertex -39.0 -54.0 32.099998474121094
        vertex -39.0 -9.0 32.599998474121094
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -9.0 2.5999999046325684
        vertex -39.0 -9.0 32.599998474121094
        vertex -39.0 -30.0 29.600000381469727
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -30.0 29.600000381469727
        vertex -39.0 -54.0 29.600000381469727
        vertex -39.0 -9.0 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -39.0 -9.0 2.5999999046325684
        vertex -39.0 -54.0 29.600000381469727
        vertex -39.0 -99.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 0.0 -77.5 2.5
        vertex 7.998000144958496 -77.5 2.5
        vertex 29.5 -8.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex 7.998000144958496 -77.5 2.5
        vertex 22.003000259399414 -77.5 2.5
        vertex 29.5 -8.5 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -81.0 -8.0 2.5
        vertex -108.5 -8.0 2.5999999046325684
        vertex -81.0 -8.0 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -109.99800109863281 -8.0 2.5
        vertex -108.5 -8.0 2.5999999046325684
        vertex -81.0 -8.0 2.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -108.5 -8.0 32.5
        vertex -81.0 -8.0 32.5
        vertex -108.5 -8.0 2.5999999046325684
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -81.0 -10.5 32.5
        vertex -81.0 -10.5 2.5
        vertex -81.0 -8.0 32.5
    endloop
endfacet
facet normal 0.0 1.0 0.0
    outer loop
        vertex -56.99800109863281 -9.0 2.5999999046325684
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -39.0 -9.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -41.5 -11.5 32.599998474121094
        vertex -56.99800109863281 -11.5 32.599998474121094
        vertex -41.5 -11.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -41.5 -11.5 2.5999999046325684
        vertex -56.99800109863281 -11.5 32.599998474121094
        vertex -56.99800109863281 -11.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -41.5 -11.5 32.599998474121094
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -56.99800109863281 -11.5 32.599998474121094
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -81.0 -10.5 2.5
        vertex -81.0 -10.5 32.5
        vertex -108.5 -10.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -81.0 -10.5 2.5
        vertex -108.5 -10.5 2.5999999046325684
        vertex -109.99800109863281 -10.5 2.5
    endloop
endfacet
facet normal 1.0 0.0 0.0
    outer loop
        vertex -81.0 -8.0 2.5
        vertex -81.0 -8.0 32.5
        vertex -81.0 -10.5 2.5
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -39.0 -9.0 2.5999999046325684
        vertex -41.5 -11.5 2.5999999046325684
        vertex -56.99800109863281 -9.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 -1.0 0.0
    outer loop
        vertex -81.0 -10.5 32.5
        vertex -108.5 -10.5 32.5
        vertex -108.5 -10.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -108.5 -8.0 32.5
        vertex -108.5 -10.5 32.5
        vertex -81.0 -8.0 32.5
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -81.0 -10.5 32.5
        vertex -81.0 -8.0 32.5
        vertex -108.5 -10.5 32.5
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -56.99800109863281 -9.0 2.5999999046325684
        vertex -56.99800109863281 -11.5 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -56.99800109863281 -11.5 32.599998474121094
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -56.99800109863281 -11.5 2.5999999046325684
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -41.5 -11.5 2.5999999046325684
        vertex -41.5 -99.0 32.599998474121094
        vertex -41.5 -11.5 32.599998474121094
    endloop
endfacet
facet normal -1.0 0.0 0.0
    outer loop
        vertex -41.5 -99.0 2.5999999046325684
        vertex -41.5 -99.0 32.599998474121094
        vertex -41.5 -11.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -56.99800109863281 -9.0 32.599998474121094
        vertex -41.5 -11.5 32.599998474121094
        vertex -39.0 -9.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -41.5 -11.5 32.599998474121094
        vertex -41.5 -99.0 32.599998474121094
        vertex -39.0 -99.0 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 1.0
    outer loop
        vertex -39.0 -99.0 32.599998474121094
        vertex -39.0 -9.0 32.599998474121094
        vertex -41.5 -11.5 32.599998474121094
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -56.99800109863281 -11.5 2.5999999046325684
        vertex -56.99800109863281 -9.0 2.5999999046325684
        vertex -41.5 -11.5 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -39.0 -99.0 2.5999999046325684
        vertex -41.5 -11.5 2.5999999046325684
        vertex -39.0 -9.0 2.5999999046325684
    endloop
endfacet
facet normal 0.0 0.0 -1.0
    outer loop
        vertex -41.5 -11.5 2.5999999046325684
        vertex -39.0 -99.0 2.5999999046325684
        vertex -41.5 -99.0 2.5999999046325684
    endloop
endfacet
endsolid
```
