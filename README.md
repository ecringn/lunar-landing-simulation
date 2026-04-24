-->Lunar Landing Simulation 
This project is a Python-based simulation that models a spacecraft's landing on the Moon. It calculates how altitude and velocity change over time under the influence of lunar gravity (1.62 m/s^2).

->How It Works (Logic & Physics)
The simulation runs a loop that calculates the following every second:
Altitude: The craft's height is updated by subtracting the distance fallen from the starting height.
Velocity: Speed is calculated based on lunar gravity and the time elapsed.
Ground Control: To keep the simulation realistic, a check ensures the craft never goes below 0 meters. If it hits the ground, the altitude is fixed at 0.

->Flight States
As the craft descends, its status is updated based on its current altitude:
Safe: When the craft is above 50 meters.
Descent: Between 10 and 50 meters.Critical: When the craft is at 10 meters or less.
Landing: Once the craft successfully touches the lunar surface (0 meters).

->Safety Feature
The system includes an automatic warning: if the craft's speed exceeds 15 m/s, a "Dangerous speed!" alert is triggered. In a standard test starting from 105 meters, this danger level is typically reached at the 10th second.
->Visual Results
Below is a screenshot of the simulation running in the terminal, showing the step-by-step analysis:
