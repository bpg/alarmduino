# Usage Scenarios

##Idle: Control Panel
- shows current time
- shows current local temperature and humidity
- shows detailed status of sensors, exceptp motion sensor
- shows pictogram of motion sensor status
- does not react on keyboard
- pressing of button 1 initiates switch to "stay" armed mode
- pressing of button 2 initiates switch to "away" armed mode


Switching to armed mode:
- "stay"  
 - if any of sesnsors except motion sensor is open then switch to armed mode should be declined with
  - sound signal 1
  - 2-times blink of red strip on strip indicator
 - otherwise switch to *Armed "stay"* mode

- "away"  
 if any of sesnsors is open then switch to armed mode should be declined with
 - sound signal 1
 - 2-times blink of red strip on strip indicator
 - otherwise switch to *Prepare to arm* mode

## Prepare to arm
- starts from 30 seconds countdown
  - play a "start contdown signal"
  - all 10 strips on strip indicator should be lit
  - message on the screen: PREPARE TO ARM, LEAVE THE HOUSE!
- every 1 second play a "countdown sugnal 1"
- every 3 seconds turn off one strip on strip indicator
- when 9 seconds lef, play "countdown signal 2" instead of "contdown signal 2"
- when 0 seconds left: switch to *Armed away* mode

## Armed "away"
- play "armed signal"
- message on screen: ARMED
- if any of sensors triggered: swith to *Prepare to Alarm* mode


## Prepare to Alarm
- starts from 10 seconds countdown
  - continiously play "alarm" signal (?)
  - all 10 strips on strip indicator should be lit
  - message on the screen: ALARM! with displaying current status of sensors
- listening for keyboard events (?)
- listening for NFC events (?)

## Alarm


## Armed "stay"
