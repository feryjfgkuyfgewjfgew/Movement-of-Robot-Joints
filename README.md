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
```

Developed by: naresh.r
RegisterNumber: 23005559
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

![Screenshot 2023-12-31 171107](https://github.com/feryjfgkuyfgewjfgew/Movement-of-Robot-Joints/assets/150319377/c7d1b8a6-6253-4f7e-97e9-2ba3744cb929)

### 2. robot.driveJoints(0,0,0,0,0,0)

![Screenshot 2023-12-31 171116](https://github.com/feryjfgkuyfgewjfgew/Movement-of-Robot-Joints/assets/150319377/26137577-65db-482f-95c1-cd0313aa0e7f)

### 3. Movement of Joint1

![Screenshot 2023-12-31 171127](https://github.com/feryjfgkuyfgewjfgew/Movement-of-Robot-Joints/assets/150319377/0d4e387d-d1a2-42c6-9059-a4b8788218dc)

### 3. Movement of Joint2

![Screenshot 2023-12-31 171135](https://github.com/feryjfgkuyfgewjfgew/Movement-of-Robot-Joints/assets/150319377/b3d685df-5338-4a8e-a719-601a0e8da61d)

### 3. Movement of Joint3

![Screenshot 2023-12-31 171143](https://github.com/feryjfgkuyfgewjfgew/Movement-of-Robot-Joints/assets/150319377/077bcdf8-4ddd-4ba2-977b-da92e8f1fb52)


## Result 
Thus the different robots joints are moved with the help of python list.
