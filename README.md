# imagemagick_cmyk

Drupal module to convert images to CMYK

This only works for *jpg* images, not for *png* or *gif*

Depends upon the [imagemagick module](https://www.drupal.org/project/imagemagick).

## Icc profiles are property of their owners and originally available here 

SRGB profiles: http://www.color.org/srgbprofiles.xalter#v2
CMYK profiles: http://www.eci.org/en/downloads

## More info on using profiles with imagemagick
 
[Consult the Imagemagick manual](http://www.imagemagick.org/Usage/formats/#profiles)


## Improvements

These issues would improve the module but are not fixed yet:

- check wether current image library is imagemagick
- detect wich profile the original image is using
- detect if the image format is jpg and throw an error if it isn't
- convert uploaded unsupported formats to JPG in order to enable the CMYK format
- allow the user to set the conversion quality (is now 75%, should be 100% for ideal print quality) 