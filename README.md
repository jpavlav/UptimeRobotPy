# UptimeRobotPy

This is a simple library to implement easy interaction with the UptimeRobot API.

## Getting Started

The latest stable release is available from Pypi:

```
pip install uptimerobotpy
```

Otherwise you can install from git:
```
pip install git+https://github.com/jpavlav/UptimeRobotPy.git
```

## Usage

```python
>>> from uptimerobotpy import UptimeRobot
>>> up_robot = UptimeRobot(api_key=UPTIMEROBOT_API_KEY)
>>> up_robot.get_monitors()
```
If no api_key is passed during instantiation, we try to handle this by creating a config file (~/.uptimerobot.ini) to read from:

```python
>>> from uptimerobotpy import UptimeRobot
>>> up_robot = UptimeRobot()
Enter UptimeRobot API key: XXXXXXXXXXXXXXXX
>>> up_robot.get_monitors()
```

The above config file is formatted as follows and can be created preemptively if you wish:

```python
[UPTIMEROBOT]
api_key = XXXXXXXXXXXXXXXX
```
### Prerequisites

```
Python3
```

## Built With

* [Python3](https://www.python.org/downloads/) - Beautiful language.

## Authors

* **Justin Palmer** - *Urrverything* - [Me](https://github.com/jpavlav)

## Acknowledgments

* Kenneth Reitz -> [setup](https://github.com/kennethreitz/setup.py) - Thanks!
* Kamori -> [Cool Guy](https://github.com/Kamori) - Thanks to you as well!
