# Estimating Turbidity with Underwater Photos (Machine Vision Application)
Repo for my senior honors research project using machine vision to estimate turbidity of underwater images.

<!---
<a href="[link](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/wiki)"><img src="./WebApp/V3/full.webp" /></a>
-->

- Currently using OpenAI CLIP format for classification with Yolov8

## Using The WebApp
### Online/Live
- NOTE: The live WebApp requires an internet connection to download the model/webpage each time the page is (re)loaded (although, all files *should* be cached for a while after the first time you use it). HOWEVER, data analysis is run on YOUR OWN device, not on a server. This means that your data/pictures are not being uploaded to and processed on a server, they stay on your computer. It also means that the faster your computer (or phone/tablet/or other device capable of surfing the web) is, the faster it will run.
- It is also worth noting that if you plan on using it multiple times, consider following the instructions for using the WebApp locally/standalone, as you would only need to download the files once (and they are decently large files).

  [CLICK HERE](https://ianrudy.com/Turbidity/) to launch the WebApp.  
  Alternatively, you can open the latest page under "Deployments", which should redirect you to the live WebApp.

### Local/Standalone
- NOTE: Instructions provided work for desktop/laptop computers only (Windows, Mac, Linux). Phones and other devices do not have instructions provided to run the code locally. The WebApp UI was designed to be mobile friendly, and can be used on mobile devices using the Live version. (Or if you know how to emulate a server on your phone)

The WebApp code was made to be a simple static webpage, as such, running (serving) it locally is rather easy. This is especially beneficial if you plan to use it multiple times, as you can avoid downloading the large files more times than is necessary (if caching isn't working), and also allows it to be used without an internet connection (the live/online WebApp only needs an internet connection to load the page at the beginning, if the internet disconnects in the middle of processing images, it will continue to work).


The basic instructions for running the WebApp standalone are as follows.
1. Download the WebApp code from [HERE](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/download/v1.0.0/Website.Standalone.zip).
2. Unzip the .zip folder and put it where you want (make note of where you put the folder).
3. Download the latest version of Servez for your operating system from <a href="[link](https://github.com/greggman/servez/releases/latest)">HERE</a>.
   - exe for windows, AppImage for Linux, universal.dmg for Mac
5. Install Servez
6. Launch Servez
7. In Servez, set the "Folder to Serve", as the unzipped folder from step 2.
8. Recommended to set Servez settings as follows:
   - Port: 8080
   - ☑ Show Folder Listings  -  (probably not necessary)
   - ☑ Automatically show index.html
   - ☐ Local Machine Only
   - ☑ Set CORS headers
   - ☑ Support Unity  -  (probably not necessary)
   - ☐ SharedArrayBuffer headers
   - ☐ Use HTTPS
8. Finally, click "Launch Browser"
   - if browser doesn't immediately open, open your web browser and try going to http://127.0.0.1:8080 or http://localhost:8080

## About The Code
- You can learn more about the WebApp's code on this repo's wiki, or by clicking [HERE](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/wiki/Web-App)
- You can view documentation and learn more about the Research Code (Data Preparation/Model Training, etc...) on this repo's wiki, or by clicking [HERE](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/wiki/Research-Code)
