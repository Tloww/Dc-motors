# DC Motors with L293D + LCD (I2C) — Arduino (Tinkercad)

##  Task
1. Run **two DC motors** forward for **30 seconds**.  
2. Run both motors **backward for 60 seconds**.  
3. Alternate between **Right** and **Left** turns for **1 minute** total.  
4. Display the current state + countdown timer on the **LCD 16×2 (I2C)**.

---

## 🔗 Tinkercad Project
👉 [Open Simulation](https://www.tinkercad.com/things/5ZbIYDgJ1z6-dc-motors?sharecode=ZAxhKS-TyMW3hQCijZeza_jZ7IzrHD5zA3R6DDBqVkQ)

---

##  Components
- Arduino Uno  
- L293D Motor Driver (L298N equivalent also works)  
- 2 × DC Motors  
- 9V Battery (for motor power only)  
- Breadboard + jumper wires  
- LCD 16×2 with **I2C module**  

---

##  Wiring Overview

### L293D Motor Driver
- **ENA → D11**  
- **ENB → D3**  
- **IN1 → D9**, **IN2 → D10** (Motor 1)  
- **IN3 → D5**, **IN4 → D6** (Motor 2)  
- **Vcc1 (logic)** → Arduino 5V  
- **Vcc2 (motor power)** → 9V battery  
- **GND shared**: Arduino + Driver + Battery

### LCD (I2C)
- **GND → GND**  
- **VCC → 5V**  
- **SDA → A4**  
- **SCL → A5**  


---

##  Motion Logic
- **Forward** → Both motors spin forward.  
- **Backward** → Both spin backward.  
- **Right** → Left motor forward, right motor backward (turns right).  
- **Left** → Right motor forward, left motor backward (turns left).  

---

## 🖼️ Screenshots
Add your simulation screenshots here (upload to `images/` folder in your repo):

```md
![Forward](images/forward.png)
![Backward](images/backward.png)
![Right](images/right.png)
![Left](images/left.png)
