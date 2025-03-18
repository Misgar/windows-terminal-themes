<h3 align="center">
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
	Catppuccin for <a href="https://github.com/Microsoft/Terminal">Windows Terminal</a>
	<img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
    <a href="https://github.com/catppuccin/windows-terminal/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/windows-terminal?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/windows-terminal/issues"><img src="https://img.shields.io/github/issues/catppuccin/windows-terminal?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/windows-terminal/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/windows-terminal?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

<p align="center">
  <img src="assets/splash.png"/>
</p>

## Usage

1. Launch Windows Terminal
2. Open the **Settings** panel (<kbd>Ctrl + ,</kbd>)
3. Select **Open JSON file** at bottom left corner (<kbd>Ctrl + Shift + ,</kbd>)
4. Choose your _flavour_ (frappe, latte, macchiato, mocha)
5. Copy the contents of _flavour_.json (example: frappe.json) into the opened JSON file under **"schemes"**:

```json
{
    ..default layout
    "schemes":
    [
        ..catppuccin flavour
        ..other schemes
    ],
}
```

6. Copy the contents of _flavourTheme_.json (example: frappeTheme.json) into the opened JSON file under **"themes"**:

```json
{
    ..default layout
    "themes":
    [
        ..catppuccin flavour
        ..other themes
    ],
}
```

7. Save and exit
8. In the **Settings** panel under Profiles, select the profile you want to apply the theme to. **Defaults** will apply theme to all profiles.
9. Select **Appearance**
10. Choose your _catppuccin flavor_ in the **Color scheme** drop down menu 
11. Click on **Save**, enjoy! ✨

## 💝 Thanks to

- [Pocco81](https://github.com/Pocco81)
- [LudoPinelli](https://github.com/LudoPinelli)
- [AdalZanabria](https://github.com/AdalZanabria)
- [Aryan Prince](https://github.com/aryanprince)

<h1> oh my posh </h1>
Oh My Posh
Oh My Posh is a prompt theme engine that lets you beautify the prompt string. This engine requires your Terminal to use a Nerd Font so make sure that you followed along the previous steps.

Setup
Install “App Installer” from Microsoft Store to get the winget Windows Package Manager CLI.

⚠ Requires Windows 10 1809 (build 17763) or later
Check out Oh My Posh’s documentation for alternative installation options.
Restart your Windows Terminal and run winget to check if the package manager is correctly installed.

In your Windows Terminal, run

winget install JanDeDobbeleer.OhMyPosh
Restart your Windows Terminal. Next, try running oh-my-posh in Powershell to see if it’s correctly installed.

Default theme

Run the following command to open your Powershell profile.

notepad $PROFILE
If notepad shows a prompt saying that “Microsoft.Powershell_profile.ps1” is not found and asks if you would like to create the file, press “Yes” to create the file.

Inside the file, paste in the following code and save the file. This will load Oh My Posh on start-up with the default theme.

oh-my-posh --init --shell pwsh --config ~/AppData/Local/Programs/oh-my-posh/themes/jandedobbeleer.omp.json | Invoke-Expression
Restart your Terminal. Your Powershell should now load Oh My Posh automatically

Default theme on startup
