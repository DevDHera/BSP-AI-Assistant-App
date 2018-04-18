# BSP - AI Assistant

>A visually beatiful AI client for BSP users. Use the Ionic as the front end. 



### System Overview

An AI client that will help you in your day to day banking needs. Talk to her, chat her and more importantly do some banking with BSP.

### Technologies Used

* Ionic 
* API.AI

### Why go Ionic rather that Native.

Ionic was used by me because of the hardware limitations I was facing. I love to go native. But if you have limited resources you have to look for alternatives.

Ionic provide cloud infrastructure to build hybrid apps. Single codebase. Everything is awesome.

If you have a machine that even can't run Android Studio (like me...) simply package the app using Ionic pro.

You can use Ionic View as feedback machenism and Ionic DevApp as a hot reloading mobile app.
## Sample Coding
Sending voice to the AI client was a place I got stuck. Here how I proceed and got rid of the problem.

#### How to send voice

```javascript
sendVoice(){
    window["ApiAIPlugin"].requestVoice({},
      (response) => {
        this.tts.speak({
          text: response.result.fulfillment.speech,
          locale: "en-LK",
          rate: 1
        })
      }, (error) => {
        alert(error)
      }
    )
  }

```

### Tasks To Achive

* [x] Make UI Beautiful
* [x] Send Voice
* [ ] AI Traning
