# Media

## - Play Bunny -

Code:

```html
<!DOCTYPE html> 
<html> 
    <body> 
        <video width="400" controls>
            <source src="./videos/mov_bbb.mp4" type="video/mp4">
            <source src="./videos/mov_bbb.ogv" type="video/ogg">
            Your browser does not support HTML video.
        </video>

        <p>
            Video courtesy of 
            <a href="https://www.bigbuckbunny.org/" target="_blank">Big Buck Bunny</a>.
        </p>
    </body> 
</html>
```

Output:

<!DOCTYPE html> 
<html> 
    <body> 
        <video width="400" controls>
            <source src="./videos/mov_bbb.mp4" type="video/mp4">
            <source src="./videos/mov_bbb.ogv" type="video/ogg">
            Your browser does not support HTML video.
        </video>

        <p>
            Video courtesy of 
            <a href="https://www.bigbuckbunny.org/" target="_blank">Big Buck Bunny</a>.
        </p>
    </body> 
</html>

## - Play bear video with controls -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <video width="320" height="240" controls>
            <source src="./videos/movie.mp4" type="video/mp4">
            <source src="./videos/movie.ogv" type="video/ogg">
            Your browser does not support the video tag.
        </video>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <video width="320" height="240" controls>
            <source src="./videos/movie.mp4" type="video/mp4">
            <source src="./videos/movie.ogv" type="video/ogg">
            Your browser does not support the video tag.
        </video>
    </body>
</html>

## - Play bear video with autoplay -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <!-- Some modern browsers like chrome will not auto-play your video if it's not muted. -->
        <video width="320" height="240" muted autoplay>
            <source src="./videos/movie.mp4" type="video/mp4">
            <source src="./videos/movie.ogv" type="video/ogg">
            Your browser does not support the video tag.
        </video>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <!-- Some modern browsers like chrome will not auto-play your video if it's not muted. -->
        <video width="320" height="240" muted autoplay>
            <source src="./videos/movie.mp4" type="video/mp4">
            <source src="./videos/movie.ogv" type="video/ogg">
            Your browser does not support the video tag.
        </video>
    </body>
</html>

## - Play Horse sound with controls -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <audio controls>
            <source src="./audios/horse.ogv" type="audio/ogg">
            <source src="./audios/horse.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <audio controls>
            <source src="./audios/horse.ogv" type="audio/ogg">
            <source src="./audios/horse.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
    </body>
</html>

## - Play a YouTube video in HTML -

Code:

```html
<!DOCTYPE html>
<html>
    <body>
        <iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
    </body>
</html>
```

Output:

<!DOCTYPE html>
<html>
    <body>
        <iframe width="420" height="345" src="https://www.youtube.com/embed/tgbNymZ7vqY"></iframe>
    </body>
</html>