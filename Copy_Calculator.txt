import pyautogui
import subprocess                                                       # Needed to open an executable
import time                                                             # Needed to call time to count/pause
import psutil,os                                                        # Needed for closing an executable

# Open the calculator, and pause for 2 seconds before executing, this gives the calculator time to open.
subprocess.Popen('C:\\Windows\\System32\\calc.exe')                     # Open windows calculator
time.sleep(2)                                                           # wait 2 seconds

pyautogui.click(pyautogui.locateCenterOnScreen('9.png'))                # Locates & clicks the 9 location on the screen from a screenshot.
pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             # Locates & clicks the + location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
#pyautogui.click(pyautogui.locateCenterOnScreen('7.png'))               # Locates & clicks the 7 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
#pyautogui.click(pyautogui.locateCenterOnScreen('6.png'))               # Locates & clicks the 6 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
#pyautogui.click(pyautogui.locateCenterOnScreen('5.png'))               # Locates & clicks the 5 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
#pyautogui.click(pyautogui.locateCenterOnScreen('4.png'))               # Locates & clicks the 4 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))            
#pyautogui.click(pyautogui.locateCenterOnScreen('3.png'))               # Locates & clicks the 3 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
#pyautogui.click(pyautogui.locateCenterOnScreen('2.png'))               # Locates & clicks the 2 location on the screen from a screenshot.
#pyautogui.click(pyautogui.locateCenterOnScreen('plus.png'))             
pyautogui.click(pyautogui.locateCenterOnScreen('1.png'))                # Locates & clicks the 1 location on the screen from a screenshot.
pyautogui.click(pyautogui.locateCenterOnScreen('Equal.png'))            # Locates & clicks the = location on the screen from a screenshot.

time.sleep(5)                                                           # wait 5 seconds to view the results

os.system("TaskKill /F /IM CalculatorApp.exe")                          # Close windows calculator