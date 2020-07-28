.config/fusuma/config.yml

swipe:
  3:
    left:
      command: 'xdotool key alt+Right'
    right:
      command: 'xdotool key alt+Left'
    up:
      command: 'xdotool key ctrl+alt+w'
    down:
      command: 'xdotool key F12'
  4:
    up:
      command: 'xdotool key ctrl+w'
    down:
      command: 'xdotool key ctrl+F5'
    left:
      command: 'xdotool key ctrl+Tab'
    right:
      command: 'xdotool key ctrl+Shift+Tab'
pinch:
  in:
    command: 'xdotool key ctrl+plus'
    threshold: 0.1
  out:
     command: 'xdotool key ctrl+minus'
     threshold: 0.1

threshold:
  swipe: 1
  pinch: 1

interval:
  swipe: 1
  pinch: 1
