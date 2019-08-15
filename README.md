
# -*- coding: utf-8 -*-

from tkinter import *

def ___3():#info 
    a=' _1   -> menubar'
    b='__2  -> root or win needed -> GUI will not be stay'
    c='___3 -> def name'
    d='____4 -> Entry+pack+bind -> all'
    print(a+'\n',b+'\n',c+'\n',d)


def setText(word):
        v.set(word)
        
def _change(____4):
     from datetime import datetime
     e=Entry(win)
     win.title(____4.widget.get()+"__jh__"+datetime.now().strftime('%Y-%m-%d %H:%M:%S'))
     e.pack()
     e.bind("<Return>", _change)
     e.pack(ipadx=735)
     print("Entry+pack+bind -> all -> one more")
     print(____4.widget.get())
     
win = Tk()

_1 = Menu(win)
win.title("jh")

#---------menu add 
_2 = Menu(_1, tearoff=1)
_2.add_command(label='Path',command=___3)
_1.add_cascade(label="Path", menu=_2)

_1.add_cascade(label='Help', command=___3)

____4 = Entry(win)
____4.pack(ipadx=735)
____4.bind("<Return>", _change)


win.config(menu=_1)
win.mainloop()
