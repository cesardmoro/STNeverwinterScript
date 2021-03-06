# Install notes

## Compiler installation :


### Option 1: Using prepared binaries
- Download and extract the latest [Packed NWNScriptCompiler](https://github.com/CromFr/STNeverwinterScript/releases) in:
	- **Windows**: C:\Program Files (x86)\
	- **Linux**: /opt/


### Option 2: Using custom binaries

- Download the AdvancedScriptCompiler (http://neverwintervault.org/project/nwn2/other/tool/advanced-script-compiler-nwn2) and extract the standalone compiler at
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
yum install wine #Fedora/Redhat users
pacman -S wine #Arch-Linux awesome users
```

## Sublime package installation :

### With PackageControl :
- Install package STNeverwinterScript
- Check that `path` setting in _Preferences/Package Settings/STNeverwinterScript/Settings_ leads to the NWNScriptCompiler script folder. If not, override it.

### Manual install :
- Clone/extract https://github.com/CromFr/STNeverwinterScript into the sublime package directory (%appdata%\Roaming\Sublime Text 3\Packages on windows)
- Check that `path` setting in _Preferences/Package Settings/STNeverwinterScript/Settings_ leads to the NWNScriptCompiler script folder. If not, override it.
