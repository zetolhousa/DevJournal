
Tkinter
======
- comes inbuilt with every Python setup
	```python
	import tkinter  #Tkinter in py2
	m = tkinter.Tk()
	#add stuff here
	m.mainloop()
	```
- arranging the window
  1. `pack()`   //simple pack elements
  2. `grid()`   //specific grids
  3. `place()`  //custom placement
	eg: `widget.pack()`
- to set canvas settings
  ```python
  canv = tkinter.Canvas(master, **kwargs)
  canv.pack()
  ```
- Widgets:
	-  `Label(parent, **kwargs)`
	- `Canvas(parent, **kwargs)`
- To overwrite basic Tk widgets:
	```python
	from tkinter import *
	from tkinter.ttk import *
	```
- Widgets available: `Button`, `Checkbutton`, `Entry`, `Frame`, `Label`, `LabelFrame`, `Menubutton`, `PanedWindow`, `Radiobutton`, `Scale` and `Scrollbar`
- Passing args to event in tkinter combobox:
	```python
	def onselection(event, id):
		print("selected combobox ID#",id)
	...
	cbox = Combobox(...)
	cbox.bind("<<ComboboxSelected>>", lambda event, id=i : onselection(event, id)
	...
	```
- Multiple elements in a grid cell
	```python
	#main window
	root = Tk()
	
	#frames 3X
	f10 = Frame(root)
	f11 = Frame(root)
	F12 = Frame(root)
	f10.grid(row=1, column=0)
	f11.grid(row=1, column=1)
	f12.grid(row=1, column=2)
	
	#buttons all inside f11 cell
	b1 = Button(f11)
	b2 = Button(f11)
	b3 = Button(f11)
	b1.pack()
	b2.pack()
	b3.pack()
	```
