---
title: "TextTrackCue: exit event"
short-title: exit
slug: Web/API/TextTrackCue/exit_event
page-type: web-api-event
browser-compat: api.TextTrackCue.exit_event
---

{{APIRef("WebVTT")}}

The **`exit`** event fires when a cue stops being active.

## Syntax

Use the event name in methods like {{domxref("EventTarget.addEventListener", "addEventListener()")}}, or set an event handler property.

```js-nolint
addEventListener("exit", (event) => { })

onexit = (event) => { }
```

## Event type

A generic {{DOMxRef("Event")}} with no added properties.

## Example

In the following example, `cue` prints to the console when it stops being displayed as the active cue.

```js
cue.addEventListener("enter", (event) => {
  console.log("Cue 1 has left the building.");
});
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}
