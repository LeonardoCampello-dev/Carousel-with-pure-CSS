<h1 align="center">
    <img src="https://images.vexels.com/media/users/3/200371/isolated/lists/039bfb98547756d2f159286c9b51fa68-carnival-carousel-color.png">
</h1>

[![forthebadge](https://forthebadge.com/images/badges/for-you.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/uses-css.svg)](https://forthebadge.com)
[![forthebadge](https://forthebadge.com/images/badges/built-with-swag.svg)](https://forthebadge.com)

## 📑 Description

Project developed from a video on the [Rocketseat YouTube channel.](https://www.youtube.com/channel/UCSfwM5u0Kce6Cce8_S72olg) 💜

- [x] Video: [Criando um Carousel do Zero só com CSS | Code/Drops #39](https://www.youtube.com/watch?v=SGwHpzgqzgk) 🎥

## 📺 Demonstration

![Carousel](/assets/carousel.gif)

## 👨‍💻 CSS code

``` css

@import url('https://fonts.googleapis.com/css2?family=Happy+Monkey&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    display: grid;
    place-items: center;
    height: 100vh;
    background-color: #373C3F;
}

.title {
    display: grid;
    grid-template-columns: 1fr 100px;
    gap: 24px;
    align-items: center;
}

.title img {
    width: 64px;
    height: 64px;
}

.title h1 {
    font-family: 'Happy Monkey', cursive;
    font-size: 40px;
    line-height: 50px;
    color: #CE0802;
    text-shadow: 1px 1px 2px #228DC3;
}

#items-wrapper {
    width: 100vw;
}

#items {
    display: flex;
    overflow-x: auto;
    scroll-snap-type: x mandatory;
    -webkit-overflow-scrolling: touch;
    scroll-behavior: smooth;
}

.item {
    flex: none;
    width: 100%;
    height: 400px;
    scroll-snap-align: start;
    pointer-events: none;
}

img {
    width: 100%;
    height: 100%;

    object-fit: cover;
}

```