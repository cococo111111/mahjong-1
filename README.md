This is a simple Mahjong solitaire game. It is written in C# and
uses the logos of various open source related projects as tile images.

![Screenshot](/Mahjong.png)

The game was only a quick POC for another implementation written in Scala.

There are no advanced features like a scoreboard or different tile setups,
but there are two other notable things included:
- Play on a web interface using the embedded web server and HTML5/jQuery
  (Same graphics as the WinForms UI, you can reach the web interface at
  http://localhost:8080/!)
- Setup Editor for creating your own Tile-Setups
  (Start with "Mahjong.exe -editor")

You have to replace the "setup.txt" to play with your own tile setup.

The web interface was successfully tested in Firefox, Chrome and Opera.
IE 9 does display the tiles correctly, but does not accept any user input.

Included third party (open source) software:
jQuery - http://jquery.com/
httpserver - http://webserver.codeplex.com/

I removed the System.Web dependency of the httpserver, so it will run
on the .Net _Client_ Profile. To achieve this, I used this file:
http://google-gdata.googlecode.com/svn/trunk/clients/cs/src/core/HttpUtility.cs