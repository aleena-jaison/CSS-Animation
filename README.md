# Bouncing Ball Animation

This project demonstrates a simple CSS animation of a bouncing ball. The ball bounces vertically with a shadow effect, giving it a dynamic and realistic look. The animation is created using **CSS keyframes** and **transform** properties for smooth motion.

## Features

- **Bouncing Ball Animation**: The ball moves up and down with a smooth bouncing effect.
- **Shadow Effect**: As the ball bounces, the shadow changes in position and intensity, adding realism.
- **Responsive Design**: The ball is centered on the screen, ensuring a good presentation on all screen sizes.

## Getting Started

To view the animation, simply open the `index.html` file in any modern web browser (Google Chrome, Firefox, Safari, etc.).

### Installation

1. **Clone the repository**:
    - You can clone the repository using Git:
    - Or, download the ZIP file of the project and extract it.

2. **Open the project**:
    - Open the `index.html` file in your preferred text editor (e.g., VSCode, Sublime Text).
    - You can also open it directly in your web browser to view the bouncing ball animation.

### File Overview

- **index.html**: Contains the structure of the HTML page and links the necessary CSS file.
- **styles.css**: Contains the CSS styling and animation for the ball and its bouncing behavior.
- **Keyframes**: The `@keyframes` in the `styles.css` define the movement and shadow effect for the bouncing animation.

### Customizing the Animation

If you want to customize the animation, you can adjust the following properties in the `styles.css`:

- **Ball Size**: Modify the `width` and `height` values in the `.ball` class to change the size of the ball.
- **Bounce Height**: Change the values in the `translateY()` functions in the `@keyframes` to control how high the ball bounces.
- **Animation Speed**: Adjust the `3s` duration in the `animation` property to make the bounce slower or faster.
- **Ball Color**: Change the `background-color` property in the `.ball` class to any color you prefer.
- **Shadow Effects**: Customize the `box-shadow` values in the keyframes to change the shadow size and intensity.

## Example Customization

To make the ball bounce higher and move slower:

```css
/* Increase bounce height and slower animation */
@keyframes bounce {
    0% {
        transform: translateY(100px); /* Start lower */
        box-shadow: 0 10px 15px rgba(128, 128, 128, 0.3);
    }
    25% {
        transform: translateY(-250px); /* Increased bounce height */
    }
    50% {
        transform: translateY(0);
    }
    75% {
        transform: translateY(-200px);
    }
    100% {
        transform: translateY(0);
    }
}

/* Slower animation duration */
.ball {
    animation: bounce 6s ease-in-out infinite;
}
    
