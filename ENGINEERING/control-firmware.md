# Control Firmware

## Overview [PILOT]
Embedded logic orchestrates everything—Python/MicroPython on MCU for user-friendly control, with ML hooks for adaptive resonances (e.g., biofeedback tuning).

## Key Specs
- Platform: ESP32/STM32 (WiFi for logs, $10-20).
- Language: MicroPython/C for real-time; Python for high-level scripts.
- Interfaces: LCD touch for ops, API for silicon integration (e.g., AI pattern feedback).
- Features: Session scripting, real-time monitoring, auto-adjust (e.g., ramp freq on HRV feedback).

## Code Snippet (Python Control Loop)
```python
import machine, time  # MicroPython imports

SAR_LIMIT = 1.6  # W/kg
def main_loop():
    while True:
        sar = read_sar_sensor()
        if sar > SAR_LIMIT * 0.8:
            warn_operator()
        if sar > SAR_LIMIT:
            emergency_shutdown()
        adjust_freq_based_on_feedback()  # ML hook
        time.sleep(0.1)  # 10Hz poll
