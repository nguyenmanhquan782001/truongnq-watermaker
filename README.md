## it is an update of pdf-watermarker for use namespace, to use it in laravel just 

``` php
<?php
use truongnq\watermarker\PDFWatermark;
use truongnq\watermarker\PDFWatermarker;
//Specify path to image
$watermark = new PDFWatermark('C:\myimage.png'); 
 
//Specify the path to the existing pdf, the path to the new pdf file, and the watermark object
$watermarker = new PDFWatermarker('C:\test.pdf','C:\output.pdf',$watermark); 
 
//Set the position
$watermarker->setWatermarkPosition('bottomleft');
 
//Save the new PDF to its specified location
$watermarker->save(); 
?>
```

Five positions can be used. 'center' is the default.

* center
* topleft
* topright
* bottomright
* bottomleft



