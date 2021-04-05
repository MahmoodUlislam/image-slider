# React image slider

![Slider Preview](https://images.ctfassets.net/zlsyc9paq6sa/4ztfe5YDb4VweOSiTbr0c/14dda169e9335f8c83f7a638f834ef26/1617358599_x.gif)

### Demo: [https://image-slider-madza.vercel.app](https://image-slider-madza.vercel.app)

---

## Installation

```javascript
 npm install @madzadev/image-slider
```

## Usage

```javascript
import Slider from "@madzadev/image-slider";
import "@madzadev/image-slider/dist/index.css";
```

```javascript
const images = [
  { url: "https://picsum.photos/seed/a/1600/900" },
  { url: "https://picsum.photos/seed/b/1920/1080" },
  { url: "https://picsum.photos/seed/c/1366/768" },
];
```

```javascript
<Slider imageList={images} width={1000} height={300} />
```

`imageList` is the mandatory prop and requires to pass in
an array consisting of objects with `url` keys.

`width` and `height` are mandatory props that
set the dimension of the images shown.

## Behavior

The default values of available options props are displayed.

```javascript
<Slider
  loop={true}
  autoPlay={true}
  autoPlayInterval={3000} // in milliseconds
/>
```

## Controls

The default values of available props are displayed.

You can further customize the player by editing the colors variable below.

```javascript
<Slider showArrowControls={true} showDotControls={true} />
```

## Styling

The default values of available props are displayed.

```javascript
<Slider bgColor="none" />
```

If set, background color is displayed to fill the background if images are smaller than the slider wrapper.

## Final notes

The project is under MIT licence, so be free to check it out and give
contributions.
