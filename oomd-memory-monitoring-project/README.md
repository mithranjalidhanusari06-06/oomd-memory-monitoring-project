# OOMD Memory Monitoring Project

A college project demonstrating the build, configuration, and testing of Facebook's OOMD (Out-Of-Memory Daemon) on Ubuntu 24.04 LTS.

## Objectives

- Build the existing OOMD source code.
- Understand Linux cgroups v2 and Pressure Stall Information (PSI).
- Configure memory-pressure monitoring.
- Run automated tests and record results.

## Technologies Used

- Ubuntu 24.04 LTS
- C++
- Meson and Ninja
- Linux cgroups v2
- Linux Pressure Stall Information (PSI)
- Git and GitHub

## Project Structure

- `configs/demo-pressure.json` — safe monitoring configuration.
- `results/project-summary.txt` — project version and configuration summary.
- `results/testlog.txt` — automated test log.

## Demonstration Configuration

- Detector: `pressure_above`
- Resource: `memory`
- Cgroup: `system.slice`
- Threshold: 60
- Duration: 30 seconds
- Action: `continue`

The demonstration uses the `continue` action and does not intentionally kill processes.

## Test Results

- Tests passed: 16
- Tests failed: 0
- Tests skipped: 0

## Limitations

The demonstration ran under low memory pressure. Genuine high memory pressure and process-killing behavior were not tested.


