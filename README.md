# IndigoTransitions

IndigoTransitions is a responsive animation library designed to enhance user interfaces with smooth, engaging animations that are easy to integrate into any web project. Built with a focus on flexibility and responsiveness, this library provides a collection of CSS animations that adapt seamlessly across various devices and screen sizes.

## Features
- **Diverse Animation Categories**: Explore a wide range of animations, including entrance and exit effects, hover animations, loading indicators, and smooth transitions, all crafted to elevate user experience.
- **Mobile-Friendly Design**: All animations are optimized for mobile devices, ensuring a fluid experience on smartphones and tablets.
- **Easy Integration**: Simple usage with straightforward CSS classes, allowing developers to implement animations with minimal effort.
- **Customizable Options**: Tailor animations to fit your project’s design language by easily adjusting duration, timing functions, and other parameters.
- **Demo and Documentation**: Comprehensive documentation and an interactive demo page showcase each animation, providing code snippets for quick reference and implementation.

## Installation

To use IndigoTransitions in your project, you can include the CSS file directly or add it via your package manager.

### Using CDN
Add the following line to your HTML file:
```html
<link rel="stylesheet" href="https://cdn.example.com/indigotransitions/animation.css">
```

### Using npm
Install IndigoTransitions via npm:
```sh
npm install indigotransitions
```
Then import it in your project:
```css
@import 'indigotransitions/animation.css';
```

## Usage

To use IndigoTransitions animations, simply add the corresponding CSS class to the HTML element you want to animate. Below are some examples:

### HTML Example
```html
<div class="fade-in">Fade In Animation</div>
<div class="slide-in-left">Slide In From Left</div>
<div class="bounce">Bounce Animation</div>
```

### JavaScript Interaction
To reset animations on user interaction, you can use JavaScript to remove and reapply the animation class:
```js
document.querySelectorAll('.demo-box').forEach(box => {
    box.addEventListener('click', () => {
        box.style.animation = 'none';
        box.offsetHeight; // Trigger reflow to restart animation
        box.style.animation = '';
    });
});
```

## Animation Classes
IndigoTransitions provides a variety of pre-defined animation classes:
- **fade-in**: Fades in the element smoothly.
- **slide-in-left**: Slides in from the left side.
- **slide-in-right**: Slides in from the right side.
- **bounce**: Creates a bouncing effect.
- **rotate-in**: Rotates the element in.
- **rotate-out**: Rotates the element out.
- **zoom-in**: Zooms in the element.
- **zoom-out**: Zooms out the element.
- **pulse**: Creates a pulsing effect.
- **flip**: Flips the element.
- **flip-in-x**: Flips in along the X-axis.
- **shake**: Creates a shaking effect.
- **wobble**: Adds a wobbly animation.

## Customizing Animations
You can easily customize the animations by adjusting properties such as `animation-duration`, `animation-timing-function`, and more:

```css
.bounce {
  animation-duration: 3s;
  animation-timing-function: ease-in-out;
}
```

## Demo
You can view and interact with a live demo of IndigoTransitions animations by opening the `demo/index.html` file included in the repository. The demo page contains examples of each animation to help you understand how to use them effectively.

## Contributing
We welcome contributions to IndigoTransitions! If you have an idea for a new animation or an improvement, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

