[[_TOC_]]

## Overview
This is the client-side application for Fast Trend (developed using Flutter)

## Development


### Running the app locally

- Open the workspace in VS Code
  - Make sure to open the workspace, and not just the folder
- Run `flutter pub get`
  - This will install all the flutter/dart dependencies for the project
- If running the app on an Android device, run `adb reverse tcp:3000 tcp:3000`
  - This will allow the app to communicate to the server on port 3000
  - NOTE: A similar step might be needed to run the app on iPhone as well
- Run `rps gen-watch`
  - This will generate the routes dynamically as you change the provided route structure
  - Let this run in the background as you develop the application. If you make any changes to the route, you will see that it re-generates new code for the routes.
  - If you stop this command, and then make a change to the routes, it will not show up in the app until this command is run again
  - Alternatively, to run this command once without letting it wait in the background, you can run `rps gen`, but it takes a while each time you run it.
- In VS Code, select the device you want to run the app on
  - You can use the Flutter Target Device shown on the right side of the task bar at the bottom of the screen
  - Alternatively, you can use `"Ctrl+Shift+P"`, and type `"Flutter: Select Device"`
- You can now run the app from VS Code:
  - Open `"Run And Debug"` from the Navigation Bar on the left side of the screen
  - Select `"Flutter (workspace)"` and hit the Play button
  - The app will start building, and once it's done, it will open up on your selected device
    - It might take a little longer when you run the app for the first time

**NOTE: For the app to function properly, you will also need to run the server in the background. You can find the instructions for that under the fashtrend_server's README**

