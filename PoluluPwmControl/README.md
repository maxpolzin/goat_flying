.ino sketch that runs on a small XIAO ESP32 C3 on the GOAT that translates the pwm signal from the PX4 to a signal that is accepted by the polulu motor driver that drives the frame tendons.

I don't remember why this was necessary. It seems like the polulu motor driver needed a higher frequency pwm signal than the px4 generates.

Better would be (now that we can configure pwm passthrough with SBUS and the new remote) to map inputs from a single pwm channel to the polulu motors.

