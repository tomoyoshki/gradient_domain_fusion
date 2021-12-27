# Gradient Domain Fusion

## Core

### Poisson Blending

#### Original Images

##### Background Image

<img src = "./assets/poisson_1_bg.JPG" style="zoom:10%"/>

-   Here is an image I took at Tokyo Airport

<div style="page-break-after: always" />

##### Object Image

<img src = "./assets/poisson_1_obj.jpeg" style="zoom:20%"/>

-   Here is the grainger Bob statue near the Grainger Library

<div style="page-break-after: always" />

#### Pasted image with source pixels directly copied onto target background region

<img src = "./assets/poisson_1_paste.png" style="zoom:100%"/>

<div style="page-break-after: always" />

#### Final Blend Result

<img src = "./assets/poisson_1_blend.png" style="zoom:100%"/>

<div style="page-break-after: always" />

#### One more good result

##### Direct pasting

<img src="./assets/poisson_2_paste.png" />

<div style="page-break-after: always" />

##### Poisson Blending

<img src="./assets/poisson_2_blend.png" />

<div style="page-break-after: always" />

#### One failure case

<img src = "./assets/poisson_fail.png" />

<div style="page-break-after: always" />

### Mixed Gradients

#### Original Images

##### Object Image

<img src="./assets/mario.png" style="zoom:30%"/>

<div style="page-break-after: always" />

##### Background Image

<img src="./assets/wall.jpeg" style="zoom:20%"/>

<div style="page-break-after: always" />

#### Pasted image with source pixels directly copied onto target background region

<img src="./assets/poisson_2_paste.png" />

<div style="page-break-after: always" />

#### Final Blend Result

<img src="./assets/mixed_2_blend.png" />

-   This is the Mixed Blend result, and it looks much natural compared to the Poisson result I presented earlier. In our Poisson blending result, there is a blurred line between the two, but Mixed Blend does not have such issue. In addition to this, both characters also have the texture of the wall and are more transparent, this makes it look like its painted to the wall. 

<div style="page-break-after: always" />

## Bell & Whistles 

### Color2Gray

-   For my own `Color2Gray` implementation, I have used Gradient domain methods similar to part 3 to preserve the highest gradient out of the red, green, and blue layer at a specific pixel. This allows us to preserve the highest gradient of any of the layer to preserve the original information and project it to the gray image. 

#### Color 4

<img src = "./assets/color4.png" style="zoom:40%"/>

<div style="page-break-after: always" />

#### Gray 4

<img src="./assets/gray4.png" style="zoom:20%"/>

#### Color 8

<img src="./assets/color8.png" style="zoom:40%"/>

#### Gray 8

<img src="./assets/gray8.png" style="zoom:40%"/>

#### Color natural image

<img src="assets/color_nature.png"/>

<div style="page-break-after: always" />

#### Gray natural image

<img src="./assets/gray_nature.png" />

-   We can see that the details of the image are preserved well

<div style="page-break-after: always" />

### Laplacian Pyramid Blending

-   <img src="./assets/laplacian_illustration.png" style="zoom:70%"/>

<div style="page-break-after: always" />

#### Original Images

##### Background Image

<img src = "./assets/lap_bg.png" />

<div style="page-break-after: always" />

##### Object Image

<img src = "./assets/lap_obj.png" style="zoom:30%">

#### Direct Pasting

<img src="./assets/lap_paste.png" style="zoom:50%"/>

<div style="page-break-after: always" />

#### Poisson Blend

<img src="./assets/lap_poisson.png" style="zoom:50%"/>

#### Mixed Blend 

<img src="./assets/lap_mixed.png" style="zoom:50%"/>

#### Laplacian Blending

<img src="./assets/lap_lap.png" style="zoom:50%"/>

