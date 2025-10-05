# PyAutoGUI Cheatsheet

## 1. Screen Info
```python
import pyautogui as pg

pg.size()          # Returns screen width & height
pg.position()      # Current mouse position
pg.onScreen(x, y)  # Check if position is on screen
```
## 2. Mouse Control
```python
pg.moveTo(x, y, duration=1)    # Move to (x, y)
pg.moveRel(x, y, duration=1)   # Move relative
pg.dragTo(x, y, duration=1)    # Drag to (x, y)
pg.dragRel(x, y, duration=1)   # Drag relative
pg.click(x, y)                 # Left click
pg.doubleClick(x, y)           # Double click
pg.rightClick(x, y)            # Right click
pg.middleClick(x, y)           # Middle click
pg.mouseDown(x, y)             # Hold down button
pg.mouseUp(x, y)               # Release button
pg.scroll(amount)              # Scroll (pos=up, neg=down)
```
## 3. Keyboard Control
```python
pg.write("Hello")               # Type string
pg.press("enter")               # Press key
pg.keyDown("shift")             # Hold key down
pg.keyUp("shift")               # Release key
pg.hotkey("ctrl", "c")          # Combination
```
## 4. Screenshots & Image Recognition
```python
pg.screenshot("file.png")       # Take screenshot
pg.locateOnScreen("img.png")    # Find image on screen
pg.locateCenterOnScreen("img.png")  # Get center coords
```
## 5. Alerts & Prompts
```python
pg.alert("Message")              # Simple alert
pg.confirm("Question?")          # OK/Cancel
pg.prompt("Input something:")    # Text input
```
## 6. Safety
```python
pg.FAILSAFE = True               # Move mouse to top-left to stop
pg.PAUSE = 0.5                   # Pause between actions
```
## 7. Safety
```python
pg.FAILSAFE = True               # Move mouse to top-left to stop
pg.PAUSE = 0.5                   # Pause between actions
```
