# Turbidivision: Estimating Turbidity from Underwater Photos with Machine Vision
Turbidivision is available as both a web app that runs locally on your computer, and as a standalone binary for certain platforms.  




[![Windows Download](https://img.shields.io/badge/-%20Windows%20Executable%20-%20?logo=Windows&labelColor=black&color=black&link=https%3A%2F%2Fgithub.com%2FYellowTeamRobot%2FAI_Turbidity_Honors2023-4%2Freleases%2Fdownload%2Fv1.0.2%2FTurbidivision.1.0.2.exe)](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/download/v1.0.2/Turbidivision.1.0.2.exe)
[![Linux Download](https://img.shields.io/badge/-%20Linux%20AppImage%20-%20?logo=Linux&logoColor=white&labelColor=black&color=black&link=https%3A%2F%2Fgithub.com%2FYellowTeamRobot%2FAI_Turbidity_Honors2023-4%2Freleases%2Fdownload%2Fv1.0.2%2FTurbidivision-1.0.2.AppImage)](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/download/v1.0.2/Turbidivision-1.0.2.AppImage)
[![Android Download](https://img.shields.io/badge/-%20Android%20APK*%20-%20?logo=Android&logoColor=white&labelColor=black&color=black&link=https%3A%2F%2Fgithub.com%2FYellowTeamRobot%2FAI_Turbidity_Honors2023-4%2Freleases%2Fdownload%2Fv1.0.2%2FTurbidivision1.0.2.apk)](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/download/v1.0.2/Turbidivision1.0.2.apk)
 &nbsp; <sup>*also available on [Google Play](https://play.google.com/store/apps/details?id=com.ianrudy.turbidity)</sup>

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10982478.svg)](https://doi.org/10.5281/zenodo.10982478) <sup>| The dataset used in this project can be downloaded from [here](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/tag/v1.0.0)</sup>


<!---
<a href="[link](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/wiki)"><img src="./WebApp/V3/full.webp" /></a>
-->

[![Turbidivision](https://img.shields.io/badge/-Turbidivision%20Website-%20?style=social&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz48c3ZnIGlkPSJMYXllcl8xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzNi44OSA1OC41MyI%2BPGRlZnM%2BPHN0eWxlPi5jbHMtMXtmaWxsOiMyZGFkZmY7fS5jbHMtMSwuY2xzLTJ7c3Ryb2tlLXdpZHRoOjBweDt9LmNscy0ye2ZpbGw6I2ZmZjt9PC9zdHlsZT48L2RlZnM%2BPHBhdGggY2xhc3M9ImNscy0xIiBkPSJNMzMuNjksMzIuNmMtLjgzLTEuOTktMy4xMi03LTcuNDMtMTMuNjUtMy44Mi01Ljg5LTcuMzgtMTYuMTUtNy44NS0xNy41M2gwcy4wMi0uMDUsMCwwYy0uMDItLjA1LDAsMCwwLDBoMGMtLjQ3LDEuMzgtNC4wMiwxMS42NC03Ljg1LDE3LjUzLTUuNjIsOC42Ni03Ljc5LDE0LjU2LTcuOCwxNC41OC0uODUsMi4wMy0xLjMyLDQuMjUtMS4zMiw2LjU5LDAsOS4zOSw3LjYxLDE3LDE3LDE3czE3LTcuNjEsMTctMTdjMC0yLjctLjYzLTUuMjUtMS43NS03LjUyWiIvPjxwYXRoIGNsYXNzPSJjbHMtMiIgZD0iTTM1LDMxLjk2Yy0uODEtMS45NC0zLjE0LTcuMDctNy41MS0xMy43OS0zLjY1LTUuNjMtNy4xMS0xNS41NS03LjYzLTE3LjA1LS4wNi0uMjItLjE3LS40Mi0uMzEtLjU4LS4yOS0uMzQtLjcxLS41My0xLjE1LS41My0uMTYsMC0uMzIuMDMtLjQ3LjA4LS41My4xOC0uODkuNjEtLjk5LDEuMTItLjYsMS43NC00LjAxLDExLjQ0LTcuNiwxNi45Ny01LjQ3LDguNDMtNy43MSwxNC4yNS03LjkxLDE0LjgtLjk1LDIuMjYtMS40Miw0LjY1LTEuNDIsNy4xMiwwLDEwLjE3LDguMjcsMTguNDQsMTguNDQsMTguNDRzMTguNDQtOC4yNywxOC40NC0xOC40NGMwLTIuODQtLjYzLTUuNTgtMS44OC04LjEyWk0zNC4zNCwzNC4yM2MtMi45Mi42My05LjY4LDEuNjgtMTUuNjItLjM1LTYuMDktMi4wOC0xMi42Ni0xLjE2LTE1Ljg1LS40OS4xOS0uNTEsMS4wNS0yLjY2LDIuNzktNS45OSwzLjM1LS40OCw4LjIyLS43MSwxMi43My44MywyLjgxLjk2LDUuNzUsMS4yOCw4LjQzLDEuMjgsMS45NCwwLDMuNzMtLjE3LDUuMjQtLjM4Ljc1LDEuNTMsMS4yNywyLjcsMS41OSwzLjQ1LjI2LjUzLjUsMS4wOC43LDEuNjRaTTE4LjQyLDEuNTFjLjQ3LDEuMzcsNC4wMSwxMS42LDcuODIsMTcuNDcuMzQuNTMuNjcsMS4wNC45OSwxLjU1LTIuNjYuMDUtNS42Mi0uMjEtOC40MS0xLjE2LTIuNTctLjg4LTUuMjItMS4yMy03LjY2LTEuMjksMy41OS01Ljk2LDYuODItMTUuMjYsNy4yNi0xNi41N1pNOS44OSwyMC4wOWMyLjYxLS4wNCw1LjUxLjIzLDguMjgsMS4xNywyLjgzLjk3LDUuNzksMS4yOSw4LjQ5LDEuMjkuNjEsMCwxLjItLjAyLDEuNzgtLjA1LDEuMTIsMS44NywyLjA0LDMuNTUsMi44LDUuMDEtMy4zNy40Mi04LjA1LjU2LTEyLjI5LS44OS00LjMxLTEuNDctOC44NS0xLjQ1LTEyLjI4LTEuMDcuOS0xLjYzLDEuOTctMy40NiwzLjIzLTUuNDZaTTIuMywzNC45NmMyLjU1LS42MSw5LjYyLTEuOTIsMTUuOTcuMjUsMi43OC45NSw1LjcxLDEuMjcsOC4zNywxLjI3LDMuNDUsMCw2LjQ1LS41Myw4LjEzLS45LjQsMS40NC42MiwyLjk1LjYyLDQuNTEsMCwuNC0uMDMuNzktLjA2LDEuMTktMi4wNy41MS05Ljg5LDIuMTgtMTYuNjUtLjEzLTcuMTEtMi40My0xNC45NC0uNzMtMTcuMTMtLjE3LS4wMi0uMjktLjA0LS41OC0uMDQtLjg4LDAtMS43OS4yOC0zLjUxLjgtNS4xM1pNMzUuMiw0Mi40M2MtLjMzLDIuNDEtMS4xNyw0LjY1LTIuNCw2LjYyLTMuNDEuNTgtOS4wOSwxLjA4LTE0LjE4LS42Ni01LjcyLTEuOTUtMTEuOTMtMS4yMS0xNS4yNC0uNTctLjkxLTEuNzYtMS41MS0zLjY5LTEuNzUtNS43NCwxLjcxLS40Niw5LjYzLTIuMzIsMTYuNjkuMSwyLjc2Ljk0LDUuNjYsMS4yNiw4LjMxLDEuMjUsMy43OCwwLDcuMDMtLjY0LDguNTgtMVpNMTAuMjQsNTQuOWMyLjU5LS4wMSw1LjQ0LjI4LDguMTcsMS4yMS44Ni4yOSwxLjczLjUxLDIuNjEuNjktLjg0LjEzLTEuNy4yMi0yLjU4LjIyLTIuOTgsMC01Ljc3LS43Ny04LjItMi4xMlpNMjIuNCw1Ni41NGMtMS4yOC0uMTktMi41Ny0uNDctMy44My0uOS0zLjA4LTEuMDUtNi4zLTEuMzEtOS4xNC0xLjIzLTIuMzItMS40Ni00LjI2LTMuNDctNS42NC01Ljg1LDMuMjgtLjYyLDkuMTgtMS4yNiwxNC41Ny41OSwyLjczLjkzLDUuNjIsMS4yNCw4LjI1LDEuMjQsMi4wOSwwLDQuMDEtLjIsNS41OC0uNDMtMi4zMywzLjI0LTUuNzgsNS42Mi05Ljc5LDYuNThaIi8%2BPC9zdmc%2B&labelColor=grey&color=grey&link=https%3A%2F%2Fturbidi.vision)](https://turbidi.vision)







## Using The WebApp
### Online/Live
- NOTE: The live WebApp requires an internet connection to download the model/webpage each time the page is (re)loaded (although, all files *should* be cached for a while after the first time you use it). HOWEVER, data analysis is run on YOUR OWN device, not on a server. This means that your data/pictures are not being uploaded to and processed on a server, they stay on your computer. It also means that the faster your computer (or phone/tablet/or other device capable of surfing the web) is, the faster it will run.
- It is also worth noting that if you plan on using it multiple times, consider following the instructions for using the WebApp locally/standalone, or downloading one of the binary releases, as you would only need to download the files once (and they are decently large files).

  [CLICK HERE](https://turbidi.vision/app) to launch the WebApp.  
  Alternatively, you can open the latest page under "Deployments", which should redirect you to the live WebApp.

### Local/Standalone (Web)
- NOTE: The standalone executables (non-web) can be found as their own separate release, and downloaded from the release [here](https://github.com/YellowTeamRobot/AI_Turbidity_Honors2023-4/releases/tag/v1.0.2), or from the buttons at the top of the readme. This section provides instructions for serving the web page locally for use in a browser.
- NOTE: Instructions provided work for desktop/laptop computers only (Windows, Mac, Linux). Phones and other devices do not have instructions provided to run the code locally. The WebApp UI was designed to be mobile friendly, and can be used on mobile devices using the Live version. (Or if you know how to emulate a server on your phone)
If you have an Android phone with Android 12 or higher, you can download the standalone app. For iPhones and Android 11 or lower, the web version is the only version available.

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

-----
Repo for my senior honors research project using machine vision to estimate turbidity of underwater images.
- Currently using OpenAI CLIP format for classification with Yolov8
