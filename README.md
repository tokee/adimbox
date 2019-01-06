# adimbox

Nothing to see here besides some ideas of a future product.

- Toke Eskildsen, te@ekot.dk

## Background

The Windows-program [JPEGCrops](http://ekot.dk/programmer/JPEGCrops/) as well as another private Windows-program allows the user to operate on multiple images at the same time. The idea is to re-implement both programs in Java. This project is about their shared component. Notes below are written primarily from a JPEGCrops perspective.

## Plans

JPEGCrops makes it possible to crop a batch of JPEG images losslessly. The images are presented in a grid and a crop-box is visible for each image. It is possible to synchronize size and position of crop-boxes between images, so that they all move at the same time.

adimbox uses the [MVC](https://en.wikipedia.org/wiki/Model%E2%80%93view%E2%80%93controller) pattern with a focus on minimizing the memory overhead of the model part, allowing editing of thousands of images at the same time.

## Minimum viable product

### Model

Minimum

* Image source-path & destination-name
* Image type & dimensions
* Crop-area position & dimensions
* Crop-area aspect ratio

Ideas

* Align to JPEG MCU (boolean)
* Rotation
* Sharpness
* Contrast

### View

Minimum

* Display image
* Display crop-box 
* Mouse-based adjustment of crop-box position & dimensions

Ideas

* Overlays etc. from JPEGCrops

### Control

Ideas

* Synchronization of crops

