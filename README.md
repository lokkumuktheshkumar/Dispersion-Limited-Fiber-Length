# Dispersion-Limited-Fiber-Length
Dispersion Limited Fiber Length
# Objective: 
 
Calculate the dispersion-limited fiber length for a fiber optic transport system that 
employs standard single-mode fiber and a directly-modulated single-mode laser diode 
transmitter. 
 
Simulate the resulting system and verify that it meets performance objective.  
 
# Theory: 
 
The maximum allowable dispersion (or pulse spread) <img width="76" height="52" alt="image" src="https://github.com/user-attachments/assets/52dff457-e7aa-4312-aef4-aa4e234afb47" /> is given in terms of the transmission rate R by the following engineering guideline <img width="192" height="124" alt="image" src="https://github.com/user-attachments/assets/4fcb3de9-6a4a-48db-ba5f-f020a6c85d8b" /> This guideline provides reasonable assurance that there will be no significant inter
symbol interference (ISI) due to pulse spread. 
 
For standard single-mode fiber driven by a directly-modulated laser diode transmitter, the 
pulse spread due to chromatic dispersion is given by
<img width="898" height="694" alt="image" src="https://github.com/user-attachments/assets/5499f4b0-2405-4a5f-b773-ce004a76e850" />
<img width="1300" height="974" alt="image" src="https://github.com/user-attachments/assets/bbd90891-43d6-4a5d-92d2-73ed3e4e57eb" />
# Layout: 
Open up the OptiPerformer file called “Dispersion Limited Fiber.osp”. This layout uses 
the Laser Rate Equations laser diode component with default parameters.  It models a 
directly modulated laser diode based using a standard rate equation model. One of the 
effects of this model is that it generates a signal with a spectral width of about 0.6 nm for 
the default parameters with 2.5 Gb/s, return to zero modulation. 
Within the layout, there are several “Visualizers.” The “Optical Time Domain 
Visualizers” allow the user to the view the simulated signal as a function of time. There is 
one at the output of the laser and one at the end of the fiber.  This allows the user to 
directly observe the changes in the pulses due fiber dispersion. The “Optical Spectrum 
Analyzer” allows the user to view the spectral content of the signal. It this lab it is used to 
verify that the spectral width is about 6 nm. The “BER analyzer” provides calculations of 
the Q factor, the bit error rate (BER) and provides a plot of the eye diagram. 
# Simulation:  
Set the laser power such to achieve a transmitter output power of 0 dBm. The transmitter 
power can be viewed by double clicking the “Output Power Meter Visualizer.” The 
power will read -100 dBm until the first run is made.  
Using the chromatic dispersion factor equation, determine the dispersion of the fiber at 
1550 nm and set the fiber dispersion parameter accordingly. 
Using the equations above, determine the dispersion-limited fiber length. 
<img width="1262" height="1044" alt="image" src="https://github.com/user-attachments/assets/e0b20ca6-42b4-4f1b-ac9a-e4f931a85001" />
# Calculation
<img width="902" height="1600" alt="WhatsApp Image 2026-05-14 at 2 34 59 PM" src="https://github.com/user-attachments/assets/69519ea7-ca5b-4f47-8a42-43887548c4ab" />
<img width="902" height="1600" alt="WhatsApp Image 2026-05-14 at 2 34 59 PM (1)" src="https://github.com/user-attachments/assets/4a99c629-954f-4182-9e3a-8787a3230362" />
# Tabulation
<img width="902" height="1600" alt="WhatsApp Image 2026-05-14 at 2 34 59 PM (2)" src="https://github.com/user-attachments/assets/2c7a194b-c21f-4678-8df7-666c7c3d6eff" />
# Output
<img width="959" height="557" alt="Screenshot 2026-05-14 142459" src="https://github.com/user-attachments/assets/2e4a9299-e213-4397-84fe-896ce8dcaddb" />
<img width="959" height="565" alt="Screenshot 2026-05-14 142713" src="https://github.com/user-attachments/assets/ba66e6f6-e4a1-42b0-b55f-4dc75ec1302e" />
<img width="959" height="566" alt="Screenshot 2026-05-14 142908" src="https://github.com/user-attachments/assets/762b9d2a-187a-4edd-b781-85ebe468355d" />
<img width="959" height="562" alt="Screenshot 2026-05-14 142927" src="https://github.com/user-attachments/assets/cd368ed8-aefe-42dd-b0e2-a3df1e328e73" />
<img width="959" height="565" alt="Screenshot 2026-05-14 142943" src="https://github.com/user-attachments/assets/f35c79d3-9645-4428-b976-fb3722c807b5" />

# Result
Thus, the output is verified.
