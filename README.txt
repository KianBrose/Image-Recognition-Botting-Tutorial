# Image-Recognition-Botting-Tutorial
Hello! This is the code I use in the https://www.youtube.com/watch?v=YRAIUA-Oc1Y video

Install these libraries from an administrator terminal (windows):

pip install pywin32
pip install keyboard
pip install pyautogui
pip install opencv-python

Here are the libraries to paste at the start of the scripts:

from pyautogui import *
import pyautogui
import time
import keyboard
import random
import win32api, win32con

Here is the click function:

def click(x,y):
    win32api.SetCursorPos((x,y))
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN,0,0)
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP,0,0)
