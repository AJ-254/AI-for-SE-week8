# AutoParts Inc – Make.com Simulation Workflow

This folder contains the Make.com automation I built for the AI Agents Assignment.  
It simulates how AI Agents would work inside a real manufacturing setup.  
The flow covers machine data, defect alerts, maintenance checks, and supervisor notifications.

---

## 📌 What the Scenario Does

1. **Receives machine data**  
   A fake data generator sends values like temperature, vibration, and defect flags.

2. **Checks for defects**  
   When a defect is true, the flow starts a maintenance ticket.

3. **Schedules maintenance**  
   A row is added to a Google Sheet (or placeholder) to log the issue.  
   This acts like an “Agent” that handles internal factory tasks.

4. **Notifies a supervisor**  
   Gmail sends an alert email when a defect is detected.  
   This is the communication Agent.

5. **Shows a full workflow run**  
   The logs in Make show each step running from start to finish.

---

## 📁 Files in this Folder

| File | Description |
|------|-------------|
| `autoparts_make_scenario.blueprint.json` | Exported Make scenario you can import back into Make |
|`demo_run.mp4`| Screen recording of the full automation and sucessful run |
| `email_received.png` | Supervisor email alert screenshot |
| `make_workflow_canvas.png` | Screenshot of the full automation layout |
| `make_run_success.png` | Screenshot of a successful run |
| `ticket_sheet_row.png` | (Optional) Screenshot of logged maintenance ticket |
| `README_make_simulation.md` | This documentation |

---

## 🛠️ How to Import the Scenario

1. Sign in to Make.com  
2. Go to **Scenarios** → click **Import blueprint**  
3. Upload `autoparts_make_scenario.blueprint.json`  
4. Reconnect Gmail or Google Sheets if needed  
5. Click **Run once** to test

---

## 🧪 Sample Machine Data Used

```json
{
  "machine_id": "MCH-001",
  "temperature": 82.5,
  "vibration_level": 0.06,
  "defect_detected": true,
  "timestamp": "2025-11-26T11:05:00Z"
}
```

---

## 🔗 Make Scenario Link

[Public scenario link](https://eu1.make.com/public/shared-scenario/Hay7tDd8VgY/autoparts-make-scenario)

---

## Summary

This simulation shows how AI Agents can support a smart factory:

- One Agent watches machine signals
- One Agent handles maintenance
- One Agent alerts humans

---

## Author
[Juliet Asiedu](https://github.com/AJ-254)
