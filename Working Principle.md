## Working Principle

The transformerless power supply works by converting **230V AC mains into regulated 5V DC** without using a bulky transformer. Instead of reducing voltage directly, it uses a **capacitive dropper** to limit the current from the AC supply.

---

### Step 1 — AC Input

The 230V AC mains enters through the input terminal **J1**.

---

### Step 2 — Capacitive Current Limiting

The capacitor **C0** acts as a capacitive dropper.
It creates capacitive reactance which limits the amount of AC current flowing into the circuit.

X_C=\frac{1}{2\pi f C}

Because the capacitor limits current with very little heat loss, it is more efficient than using a large resistor.

The resistor **R3** acts as a bleeder resistor to safely discharge the capacitor when power is turned OFF.

---

### Step 3 — Rectification

The four diodes **D1, D2, D3, and D4** form a bridge rectifier.

Their function is to convert AC into pulsating DC by allowing current to flow in only one direction during both halves of the AC cycle.

---

### Step 4 — Filtering

The capacitors **C1** and **C2** smooth the pulsating DC output from the bridge rectifier.

* **C1** removes high-frequency noise.
* **C2** stores charge and reduces ripple voltage to provide smoother DC.

---

### Step 5 — Voltage Protection

The zener diodes **D5** and **D6** protect the circuit from excessive voltage.

If the voltage rises above the zener voltage rating, the zeners conduct and clamp the voltage to a safer level.

Resistors **R1** and **R2** limit the current through the zener diodes.

---

### Step 6 — Voltage Regulation

The IC **LM7805** regulates the filtered DC voltage and provides a stable 5V output.

It ensures that the output remains approximately constant even if the input voltage fluctuates slightly.

---

### Step 7 — Output Filtering and Indication

The capacitor **C3** improves output stability and reduces remaining ripple at the regulator output.

The LED **D7** with resistor **R4** acts as a power indicator showing that the supply is ON.

---

### Final Output

The regulated 5V DC output is available at terminal **J2** and can be used to power low-power electronic circuits such as microcontrollers and sensors.

---

## Important Note

⚠ This circuit is a **non-isolated power supply**, meaning the output is electrically connected to the AC mains. Proper insulation and safety precautions are mandatory while testing or operating the circuit.
