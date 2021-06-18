## ❓What is The Use of This Code


- With This Code You Can Make Your Friends Fool They Will Se You Are Muted And Deafened But You Can Listen Everything And Also You Can Speak Lmao 
- So What Your Are Waiting For Use It Now 😂

## 🔗Join Your Discord Server


- [Join Developers Adda](https://dsc.gg/developersarena)

## 🖥 MAIN CODE

##How To Use This Code

```
Simply Copy This Code And Paste It Into Your Discord Console !! 
To Open Your Dicord Console `Press CTRL Shif + I` To Open Your Console
```

```css

var text = new TextDecoder("utf-8");

WebSocket.prototype.original = WebSocket.prototype.send;
WebSocket.prototype.send = function(data) {
    if (Object.prototype.toString.call(data) === "[object ArrayBuffer]") {
        if (text.decode(data).includes("self_deaf")) {
            console.log("found mute/deafen");
            data = data.replace('"self_mute":false', 'https://dsc.gg/developersarena');
            console.log("By Vishal CodeZ");
        }
    }
    WebSocket.prototype.original.apply(this, [data]);
}
```

Note This Hack Is Only Works On Discord Application
