# Install notes

## Compiler installation :


### Using prepared binaries
- Download and extract [NWNScriptCompiler package](https://github.com/CromFr/STNeverwinterScript/releases/download/1.0/NWNScriptCompiler.zip) in:
	- **Windows**: C:\Program Files (x86)\
	- **Linux**: /opt/


### Using custom binaries

- Download the AdvancedScriptCompiler (http://nwvault.ign.com/View.php?view=nwn2plugins.Detail&id=99) and extract the standalone compiler at
	- **Windows**: C:\Program Files (x86)\NWNScriptCompiler\
	- **Linux**: /opt/NWNScriptCompiler/
	
- If installed in another directory that the one specified, you will need to update the path to NWNScriptCompiler.exe in nwscript.sublime_build (dont forget to use double backslashes)

- Extract the NWN2 script data files (maybe C:\Program Files (x86)\Atari\Neverwinter Nights 2\Data\Scripts*.zip) in
	- **Windows**: C:\Program Files (x86)\NWNScriptCompiler\Scripts\
	- **Linux**: /opt/NWNScriptCompiler/Scripts

- You can delete ncs files from this directory since only nss are required to build

## Extra steps for Linux
You need wine in order to use the NWNScriptCompiler.exe
```bash
apt-get install wine #Ubuntu/Debian users
yup install wine #Fedora/Redhat users
pacman -S wine #Arch-Linux awesome users
```

## Sublime package installation :

### With PackageControl :
- Add repository https://github.com/CromFr/STNeverwinterScript.git
- Install package STNeverwinterScript

### Manual install :
- Clone/extract https://github.com/CromFr/STNeverwinterScript into the sublime package directory (%appdata%\Roaming\Sublime Text 3\Packages on windows)
