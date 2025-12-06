# CSS Animations — Learning Examples

This repository contains different CSS animation examples, each placed in its own HTML and CSS file.
It is designed to help beginners understand how CSS animations work, how to define keyframes, and how to use all animation-related properties.

## What Are CSS Animations?
CSS animations let you smoothly change CSS properties over time.
They are made of two main parts:

## 1. `@keyframes`
   `@keyframes` defines the stages of an animation:
```
@keyframes bounce {
  from {
    transform: translateY(0);
  }
  to {
    transform: translateY(-30px);
  }
}
```
Or using percentages for more complex motion:
```
@keyframes fadeInOut {
  0%, 100% {
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
}
```

## 2. Animation Properties
Animation properties control how the animation behaves when applied to an element. Below are all the important animation properties and what they do:

### animation-name
The name of the keyframes animation.
```
animation-name: bounce;
```

### animation-duration
How long it takes to complete one animation cycle.
```
animation-duration: 2s;
```

### animation-timing-function
Controls the speed curve of the animation. Examples:
- linear
- ease
- ease-in
- ease-out
- ease-in-out
steps(n)
- cubic-bezier(x1, y1, x2, y2)
```
animation-timing-function: ease-in-out;
```

### animation-delay
How long to wait before the animation starts.
```
animation-delay: 1s;
```

### animation-iteration-count
How many times the animation should repeat.
Values:
- 1
- 2
- infinite
```
animation-iteration-count: infinite;
```

### animation-direction
Controls how the animation runs on each cycle.
Options:
- normal
- reverse
- alternate
- alternate-reverse
```
animation-direction: alternate;
```

### animation-fill-mode
Defines the style before and after the animation runs.
Values:
- none
- forwards
- backwards
- both
```
animation-fill-mode: forwards;
```

### animation-play-state
Used to pause or resume animations.
```
animation-play-state: paused;
```

### Shorthand
You can combine the properties like this:
```
animation: bounce 1.5s ease-in-out infinite alternate forwards;
```

## Example Animations Included
Below are the animations included in this project.
- Bounce
- Fade In
- Color Change
- Loader
- Slide Fade
- Typing Text
