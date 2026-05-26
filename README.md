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
# Tabulation
<img width="1265" height="667" alt="image" src="https://github.com/user-attachments/assets/4e1cf557-1b7d-4651-9c0b-be4c01beedce" />

<img width="1260" height="662" alt="image" src="https://github.com/user-attachments/assets/a0ce64c9-3821-4e28-a5f6-d4eae824edf2" />

<img width="1262" height="666" alt="image" src="https://github.com/user-attachments/assets/22a8a70c-8027-4aaa-aaae-a4cf445de92e" />

<img width="1256" height="672" alt="image" src="https://github.com/user-attachments/assets/c08cb901-3b7e-45bc-aa17-a0bf09703c6c" />

<img width="1263" height="665" alt="image" src="https://github.com/user-attachments/assets/c9981265-0f88-4dde-9a62-89ff705cd505" />


<img width="859" height="1599" alt="WhatsApp Image 2026-05-26 at 8 17 27 PM" src="https://github.com/user-attachments/assets/839af387-38db-481a-80d0-6bfbb5cfe360" />
<img width="804" height="748" alt="WhatsApp Image 2026-05-26 at 8 17 28 PM" src="https://github.com/user-attachments/assets/0c92780c-f138-4867-9000-18590a1b9302" />

# Result
The dispersion-limited fiber length for the given optical communication system was found to be approximately 10 km. The simulation results showed acceptable BER performance with a clear eye diagram and minimal intersymbol interference. Hence, the system performance was satisfactory and remained within the allowable dispersion limit.
