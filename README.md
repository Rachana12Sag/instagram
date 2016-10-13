# Introduction:

   Instagram is an online mobile photo-sharing, video-sharing, and social networking service that enables its users to take pictures and videos, and share them either publicly or privately on the app, as well as through a variety of other social networking platforms, such as Facebook, Twitter, Tumblr, and Flickr. 
   Originally, a distinctive feature was that it confined photos to a square shape, similar to Kodak Instamatic and Polaroid SX-70 images, in contrast to the 4:3 aspect ratio typically used by mobile device cameras. 
In August 2015, version 7.5 was released, allowing users to upload media captured in any aspect ratio. 
   Users can also apply digital filters to their images. 
   Videos on Instagram debuted with a 640x640 fixed resolution and maximum 15-second limit in June 2013; resolutions now include up to 1080p since July 2015 and length is now up to 60 seconds since January 2016.


# The original Instagram website and API client

This was the first web app that displayed profiles of Instagram users online. It
was done by using Instagrams private API. Despite the fact that Instagram now
displays user profiles on their official site, [this app is still online][web].

The process of sniffing out their private API is described in my post:
[Creating the missing Instagram web interface][story].

Nowadays [Instagram has an official API][official] and many 3rd-party web sites
that do interesting things with people's photos and data.

## The code

* The app is mostly contained in a single file: [`app.rb`][app]
* The lightweight Ruby API client it is using: [`instagram.rb`][client]
* The legacy API client (**not to be used**) is in `lib/`.


[web]: http://instagram.heroku.com
[official]: http://instagram.com/developer/
[story]: http://mislav.uniqpath.com/2010/12/instagram-web/
[app]: https://github.com/mislav/instagram/blob/master/app.rb
[client]: https://github.com/mislav/instagram/blob/master/instagram.rb
