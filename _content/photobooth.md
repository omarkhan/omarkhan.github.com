### [Khanival Photobooth][1]

When my brother got married in 2012, he wanted a photo booth so that guests
could take memorable pictures of themselves in a wide variety of silly outfits.
Being a young musician, he couldn't afford the real deal, so I was given the
task of hacking one together using an old netbook and his DSLR.

The hastily-written is code responsible for some very embarassing pictures. It
works as follows:

- A nodejs server script serves a single page with some client code.
- The client code uses `getUserMedia` to display the webcam image on the screen,
  as well as a helpful 'press a key to take a picture' message.
- When a drunk guest presses a key, the client notifies the server over
  websockets using [socket.io][2].
- The server then shells out to [gphoto2][3], which takes 4 pictures using the
  attached camera balanced just above the webcam.
- Once the pictures are ready, the server thumbnails them and notifies the
  client over websockets.
- The client displays the images, everyone is amused.

[1]: https://github.com/omarkhan/photobooth
[2]: http://socket.io/
[3]: http://www.gphoto.org/proj/gphoto2/
