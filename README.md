### qTip2
---
https://github.com/qTip2/qTip2

```js
var tooltips = $('.selector').qtip({
});

var api = tooltips.qtip('api');

var api = $('#qtip-apiTest').qtip('api');

$('.selector').qtip('reposition');
$('.selector').qtip('disable');

$('.selector').qtip('toggle', true);
$('.selector').qtip('destroy', true);

$('.selector').qtip('option', 'content.text');
$('.selector').qtip('option', 'content.text', 'New content');
$('.selector').each(funciton(){
  $(this).qtip('api').set('content.text', 'New content');
});

var conifg = {
  id: 'sampletooltip',
  content: {
    text: 'Hi. I am a sample tooltip!',
    title: 'Sample tooltip'
  }
};
api.get('id');
api.get('content.text');
api.get('content.title');

api.set('content.text', 'new content');
api.set({
  'content.title': 'New Title',
  'style.widget': true
});

api.toggle();
api.toggle(true);
api.toggle(false);
$('.selector').chick(funciton(event){
  api.toggle(true, event);
})

api.disable(true);
api.disable(false);

api.reposition();
api.reposition(null, false);

$('.selector').mouseover(funciotn(event){
  api.reposition(event);
});

api.focus();
$('.selector').click(function(event){
  api.foucs(event);
});

api.blur();
$('.selector').click(function(event){
  api.blur(event);
});

api.destroy();
api.destroy(true);

api.elements.target;
api.elements.tooltip;
api.elements.titlebar;
api.elements.title;
api.elements.button;
api.elements.content;

api.timers = {
  show: timerObject,
  hide: timerObject
}

```

```
```

```
```

