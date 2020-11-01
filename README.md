# preact-animated-css
Preact component to show or hide elements with animations using [Animated.css](https://daneden.github.io/animate.css/)
This is a fork created to fix some bugs and add compatibility with animate.css version 4

## demo
(by the original author, Fareed Alnamrouti <digital.flowers@hotmail.com>)

https://digital-flowers.github.io/react-animated-css.html

## install

```bash
npm i @micheg/preact-animated-css-fork --save
```
**Note** You have to include [Animated.css](https://daneden.github.io/animate.css/) in your html page, this component is just a wrapper for it.

```html
<head>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css">
</head>
```
or even better:
```bash
npm i animate.css --save
```
If you use a bundler, for example parcel:

```javascript
import 'animate.css';
```

## how to use
very easy to use, just wrap your content with the animated component
```javascript
import 'animate.css';
import {Animated} from "@micheg/preact-animated-css-fork";

<Animated animationIn="bounceInLeft" animationOut="fadeOut" isVisible={true}>
    <div>
        hello world ;)
    </div>
</Animated>

```

then you can just toggle the  `isVisible` property to see the animation.

### Properties

- **animationIn** animation in name, default "fadeIn"
- **animationOut** animation out name, default "fadeOut"
- **animationInDelay** animation in delay, default 0
- **animationOutDelay** animation out delay, default 0
- **animationInDuration** animation in delay, default 1000
- **animationOutDuration** animation out delay, default 1000
- **style** react style property for the inner component
- **isVisible** if the component is visible or not, default true
- **innerRef** react ref property for the inner component
- **className** react className property for the inner component
- **animateOnMount** apply animationIn on mount or not, default true


### List of animation
All the following animation from animated.css are supported.

| ﻿Animation Name |
|--------------------|
| `bounce` |
| `flash` |
| `pulse` |
| `rubberBand` |
| `shakeX` |
| `shakeY` |
| `headShake` |
| `swing` |
| `tada` |
| `wobble` |
| `jello` |
| `heartBeat` |
| `backInDown` |
| `backInLeft` |
| `backInRight` |
| `backInUp` |
| `backOutDown` |
| `backOutLeft` |
| `backOutRight` |
| `backOutUp` |
| `bounceIn` |
| `bounceInDown` |
| `bounceInLeft` |
| `bounceInRight` |
| `bounceInUp` |
| `bounceOut` |
| `bounceOutDown` |
| `bounceOutLeft` |
| `bounceOutRight` |
| `bounceOutUp` |
| `fadeIn` |
| `fadeInDown` |
| `fadeInDownBig` |
| `fadeInLeft` |
| `fadeInLeftBig` |
| `fadeInRight` |
| `fadeInRightBig` |
| `fadeInUp` |
| `fadeInUpBig` |
| `fadeInTopLeft` |
| `fadeInTopRight` |
| `fadeInBottomLeft` |
| `fadeInBottomRight` |
| `fadeOut` |
| `fadeOutDown` |
| `fadeOutDownBig` |
| `fadeOutLeft` |
| `fadeOutLeftBig` |
| `fadeOutRight` |
| `fadeOutRightBig` |
| `fadeOutUp` |
| `fadeOutUpBig` |
| `fadeOutTopLeft` |
| `fadeOutTopRight` |
| `fadeOutBottomRight` |
| `fadeOutBottomLeft` |
| `Flippers` |
| `flip` |
| `flipInX` |
| `flipInY` |
| `flipOutX` |
| `flipOutY` |
| `Lightspeed` |
| `lightSpeedInRight` |
| `lightSpeedInLeft` |
| `lightSpeedOutRight` |
| `lightSpeedOutLeft` |
| `rotateIn` |
| `rotateInDownLeft` |
| `rotateInDownRight` |
| `rotateInUpLeft` |
| `rotateInUpRight` |
| `rotateOut` |
| `rotateOutDownLeft` |
| `rotateOutDownRight` |
| `rotateOutUpLeft` |
| `rotateOutUpRight` |
| `Specials` |
| `hinge` |
| `jackInTheBox` |
| `rollIn` |
| `rollOut` |
| `zoomIn` |
| `zoomInDown` |
| `zoomInLeft` |
| `zoomInRight` |
| `zoomInUp` |
| `zoomOut` |
| `zoomOutDown` |
| `zoomOutLeft` |
| `zoomOutRight` |
| `zoomOutUp` |
| `slideInDown` |
| `slideInLeft` |
| `slideInRight` |
| `slideInUp` |
| `slideOutDown` |
| `slideOutLeft` |
| `slideOutRight` |
| `slideOutUp` |

## note by the original author, Fareed Alnamrouti <digital.flowers@hotmail.com>:
From React 17.x.x [componentWillReceiveProps](https://medium.com/@baphemot/whats-new-in-react-16-3-d2c9b7b6193b#dd16) will be deprecated and a different strategy is introduced.
