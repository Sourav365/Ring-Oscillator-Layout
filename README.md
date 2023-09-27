# Ring-Oscillator-Layout

## 1.	Schematic of Ring Oscillator with 21 inverters
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/8431ecf3-b02d-4fb6-84eb-8fdb9094013f)


## 2.	Simulation of the above ring oscillator schematic 
  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/4dc5d2c0-ab3e-4e39-a699-6b5de7472d0e)

  ![image](https://github.com/Sourav365/Ring-Oscillator-Layout/assets/49667585/6e4e2d0a-b123-4e2f-8c4e-fe1e44e4cad8)


  **Results**
  * Propagation delay of Ring Oscillator = (tpLH + tpHL) / 2 = (1.11nSec + 1.11nSec) / 2 = 1.11nsec
  * Propagation delay of Each Inverter = 1.11nSec / (2*21) = 26.4 pSec

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
    
## 6. 
