# krsbi-beroda-simulator
An open source simulator for KRSBI-B (Kontes Robot Sepak Bola Indonesia Beroda) or Wheeled Robot Soccer Simulator 

## Get to know the maintainer
My name is Danendra Clevero Ananda, an ex-programmer from IRIS ITS Robotics team. I have several experiences in robotics field such as:
<!-- make table -->
| Experience                 | Company           | Year start - Year end |
| :------------------------- | :---------------- | :-------------------- |
| Robot Programmer           | IRIS ITS Robotics | 2021 - 2024           |
| Robot UI Programmer        | Raisa ITS         | 2023 - 2024           |
| RnD Gazebo                 | PUI-AIHES         | 2023 - 2023           |
| ROS Engineer               | Widya Robotics    | 2024 - now            |
| Freelance Robotic Engineer | Kakarobot         | 2024 - now            |

## Why do i want to contribute?
A lot of campus have a grant amount of human resources, but not with the help from cash. Thus I want to make the robotics competition, esp. in wheeled robot soccer in KRI more alive
One of the way to do it is to build the simulator. Thus, I can contribute to the project and make the simulator more alive.

This repository is open-source, you're free to use it, as long as you include the copyright of this project. And also, if you have any idea to improve this project, you could do
[this](#how-to-contribute)

## How to contribute?
1. Fork this repository
2. Update the code from your local repository
3. Follow this [commit rule](#commit-rule)
4. Create a pull request
5. If the code is safe and good enough, I'll merge it.

## Commit rule
1. Commit message:
   1. [feature] Add new feature
   2. [bugfix] Fix bug
   3. [refactor] Refactor code
   4. [docs] Add documentation
   5. [style] Format code
   6. [ci] Run CI
   7. [revert] Revert commit
   8. [other] Other
   
   Example: ``` [feature] Add new feature ```

2. Commit description: Please describe your commit as follow
   1. What's node being changed? (in a list)
   2. What's the changes?
   3. What's the reason for the changes?
   4. What's the impact of the changes?

    Example:
    ```
    Changed node: Node x, y, z
    Changes:
    - add new node
    - change node properties
    - add node properties
    - change algorithm x
    Reason of change:
    - need more modular processing
    - need additional properties
    - found more efficient algorithm
    Impact of change:
    - xxxx
    ```
## Syntax Format:
1. Function name: PascalCase
   
   example: ```cpp void MyFunction() ```

2. Variable name (global): snake_case

   example: ```cpp float pose_x ```

3. Variable name (local): snake_case_

   example: ```cpp float pose_x_ ```

4. Constant name: UPPER_SNAKE_CASE

   example: ```cpp constexpr float PI = 3.14; ```

5. Class name: PascalCase

   example: ```cpp class MyClass {} ```

6. Enum name: PascalCase

   example: ```cpp enum MyEnum {} ```

7. Macro name: UPPER_SNAKE_CASE

   example: ```cpp #define DEG2RAD(x) (x * PI / 180.0)```

## Package structure

```bash
krsbi-beroda-simulator
│
├── include
│   └── krsbi-beroda-simulator
├── launch
├── meshes
├── src
├── urdf
├── world
│
├── .gitignore
├── CMakeLists.txt
├── LICENSE
└── package.xml

```

## How to use
1. Clone this repo to your src workspace
```bash
cd <ws_name>/src
git clone https://github.com/danendra10/krsbi-beroda-simulator.git
```

2. Build the package
```bash
cd ..
catkin_make
```

3. Try to launch the simulator
```bash
source devel/setup.bash
roslaunch krsbi_beroda_simulator main.launch
```