# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
# DEVELOPED BY : GANESH R
# REG NO : 212222240029
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot
![PY1](https://github.com/ganesha360/Movement-of-Robot-Joints/assets/120884552/9408247d-d46e-4a56-abcf-b4c858a8ccf6)

### 2. robot.driveJoints(0,0,0,0,0,0)
![PY2](https://github.com/ganesha360/Movement-of-Robot-Joints/assets/120884552/f13e0caf-9e9a-46c9-948a-25344cae31c6)

### 3. Movement of Joint1
![PY3](https://github.com/ganesha360/Movement-of-Robot-Joints/assets/120884552/8ad75e78-2bff-4114-8279-12a9fba44316)

### 3. Movement of Joint2
![PY4](https://github.com/ganesha360/Movement-of-Robot-Joints/assets/120884552/394e9ab8-0db9-45b0-a69c-656b815596bf)


### 3. Movement of Joint3
![PY5](https://github.com/ganesha360/Movement-of-Robot-Joints/assets/120884552/a301f892-c70e-41ae-bc02-7ca6d0841131)


## Result 
Thus the different robots joints are moved with the help of python list.


