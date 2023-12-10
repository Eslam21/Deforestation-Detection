# Deforestation-Detection

The data here is a 4 Landsat-8 half-year image composites, covering a small area on the Malaysia Peninsular. 
Landsat-8 is the eighth NASA satellite of the landsat series. It measures reflectance in the so-called optical part of 
the electromagnetic spectrum. Besides the familiar blue, green and red, it measures near-infrared, shortwave, and thermal infrared.

2016_1 RGB image looks like this:

![pm_2016_1_rgb](https://storage.googleapis.com/s11-litmustest/Screenshot%20from%202018-02-01%2014-00-16.png)

The Landsat bands are particularly suited for detecting vegetation characteristics. A forest for the human eye 
is mostly green and no forest is often brownish or grey. For Landsat, a more effective measure of the forest is the 
relative reflectance in the shortwave infrared compared to near-infrared. Using Landsat's `1.5 * swir / nir` 
will give high values for bare areas and low values for forested areas.

### The deforestation detector
The task is to use the numpy arrays you can now create to identify **which** pixels in the sample data got deforested and **when** this has happened.

