jquery.timer
============

This is a jQuery timer plugin.

**Examples:**

```JavaScript
// the timer is fired immediately and then is fired every 1 second
$.timer(0, function () {
    this.setDelay(1000);
    console.log('fired!');
}).start();
```

```JavaScript
// the timer is fired 5 times
$.timer(1000, function () {
    console.log(this.getCount());
}).start(5);
```

```JavaScript
// the timer is fired only one time
$.timer(1000, function() {
    console.log('just one time');
}).once();
```

**Important methods:**

1. start()    : starts the timer
2. stop()     : stops the timer
3. play()     : resumes the timer
4. pause()    : pauses the timer
5. toggle()   : resumes or pauses the timer
6. once()     : starts and fires only one time
7. setDelay() : sets the delay
