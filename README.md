# gn-notification

GreenNav polymer element for showing route informations and notifications. The gn-notification-container handles route informations and additional notifications with data-bindings. The gn-route-notification shows hints, warnings and errors (very important informations) on the route.

## Setup Instructions

Clone the project (or download and extract zip).

```
git clone https://github.com/tom3012/gn-notification.git
```

### Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can install that (globally) via:

```
npm install -g bower
```

Move in the project folder and download the element's dependencies:

```
bower install
```

### Documentation and Demo

Use [Polyserve](https://github.com/PolymerLabs/polyserve) to play with gn-notification, read the documentation and watch the demo. You can install it via:

```
npm install -g polyserve
```

And you can run it via:

```
polyserve
```

Once running, you can preview your element at `http://localhost:8080/components/gn-notification/`, where `gn-notification` is the name of the directory containing it.

### Short examples

The main component:

```html
<gn-notification-container turn-code="3"
                           distance="25"></gn-notification-container>
<google-map latitude="37.77493" longitude="-122.41942"></google-map>
```

Example of different notifications:

```html
<paper-button raised onclick="warning.open()">warning notification</paper-button>
<paper-button raised onclick="error.open()">error notification</paper-button>

<gn-route-notification  id="warning" warning title="Warning">
  Oh, oh... there is a warning message.
</gn-route-notification>
<gn-route-notification  id="error" error title="Error">
  An error has occurred
</gn-route-notification>
```

With text to speech:

```html
<gn-notification-tts text="Hello World!" locale="en"></gn-notification-tts>
```

## TODO

### Done

- [x] ~~Show directions (Webapp)~~
- [x] ~~Show useful information with additional notifications (Webapp)~~
- [x] ~~Add voice output~~

### Maybe in Future

- [ ] Implement Google Authentificaiton (?)


