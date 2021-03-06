# Make-FirefoxApplication

A PowerShell script to:

* Automate download and creation of a customized Firefox ESR installer package
* Include support for user interaction with AppDeployToolkit
* Create a ready-to-deploy Application object in Configuration Manager (SCCM)

This is a fork of <https://github.com/hewipera/Make-FirefoxAppSource>.

Added features:

* Extract Firefox setup files with 7Zip to avoid having to run the script elevated
* Support PSAppDeployToolkit directory structure
* Support PSAppDeployToolkit with 32-bit ServiceUI.exe by running the installation as 32-bit process
* Make string replacements in files configurable with XML config file
* Create SCCM Application and Deployment Type


The script doesn't enable completely automated workflow. Manual work is required in SCCM to:

* Supercede previous Firefox version (No can do in PowerShell?)
* Create the deployments (This is possible in PowerShell, but I prefer doing it manually just in case)

# Credits

Contributors:

- hewipera (<https://github.com/hewipera>)
- Jaakko Luoto (<https://github.com/jaluoto>)
