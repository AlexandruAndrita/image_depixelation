The purpose of the project is image depixelation, starting from the original image (into grayscale format), learning the image and then reconstructing the pixeled zone. 

The following steps have been performed so far: <br/>

[ x ] a function ```validate_images``` created in order to validate the images. Some of the criteria would be: size of the image is not more that 250kB, the image should be in ```.JPG``` format, the image is either ```RGB``` or ```L``` (grayscale), the image could be read using the ```pillow``` module and the variance of image is larger than 0 (i.e. there is not just one common pixel in the image data). <br/><br/>
[ x ] a log file is created in order to keep track of the images from the dataset that do not meet the requirements presented above. <br/><br/>
[ x ] a function ```to_grayscale``` created in order to convert the ```RGB``` images to grayscale ones - the original image remains unchanged. The transformation process is done on a copy. <br/><br/>
[ x ] a function ```prepare_image``` created that pixels a specified part of the image (part given by the specified coordinates). The pixelation process is done on the grayscale version, the 'original grayscale' remains unchanged. Thus, after calling this method, we have the following results: <br/>
 - ```pixelated_image``` = the original image with the pixeled zone <br/>
 - ```known_array``` = boolean array that contains ```False``` when the image is pixeled and ```True``` everywhere else <br/>
 - ```target_array``` = the zone that has been pixeled - ground truth <br/>

Further details will be provided soon. 
