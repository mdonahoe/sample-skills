# Getting Started with the Skills SDK

Skills are python scripts that run onboard the drone and provide basic UI elements inside the app.

![animation](images/roof-inspection.gif)


## Skillset

We've put together a skillset of sample skills that you can use to learn how the Skills SDK works.

### Try these skills in the simulator and control with your mobile app

1. [Download](https://github.com/mdonahoe/sample-skills/archive/master.zip) this repo and unzip it.
1. [Login](https://console.skydio.com) to the Developer Console using the same email you use in the mobile app.
1. Create a new [skillset](https://console.skydio.com/skillsets/) with a unique name for your testing.
1. Upload the `skillset` folder from the zip into your newly created skillset. This creates an automatic file sync between our server and your browser tab if using Google Chrome.
1. Open the [simulators page](https://console.skydio.com/simulators) in a new tab.
1. Open the mobile app  and [select the matching simulator](https://console.skydio.com/docs/skills/getting_started.html#running-the-skydio-mobile-app) via the INFO tab.
1. Tap `FLY NOW` in the app, and you should start to see streaming video from the simulator in your app and the browser.
1. Press and hold the launch button to get your drone flying.
1. Select the `PropertyTour` sample skill from the menu in the app to activate it. You should see a `Go` button on screen. Pressing it will initiate the automated tour.
1. Edit the code for the `property_tour.py` using your favorite code editor.
1. Save the file and your change will be automatically uploaded to the cloud via your open skillset web page (if you are not using Chrome you will have to re-upload).
1. Press the `Sync` button in the CLOUD menu of the app to redeploy your code to the simulator. You will need to re-select your skill, as the system restarts and selects the `Motion Track` skill by default.

Visit the [Getting Started](https://console.skydio.com/docs/skills/getting_started.html) section of the SDK docs for more information.

### Included Skills

- [Polygon Path](skillset/polygon_path.py): Fly a path in the shape of a user-defined polygon.
- [Property Tour](skillset/property_tour.py): Perform a series of cinematic motions to record a real estate video.
- [Roof Inspection](skillset/roof_inspection.py): Fly a configurable scanning pattern over the roof of a house.
- [Security Bot](skillset/security_bot.py): Follow anyone that gets within range of a home point, then return.
- [Party Mode](skillset/party_mode.py): Automatically follow subjects for 15 seconds at a time within a defined area.
