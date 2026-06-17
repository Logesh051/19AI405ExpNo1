# Exp No: 1 – Developing AI Agent with PEAS Description

### Name: LOGESH.N.A

### Register Number: 212223240078

## AIM

To find the PEAS description for the given AI problem and develop an AI agent.

---

## THEORY

### Medicine Prescribing Agent

A medicine prescribing agent is an intelligent agent used in a hospital environment. The agent checks the temperature of patients and prescribes medicine when the temperature is greater than 98.5°F. The environment consists of hospital rooms containing patients.

The agent moves between rooms, identifies unhealthy patients, and provides treatment. The performance of the agent increases whenever treatment is provided and decreases whenever the agent moves from one room to another.

Thus, the agent helps in identifying and treating unhealthy patients efficiently.

---

## PEAS DESCRIPTION

| Agent Type                 | Performance Measure                         | Environment     | Actuators           | Sensors               |
| -------------------------- | ------------------------------------------- | --------------- | ------------------- | --------------------- |
| Medicine Prescribing Agent | Treating unhealthy patients, agent movement | Rooms, Patients | Medicine, Treatment | Location, Temperature |

---

## DESIGN STEPS

### Step 1: Identifying the Input

* Patient Temperature
* Room Location

### Step 2: Identifying the Output

* Prescribe medicine if the patient has fever.

### Step 3: Developing PEAS Description

* Performance Measure
* Environment
* Actuators
* Sensors

### Step 4: Implementing the AI Agent

* Check patient condition.
* Treat unhealthy patients.
* Move between rooms.

### Step 5: Measure Performance

* Treatment → Performance increases.
* Movement → Performance decreases.

---

## ALGORITHM

Step 1: Start.

Step 2: Read patient's temperature.

Step 3: Check the room location.

Step 4: If temperature > 98.5°F, identify patient as unhealthy.

Step 5: Prescribe medicine.

Step 6: Increase performance score.

Step 7: Move to another room.

Step 8: Repeat until all rooms are checked.

Step 9: Stop.

---

## PROCEDURE

1. Create a medicine prescribing agent.
2. Define hospital rooms as environment.
3. Read temperature using sensors.
4. Identify healthy or unhealthy patients.
5. Prescribe medicine for unhealthy patients.
6. Update performance measure.
7. Display treatment status and performance.

---

## PROGRAM

```python
import random

class MedicineAgent:

    def __init__(self):
        self.performance = 0

    def check_patient(self, temp):

        if temp > 98.5:

            print("Patient is Unhealthy")
            print("Medicine Prescribed")

            self.performance += 10

        else:

            print("Patient is Healthy")

agent = MedicineAgent()

temperature = float(input("Enter Temperature: "))

agent.check_patient(temperature)

print("Performance =", agent.performance)
```

---

## OUTPUT

```text
Enter Temperature: 100

Patient is Unhealthy

Medicine Prescribed

Performance = 10
```

---

## RESULT

Thus, the PEAS description for the given AI problem was developed and an AI agent was successfully implemented using Python.
