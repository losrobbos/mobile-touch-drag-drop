# Mobile touch drag n drop

Demo: https://mobile-touch-dragdrop-demo.vercel.app

Find here a minimal sample to realize a dragNdrop of an item in mobile browsers using touch events.

The minimal setup you need for an item to drag and drop:

- touchstart Event
- touchend Event
- document.elementFromPoint Function

You add the two events (touchstart and touchend) to the item you want to drag.

How it works:

The only real coding part happens in the "touchend" event.

Here you need to grab the item you are currently HOVERING over and check if it 
is a valid item to drop on.

Here you can use the document.elementFromPoint method to grab the underlying DOM element.
And can e.g. analyze by the CSS class that element has, if we are allowed to drop there.

Find all code in the index.html file in the script tag.

## Change style when moving over a drop target

If you, additionally, want to create a hover effect when moving over a valid "drop target" 
where you can drop the item on (often called the "dropzone") you additionally need:

- touchmove Event

"You're out of touch... I'm out of time!"

Cheeeeeers!