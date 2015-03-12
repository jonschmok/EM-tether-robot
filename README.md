# EM-tether-robot
Project 2: Electromagnetic tether robot for EECE 282

Requirements:
  - Use f38x boards
  - battery operated - AA battery holder in lab kit
  - Any material can be used for robot chassis
    Material from workshop can be expensive - also need safety training, goggles and safety shoes
    Parts given to us in kit ($40):
      - Solarbotics GM4 Gear Motor 4 - Clear Servo
      - Lynxmotion Servo Wheel 2.63" x 0.35" (pair)
      - ￼Tamiya 70144 Ball Caster
      - ￼4 x AA Battery holder
      - ￼1 x 9V cable 9V battery clip
      - Unfolded chassis Aluminum chassis made using the water jet cutter.
  - Must be completed in C
  - Must use MOSFETs to drive and control motors of robot - NMOS and PMOS given to us
    May need optocouplers to isolate noisy motors (LTV847)
    Need to go forward, backward, left and right
  - Transmitter:
    One microcontroller for robot, another to transmit EM signal at a constant frequency
    Robot controller reads signal using inductive sensors and determines its distance and direction from beacon, adjusts
    Transmitter must send commands to robot:
      - 0 move closer
      - 1 move farther
      - 2 rotate 180
      - 3 turn front LED on/off
      - 4 turn back LED on/off
      - 5 Beep for 1 sec
      - 6 parallel park
      - at least 5 preset distances in "move closer"/"move farther"
      - display command # on 7 seg display
  - Distance:
    Robot must be able to track transmitter when seperated by at least 100cm - farther is better
    Bonus feature: 200cm
    Tranmitter/receiver design http://ww1.microchip.com/downloads/en/AppNotes/00232B.pdf
