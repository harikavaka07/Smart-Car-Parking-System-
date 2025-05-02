# 🚗 Smart Parking System using STM32, IR Sensors & Bluetooth

This project demonstrates an automated smart parking gate system using IR sensors, a servo motor, and Bluetooth communication, all controlled by an STM32 microcontroller.

---

## 🛠️ Hardware Components
- **STM32 Microcontroller**  
- **IR Sensors**
  - **IR1 (PA0)**: Entry detection  
  - **IR2 (PA1)**: Exit detection  
- **Servo Motor**: For gate movement  
- **Bluetooth Module (HC-05/06)**  
  - TX → PA2  
  - RX → PA3  
- **Wires, Breadboard, Power Supply**

---

## ⚙️ How It Works

### 🚘 Vehicle Entry
- IR1 detects an approaching car.
- The microcontroller activates the servo motor to **open** the gate.
- After the car passes, the gate **closes automatically**.

### 🚙 Vehicle Exit
- IR2 detects the car leaving.
- The gate opens and then closes after exit.

### 📲 Bluetooth Control
- A mobile app communicates via Bluetooth to:
  - Monitor parking slot availability.
  - Manually open/close the gate.

---

## 💻 Software Details
- Programmed in C using STM32CubeIDE.
- Uses UART for Bluetooth communication.
- Handles real-time sensor detection and motor control logic.

---

## 🔧 Setup Instructions

1. **Connect hardware** as described above.
2. **Flash the code** to the STM32 board via STM32CubeIDE.
3. Use a Bluetooth terminal app (like Serial Bluetooth Terminal) to send commands or check status.
4. Test entry/exit detection with small vehicles or objects.

---


