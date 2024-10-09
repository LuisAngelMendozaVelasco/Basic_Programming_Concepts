# Image Sprites

## An image sprite

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #home { width: 46px;
                    height: 44px;
                    background: url(../data/images/img_navsprites.gif) 0 0;}

            #next { width: 43px;
                    height: 44px;
                    background: url(../data/images/img_navsprites.gif) -91px 0;}
        </style>
    </head>
    <body>
        <img id="home" src="../data/images/img_trans.gif" width="1" height="1">
        <img id="next" src="../data/images/img_trans.gif" width="1" height="1">
    </body>
</html>
```

Output:

[Click here!](./Image_Sprites/Example_1.html)

## An image sprite - a navigation list

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #navlist {position: relative;}

            #navlist li {   margin: 0;
                            padding: 0;
                            list-style: none;
                            position: absolute;
                            top: 0;}

            #navlist li, #navlist a {   height: 44px;
                                        display: block;}

            #home { left: 0px;
                    width: 46px;
                    background: url('../data/images/img_navsprites.gif') 0 0;}

            #prev { left: 63px;
                    width: 43px;
                    background: url('../data/images/img_navsprites.gif') -47px 0;}

            #next { left: 129px;
                    width: 43px;
                    background: url('../data/images/img_navsprites.gif') -91px 0;}
        </style>
    </head>
    <body>
        <ul id="navlist">
            <li id="home"><a href="https://www.w3schools.com/css/default.asp"></a></li>
            <li id="prev"><a href="https://www.w3schools.com/css/css_intro.asp"></a></li>
            <li id="next"><a href="https://www.w3schools.com/css/css_syntax.asp"></a></li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Image_Sprites/Example_2.html)

## An image sprite with hover effect

Code: 

```html
<!DOCTYPE html>
<html>
    <head>
        <style>
            #navlist {position: relative;}

            #navlist li {   margin: 0;
                            padding: 0;
                            list-style: none;
                            position: absolute;
                            top: 0;}

            #navlist li, #navlist a {   height: 44px;
                                        display: block;}

            #home { left: 0px;
                    width: 46px;
                    background: url('../data/images/img_navsprites_hover.gif') 0 0;}

            #prev { left: 63px;
                    width: 43px;
                    background: url('../data/images/img_navsprites_hover.gif') -47px 0;}

            #next { left: 129px;
                    width: 43px;
                    background: url('../data/images/img_navsprites_hover.gif') -91px 0;}

            #home a:hover {background: url('../data/images/img_navsprites_hover.gif') 0 -45px;}

            #prev a:hover {background: url('../data/images/img_navsprites_hover.gif') -47px -45px;}

            #next a:hover {background: url('../data/images/img_navsprites_hover.gif') -91px -45px;}
        </style>
    </head>
    <body>
        <ul id="navlist">
            <li id="home"><a href="https://www.w3schools.com/css/default.asp"></a></li>
            <li id="prev"><a href="https://www.w3schools.com/css/css_intro.asp"></a></li>
            <li id="next"><a href="https://www.w3schools.com/css/css_syntax.asp"></a></li>
        </ul>
    </body>
</html>
```

Output:

[Click here!](./Image_Sprites/Example_3.html)