# Unity (game engine) Setup Guide

## Unity installation

* Go to Unity download web page (<https://unity3d.com/get-unity/download>)

* Click on Hub download button ("**Download Unity Hub**")

* Ubuntu/Linux: make downloaded AppImage executable: `chmod +x UnityHub.AppImage`

* Open Unity Hub.

* Click on "Installs" and then "ADD".

* Click on "Unity 2020.3 (LTS)" and then "NEXT".

* Click on "DONE". No need to install modules for now, can be added later.

* Click on top-right icon in Unity Hub and create a Unity account (ID), if not already.

* Sign in within Unity Hub with your account.

* Go into "Preferences" (top-right) and then into "Licence Management".

* Add a free "Personal Licence".

* Go back to the main page of Unity Hub.

* From here you can now start a new project with the Unity Editor!

## Get to know Unity

* Check out Manual: <https://docs.unity3d.com/Manual/index.html>

* Check out Tutorials: <https://learn.unity.com/>

  * Recommend this for our use-case: <https://learn.unity.com/tutorial/creating-a-tic-tac-toe-game-using-only-ui-components>

## (Optional) Linux: Setup script editing with Visual Studio Code

* Writing and editing scripts in Unity requires a third-party editor. By default this is set to "Open by file extension". To use VS Code properly with all functionality some extra stuff has to be done.

* Install VS Code, if not already. One way of doing it:

  ```bash
  sudo snap install code --classic
  ```

  * Source: <https://snapcraft.io/code>

* Install .NET. One way (easiest) of doing it:

  ```bash
  sudo snap install dotnet-sdk --channel=5.0/stable --classic
  ```

  * Source: <https://docs.microsoft.com/en-us/dotnet/core/install/linux>

* Install Mono:

  * <https://www.mono-project.com/download/stable/#download-lin>

* In Visual Studio Code:

  * Go to Extensions and install the official **C#** Extention.
  * Click on the gear wheel (Manage) button of that extension.
  * Click on "Extension Settings".
  * Go to "Omnisharp: **Use Global Mono**".
  * Change setting from "auto" to "always".

* In Untiy Editor:

  * Go to "Edit" and than "Preferences...".
  * Go to "External Tools".
  * Change "External Script Editor" to "Visual Studio Code".
  * Close "Preferences" window.

* You should now be good to go!
