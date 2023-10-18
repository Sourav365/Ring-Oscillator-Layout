# Ring-Oscillator-Layout

* For inverter, (W/L)PMOS = 2* (W/L)NMOS
 
## 1.	Schematic of Ring Oscillator with 21-Inverters
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/8431ecf3-b02d-4fb6-84eb-8fdb9094013f)


## 2.	Simulation of the above Ring Oscillator Schematic 
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/4dc5d2c0-ab3e-4e39-a699-6b5de7472d0e)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/6e4e2d0a-b123-4e2f-8c4e-fe1e44e4cad8)


  **Results**
  * Time Period(T) of Square-Wave Output of Ring Oscillator (without Parasitics) = (tpLH + tpHL) / 2 = (1.11nSec + 1.11nSec) / 2 = 1.11nsec
  * Propagation delay of Each Inverter (without Parasitics) = 1.11nSec / (2*21) = 26.4 pSec

## 3. Layout of Ring Oscillator
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/e44d0c9a-6fb7-45ef-a357-a39fe200caf8)

  <img width="1000" alt="image" src="https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/1cc82f6e-d184-46a0-96c5-35566391c7f7">


  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/2b13bbe2-b4a5-4ef6-b315-9895a31db146)

## 4. DRC (Design Rule Check)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/985add90-ac86-4a0a-a06e-0ce94795ab8b)

  * Minimum Metal (M-1 to M-6) and Poly density error is coming only.
  * It can be neglected by putting some dummy transistors.

## 5. LVS (Layout Versus Schematic) Check
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/98e40dcc-c240-4f4a-8a65-1dc1ef3c19e0)

  * No LVS and ERC error.
    
## 6. PEX (Parasitic Extraction)
  Resistor (R), Capacitor (C), Coupling Capacitor(CC) of all the nets are given:
  
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/6731c195-c117-4438-933e-22d956eb4ede)

  Schematic after Parasitic Extraction
  
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/1f8959f0-e3f7-4c6f-8fb4-9a32c36b886a)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/6e878d7f-a8c0-40e2-adc2-f9fc40d05ec3)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/593d0875-e6ed-423f-ab63-91ed5a33d9d3)
  
## 7. Post Layout Simulation
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/4e91a6c9-7ee4-44b6-935e-c6b673ce8f39)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/39ca951c-47aa-48ca-aae1-251cfd8c19cd)

  **Results**
  * Time Period(T) of Square-Wave Output of Ring Oscillator (with Parasitics) = (tpLH + tpHL) / 2 = (1.59nSec + 1.59nSec) / 2 = 1.59nsec
  * Propagation delay of Each Inverter (with Parasitics)= 1.59nSec / (2*21) = 37.8 pSec
  * Spikes during transition comes, due to the internal capacitors of gates. Cap don't allows sudden change of voltage. When i/p High, o/p Low. When i/p goes from H -> L, o/p 1st goes to low (due to C), then increases.
  * Intermidiate cap of each inverter causes variation of signal for a particular logic level.





