# Colorme

####  _This application was developed during the immersive course at Code Chrysalis_  <br><br>

"What was the name of this color?
Is neither "red" nor "blue". It's a name more subtle."　　

Color names are not just signes. They are delicate, emotional, and can evoke forgotten memories. With this app, you can find the ancient name of the color of a photo.  

---
## Installing locally

### Backend  
Assuming python has already been installed, clone [the backend repository](https://github.com/miomaeshima/Colorme-backend) and enter the commands below in the terminal.  
```
$ pip install flask flask_cors openpyxl
$ virtualenv 
$ env\Scrips\activate 
$ python app.py
```

### Frontend  
Clone [the frontend repository](https://github.com/miomaeshima/Colorme-frontend) and enter the commands below in the terminal.  
```
$ npm install or yarn 
$ npm http-server or yarn http-server
```
Open localhost:8080.  

## How to use  
Add your images in the img file to get the name of color in your images.  

This app has a Japanese traditional color pallete containing 712 colors. Each color has RGB value and its ancient name.

<p align="center"><img src="./img/cherry.png" width="60%"></p>

For example, clicking the image above, the closest color to the color used most in the picture is searched from the palette, and its tranditional name is displayed. The background color is the found color.

<p align="center"><img src="./img/cherry-name.png" width="60%"></p>

The closeness of colors in the pallet to the color in the picture is assessed based on the distance between 3D cordinates of rgb values. 


<p align="center"><img src="./img/rgb3d.png" width="300px"></p>


If the main color of a picture is a, color c is closer than color b.

___
## Technology

Frontend:　HTML, CSS, HTML, CSS, JavaScript, [color-thief](https://github.com/lokesh/color-thief)   
Backend:　Python
___
## Future features

1．Build a demo site  
2．Allow select file from the device  
3．Allow uploading images to the demo site  
4．Switch between pallets (e.g. between Japanese to English color name pallets)
5. Switch the font color to what is appropriate for the background (e.g. white font on dark color) 