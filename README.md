# Heart present
This is a 3d heart that is intended to be a present for my first girlfriend.

I'm using SpaceClaim to build these models and each of the versions I have an exported stl file ready to be printed. All parts are intended to be printed without support which makes everything sharp.

The equations of the heart in these models (which is taken from [here](https://www.quora.com/What-is-the-equation-that-gives-you-a-heart-on-the-graph)) are:

- a * sqrt(1 - (|x| - 1) ^ 2)
- a * (acos(1 - |x|) - pi)

Keep in mind a few things however:

1. The range of x is [-2, 2] and is undefined when x is outside of it. This can make some 3d modelling tools throw some errors at the boundaries {-2, 2}. So you might want to put -1.99999 and 1.99999 respectively
2. All the units are measured in millimeters except when specified.
3. The a variable will be 30 when the width of the heart is 12cm.

## Model 1

This is a small 5cm x 5cm box with a lid intended to see if carved out letters are ok and whether the lid fits the container. Both pieces have 3 number 3s and are of different sizes and looks like this:

![](https://i.imgur.com/T1ly2v7.jpg)

## Model 2

This is the second model which is a box with a container part and a lid.
The container:

- Total height: 7mm
- Base height: 3mm
- Usable storage height: 4mm
- Inner space is a heart with a width of 12cm
- Outer boundary is a heart with a width of 13cm and is shifted upwards respective to the inner heart 2mm
- Inner space: 90 pi cm^2
- Inner volume/capacity: 36 pi cm^3

The lid:

- Total height: 5mm
- Popped out height: 2mm
- Popped out is a heart with a width of 12cm
- The lid's top part is a heart with a width of 13cm

Together:

- Total height: 12mm
- Usable storage height: 2mm
- Inner volume/capacity: 18cm^3

Here's what it looks like:

![](https://i.imgur.com/rwJJzlU.png)

## Model 3

This is the third model which is still the heart from model 2 with the base bent outwards to open the heart easily. This doesn't add much to model 2 and is meant to be sort of a template only. Other models that extends this template can change their usable volume by adjusting the variable "b" in the specs below:

The container:
- Total height: (7 + 4 + b)mm
- Base height: 3mm
- Usable storage height: (8 + b)mm
- Bent outer body's height/slanted part: 4mm
- Straight outer body's height: (7 + b)mm
- Inner volume/capacity: (8 + b) * 9 pi cm^3

The lid:
- Total height: (5 + 2)mm
- Stick out height: 2mm
- Slanted/bent part's height: 2mm
- Straight part's height: 3mm

Together:

- Total height: (16 + b)mm
- Straight part's height: (7 + 3 + b)mm
- Slanted/bent part's height: 6mm
- Usable storage height: (6 + b)mm
- Inner volume/capacity: (6 + b) * 9 pi cm^3

## Model 4

This model's core is essentially model 3 with b = 9.5.

I plan to have 2 layers of chocolate with a 3mm of paper, totaling up to 15.5mm of usable storage height which we can deduce that b = 9.5.

Besides that, I have also build a strongback-like structure that will support the heart and allows it to be packaged into a ship-able present. There're 3 schemas to do this:

### Schema 1

A strongback that supports the straight part only and leaves the front and back bent parts naked. This almost makes it a box but not quite. Involves the following files:

- [model 4 strongback without cover](https://github.com/157239n/Heart-present/blob/master/model%204%20strongback%20without%20cover.scdoc) (SpaceClaim file)

### Schema 2

A strongback that supports the straight part and have 4 circle fourths covering the front and back parts. This makes the heart into a box. However, this require supports which won't give nice results in a 3d printer so I use the 3rd schema instead. Involves the following files:

- [model 4 strongback with cover](https://github.com/157239n/Heart-present/blob/master/model%204%20strongback%20with%20cover.scdoc) (SpaceClaim file)

### Schema 3

A strongback that supports the straight part and have 4 circle fourths covering the front and back parts and makes the heart into a box. This involves:

- Knotched left and right sides of schema 1: [model 4 strongback knotch core side](https://github.com/157239n/Heart-present/blob/master/model%204%20strongback%20knotch%20core%20side.stl) (stl file)
- Knotched front cover: [model 4 strongback knotch lid](https://github.com/157239n/Heart-present/blob/master/model%204%20strongback%20knotch%20lid.stl) (stl file)
- Knotched back cover: [model 4 strongback knotch container](https://github.com/157239n/Heart-present/blob/master/model%204%20strongback%20knotch%20container.stl) (stl file)

It's intended to first assemble left and right core sides first and then put together the front and back cover later with rubber bands or cloth or a wire of some kind.

## Final product

The main body:

![](https://i.imgur.com/MwqAJY9.jpg)

The lid:

![](https://i.imgur.com/QYkAOqX.jpg)

Direct view with strongback:

![](https://i.imgur.com/rRUXevy.jpg)

Angled view with strongback:

![](https://i.imgur.com/UrjFdpm.jpg)

Paper message inside:

![](https://i.imgur.com/suyvtVl.jpg)
