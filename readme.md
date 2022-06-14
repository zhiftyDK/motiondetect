## motiondetect.js the webcam motion detector library
### Get Started
Include the library in your `.html` file
```JS
<script src="https://zhiftydk.github.io/motiondetect/motiondetect.js"></script>
```

### Start the bot
First of all you need to install the telegram app
<br>
<br>
<a href="https://telegram.org/"><img src="images/telegram.webp" style="width:10vw;"></a>

Then in the app search for `@TheMotionDetectorBot`
<br>
<br>
<img src="images/search.JPG" style="width:15vw;">

Now open the bot and click start
<br>
<br>
<img src="images/start.PNG" style="width:15vw;">

### Initialize motion detector
Example: Full setup with all possible varaibles
```JS
//The motion detector is using telegram to send messages!
const config = {
    chatId: "5598851680", //REQUIRED How to get telegram chatId https://www.alphr.com/find-chat-id-telegram/
    message: "Motion is detected!", //OPTIONAL Default message is "Motion is detected!"
    displayVideo: false, //OPTIONAL Boolean.. Default is false
    detectThreshold: 50, //OPTIONAL integer.. Default detectThreshold is 50
    botId: "5338504929:AAHZulboa7YpUPDjU3QgqPI9JUARlHuj5YI", //OPTIONAL This is the defualt telgram botId for TheMotionDetector bot
}
const md = new motionDetect(config); //Create new detection instance with the config
```

Example: Simple setup with fewest possible varaibles
```JS
//The motion detector is using telegram to send messages!
const config = {
    chatId: "5598851680", //REQUIRED How to get telegram chatId https://www.alphr.com/find-chat-id-telegram/
}
const md = new motionDetect(config); //Create new detection instance with the config
```

### Start motion detector
```JS
md.start(); //Start the detection from the webcam
```

### Stop motion detector
```JS
md.stop(); //Stop the detection from the webcam
```

### Bot response example
<img src="images/response.PNG" style="width:15vw;">
