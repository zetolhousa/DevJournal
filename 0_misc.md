Random stuff
============
- Two python version in Windows:
	1. Install both Py2 and Py3
	2. Make a copy of both Python.exe files for Py2 and Py3
	3. Rename one of the Python.exe in both locations to Py2.exe and Py3.exe respectively (Both are initially Python.exe)
	4. Add env paths of both locations, including their /Scripts dir
	5. Done
- Set alias in PowerShell
	- `Function <var_name> {Set-Location <full_path>}`
	- `Set-Alias -Name <the_alias> -Value <var_name>`
- Setting up WSL
	- Set aliases file **.bash_aliases**
	- Set proxy **/etc/apt/apt.conf**
		- `Acquire::http::Proxy "http://...@...:xxx";`
	- Sudo apt update
	- Sudo apt install build-essential
	- Sudo apt install python3, python3-pip
- Linux commands
	- To see and also save command ouputs [src](https://askubuntu.com/a/731237)
		- `<cmd> |& tee output_file`
	- See apt installed packages
		- `apt list --installed`
