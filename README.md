# dmis-facebook

This is a rewrite of Facebook Album Photos(jquery) 
- http://www.jqueryscript.net/social-media/jQuery-Plugin-To-Display-Photos-From-Your-Facebook-Album-Facebook-Photos.html

##Additional Components

* bootstrap carousel photo viewer with captions
* uploaded time 

This just dumps a set of photos from a [Facebook](http://facebook.com) album into an html object.

## Options

* **albumURL** (required): full URL to a  Facebook Album
* **limit**: limit to the last X photos (default: 10)
* **imgSize**: size of the image (default: medium)
	* original
	* huge
	* x-large
	* large
	* medium
	* small
	* x-small

For more information on image sizes, check out the [Facebook Graph Photos API](https://developers.facebook.com/docs/reference/api/photo/).

## Example

[Play around with it on jsFiddle] 
For latter modified demonstration, you can refer to http://jsfiddle.net/shumanbaral/624v9abL/1/  
For previous demonstration, you can refer to (http://jsfiddle.net/chris79/cEN9v/2/)


	$(document).ready(function(){
		$("#slideshow").facebookAlbumPhotos({
			'albumURL': 'https://www.facebook.com/media/set/?set=a.247569245406039.1073741837.194753444020953',
			'limit': 10, //The number of photos to be shown in carousel
			'evt':"Nepali cricket team" //Heading of the album 
		});
	});

