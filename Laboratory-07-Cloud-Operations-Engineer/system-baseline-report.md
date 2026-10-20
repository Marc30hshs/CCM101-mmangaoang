# System Baseline Report

## Mission Overview
This report documents the initial health check of the Linux server before deploying the client website.

## Memory (RAM) Check
- **Total RAM:** [Enter total RAM from `free -h`]
- **Used RAM:** [Enter used RAM]
- **Available RAM:** [Enter available RAM]

## Disk Storage Check
- **Root Filesystem (/):** [Enter size from `df -h /`]
- **Used Storage:** [Enter used storage]
- **Available Storage:** [Enter available storage]

## CPU and Running Processes
The `top` command was used to observe CPU utilization, memory usage, and active processes running on the server.

## Why Disk Monitoring Is Important
Checking disk space is critical before a massive traffic surge because insufficient storage can prevent applications from writing logs, saving data, and operating correctly.

## Evidence
- `screenshots/memory-check.png`
- `screenshots/disk-check.png`
