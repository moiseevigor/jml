JML - Javascript markup language
===

**JML** is as [QT](http://qt-project.org/) meets the HTML, CSS and DOM events, kind of [AbsurdJS](http://krasimir.github.io/absurd/) at the `n`-th power of the absurd.


```javascript
Body = function() {
  html: 'body'
}
```

Nice ideas at [Asana](https://asana.com/luna)

```
defineType('World', {
  messages: List/*<ChatMessage>*/
});

defineType('ChatMessage', {
  user: User,
  text: String
});

defineType('Session', {
  user: User,
  new_comment: String
});

function renderMessage(message) {
  return DIV([
    IMG({src: message.user().small_pic_url()}),
    DIV({'class': 'bubble'}, [
      B([message.user().name(), ': ']),
      DIV([message.text()])
    })
  ]);
}
```
