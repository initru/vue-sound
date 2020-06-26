# Vue Hifi: An accessible audio player built with Vue.js

Add a beautiful & accessible cross-browser HTML5 audio player to your Vue app!

## Installation and Usage

```
npm install vue-hifi
```

Import or require Vue and Vue Hifi in your code:

```
import Vue from 'vue'
import VueHifi from 'VueHifi'
```

### Example

``` 
<vue-hifi
  livestream
  show-download
  title="The Show"
  title-link="http://www.google.com"
  details="Lorem Ipsum Dolor Sit Amet"
  details-link="http://www.bing.com"
  file="http://www.hochmuth.com/mp3/Haydn_Cello_Concerto_D-1.mp3"
/>
```

### Configuration

All props except for the audio file are optional.

Prop | Type | Default | Description
--- | --- | --- | ---
livestream | boolean | false | if true, displays slimmer version of audio player meant for a livestream
show-download | boolean | false | if true, display a download button
title | string | null | the title of the track
title-link | string | null | url for the title link
details | string | null | details for the track
details-link | string | null | url for the details
file | string | null | url for the audio file (mp3 is highly recommended)

#### Styles

Override these CSS variables to customize the look and feel:

``` 
:root {
    --player-background: #ff9efc;
    --player-font-size: 1rem;
    --player-font-size-small: .7rem;
    --player-font-weight: 300;
    --player-font-weight-bold: 500;
    --player-text-color: #451a43;
    --player-icon-color: var(--player-text-color);
    --player-link-color: var(--player-text-color);
    --player-progress-color: #f25ced;
    --player-buffered-color: #cc4ec8;
    --player-seeker-color: #451a43;
    --player-input-range-color: var(--player-text-color);
}
``` 

### Browser Support

The audio element is supported by all modern browsers. We recommend using MP3 audio files since that format is also supported by all modern browsers.

### Accessibility

Vue Hifi is 100% keyboard accessible. The enter/space keys toggle play/pause, the up/down arrows control the volume, and the right/left arrows skip ahead/back. Other audio player controls such as mute and download can be tabbed to and controlled by the keyboard.

## Local Development Environment

```
npm install
```

Compiles and hot-reloads for development
```
npm run serve
```

Compiles and minifies for production
```
npm run build
```

Launches Storybook
```
npm run storybook
```

Lints and fixes files
```
npm run lint
```

## Questions / Contributing

Report issues or open pull requests on github: https://github.com/kimlarocca/vue-hifi/
