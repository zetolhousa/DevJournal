- Two python version in Windows:
	1. Install both Py2 and Py3
	2. Make a copy of both Python.exe files for Py2 and Py3
	3. Rename one of the Python.exe in both locations to Py2.exe and Py3.exe respectively (Both are initially Python.exe)
	4. Add env paths of both locations, including their /Scripts dir
	5. Done
- Set alias in PowerShell
	- `Function <var_name> {Set-Location <full_path>}`
	- `Set-Alias -Name <the_alias> -Value <var_name>`
