# covert-radio

This is a Covert Radio disguised in a binder. The parts are as follows:
Anker Powercore 10000mAh Portable Battery
Anker 4 Port USB Dock (Not strictly necessary but to allow for ethernet to be used easily without an obvious cable snaking out, and to also allow the Radio to be situated inside the binder it was the best choice)
Raspberry Pi 3 B v2, Running OpenWebRx+
RTL SDR Blog v4 (avoid counterfits!)
Dipole Antenna w/ Coaxial Connector

Pictures:



Build Instructions:
First I harvested a binder. Breaking off the Rings was trivial, using pliers. Designing this with my backpack in mind, I cut the sides of it to allow it to squeeze into a laptop slot in the bag. To make it look pretty, I painted over the cut edges with white paint.
To make the thing look like a normal binder not something used for other purposes, I cut pieces of scrap paper to the size of the binder allowing room for them to stick out. I did it in three sections for the top, bottom and side. By cutting tons of paper and then glueing the far side of it, it would make the paper look like it was springing out of the binder. A thing to note is to vary the size so it looks natural. 
After doing this three times I split the long side horizontally on the top and bottom just enough for them to slide in, so it wouldnt be obvious.

The Next step is to measure your components and hot glue them down. I made a simple 3d Model using the scales of the parts and then printed out a 2d version and traced, then glued cardboard on the traced lines. 
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
