Nach Neuinstallation:

folgenden Befehl in Powershell mit Adminrechten Starten
```PowerShell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/michaelcuerlis/windeb/refs/heads/master/Get.ps1"))) -RemoveApps -RemoveW11Outlook -RemoveGamingApps -DisableDVR -DisableTelemetry -DisableBing -DisableSuggestions -DisableDesktopSpotlight -DisableLockscreenTips -RevertContextMenu -ShowKnownFileExt -HideSearchTb -HideTaskview -HideChat -DisableWidgets -DisableCopilot -DisableRecall -ExplorerToThisPC
```

Bestehende Installationen:

folgenden Befehl in Powershell mit Adminrechten Starten
```PowerShell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/michaelcuerlis/windeb/refs/heads/master/Get.ps1"))) -RemoveW11Outlook -RemoveGamingApps -DisableDVR -DisableTelemetry -DisableBing -DisableSuggestions -DisableDesktopSpotlight -DisableLockscreenTips -RevertContextMenu -ShowKnownFileExt -HideSearchTb -HideTaskview -HideChat -DisableWidgets -DisableCopilot -DisableRecall -ExplorerToThisPC
```

### Parameters

Liste der Parameter genutzt werden können
Bsp.
```PowerShell
& ([scriptblock]::Create((irm "https://raw.githubusercontent.com/michaelcuerlis/windeb/refs/heads/master/Get.ps1"))) -RemoveW11Outlook
```

| Parameter | Description |
| :-------: | ----------- |
| -Silent                            |    Suppresses all interactive prompts, so the script will run without requiring any user input. |
| -Sysprep                           |    Run the script in Sysprep mode. All changes will be applied to the Windows default user profile and will only affect new user accounts. |
| -RunDefaults                       |    Run the script with the default settings. |
| -RunSavedSettings                  |    Run the script with the saved custom settings from last time. These settings are saved to and read from the `SavedSettings` file in the root folder of the script. |
| -RemoveApps                        |    Remove the default selection of bloatware apps. |
| -RemoveAppsCustom                  |    Remove all apps specified in the 'CustomAppsList' file. IMPORTANT: You can generate your custom list by running the script with the `-RunAppConfigurator` parameter. No apps will be removed if this file does not exist! |
| -RunAppConfigurator                |    Run the app configurator to generate a list of apps to remove, the list is saved to the 'CustomAppsList' file. Running the script with the `-RemoveAppsCustom` parameter will remove the selected apps. |
| -RemoveCommApps                    |    Remove the Mail, Calendar, and People apps. |
| -RemoveW11Outlook                  |    Remove the new Outlook for Windows app. |
| -RemoveDevApps                     |    Remove developer-related apps such as Remote Desktop, DevHome and Power Automate. |
| -RemoveGamingApps                  |    Remove the Xbox App and Xbox Gamebar. |
| -ForceRemoveEdge                   |    Forcefully remove Microsoft Edge, this option leaves Core, WebView and Update components installed for compatibility. NOT RECOMMENDED! |
| -DisableDVR                        |    Disable Xbox game/screen recording feature & stop gaming overlay popups. |
| -ClearStart                        |    Remove all pinned apps from start for the current user (Windows 11 update 22H2 or later only) |
| -ClearStartAllUsers                |    Remove all pinned apps from start for all existing and new users. (Windows 11 update 22H2 or later only) |
| -DisableTelemetry                  |    Disable telemetry, diagnostic data & targeted ads. |
| -DisableBing                       |    Disable & remove Bing web search, Bing AI & Cortana in Windows search. |
| -DisableSuggestions                |    Disable tips, tricks, suggestions and ads in start, settings, notifications and File Explorer. |
| -DisableDesktopSpotlight           |    Disable the 'Windows Spotlight' desktop background option. |
| <pre>-DisableLockscreenTips</pre>  |    Disable tips & tricks on the lockscreen. |
| -RevertContextMenu                 |    Restore the old Windows 10 style context menu. (Windows 11 only) |
| -ShowHiddenFolders                 |    Show hidden files, folders and drives. |
| -ShowKnownFileExt                  |    Show file extensions for known file types. |
| -HideDupliDrive                    |    Hide duplicate removable drive entries from the File Explorer navigation pane, so only the entry under 'This PC' remains. |
| -TaskbarAlignLeft                  |    Align taskbar icons to the left. (Windows 11 only) |
| -HideSearchTb                      |    Hide search icon from the taskbar. (Windows 11 only) |
| -ShowSearchIconTb                  |    Show search icon on the taskbar. (Windows 11 only) |
| -ShowSearchLabelTb                 |    Show search icon with label on the taskbar. (Windows 11 only) |
| -ShowSearchBoxTb                   |    Show search box on the taskbar. (Windows 11 only) |
| -HideTaskview                      |    Hide the taskview button from the taskbar. (Windows 11 only) |
| -HideChat                          |    Hide the chat (meet now) icon from the taskbar. |
| -DisableWidgets                    |    Disable the widget service & hide the widget (news and interests) icon from the taskbar. |
| -DisableCopilot                    |    Disable and remove Windows Copilot. (Windows 11 only) |
| -DisableRecall                     |    Disable Windows Recall snapshots. (Windows 11 only) |
| -HideHome                          |    Hide the home section from the File Explorer navigation pane and add a toggle in the File Explorer folder options. (Windows 11 only) |
| -HideGallery                       |    Hide the gallery section from the File Explorer navigation pane and add a toggle in the File Explorer folder options. (Windows 11 only) |
| -ExplorerToHome                    |    Changes the page that File Explorer opens to to `Home` |
| -ExplorerToThisPC                  |    Changes the page that File Explorer opens to to `This PC` |
| -ExplorerToDownloads               |    Changes the page that File Explorer opens to to `Downloads` |
| -ExplorerToOneDrive                |    Changes the page that File Explorer opens to to `OneDrive` |
| -HideOnedrive                      |    Hide the OneDrive folder from the File Explorer navigation pane. (Windows 10 only) |
| -Hide3dObjects                     |    Hide the 3D objects folder under 'This pc' in File Explorer. (Windows 10 only) |
| -HideMusic                         |    Hide the music folder under 'This pc' in File Explorer. (Windows 10 only) |
| -HideIncludeInLibrary              |    Hide the 'Include in library' option in the context menu. (Windows 10 only) |
| -HideGiveAccessTo                  |    Hide the 'Give access to' option in the context menu. (Windows 10 only) |
| -HideShare                         |    Hide the 'Share' option in the context menu. (Windows 10 only) |
