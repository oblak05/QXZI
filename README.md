# QXZI Auto Boosting Tool (auto_boost.py)

## Features
- Interactively choose a service from a predefined list.
- Place orders via the panel.
- Automatic re-order with configurable interval and cooldown between completed orders.
- Counts placed, successful and failed orders and prints a summary.

## Requirements
- Python 3.8+
- requests library

Install dependency:
```
pip install requests
```

## Usage
- On start you will be prompted to select a service (1..10).
- Provide the target link/post URL.
- Optionally set:
  - Cooldown in seconds (time to wait after a completed order before placing next)
  - Status check interval (seconds between polls)
  - Total number of orders to place (or press Enter to run indefinitely)
- Stop at any time with Ctrl+C.

Example interactive session:
- Choose service 2 (TikTok Views)
- Enter link: https://www.tiktok.com/@user/video/12345
- Cooldown: 60
- Poll interval: 8
- Orders: 10

Script prints progress and a final summary.

## Services List (as defined in the script)
- 1 — TikTok Likes (qty 50)
- 2 — TikTok Views (qty 100)
- 3 — Instagram Likes (qty 10)
- 4 — Instagram Followers (qty 10)
- 5 — Facebook Followers (qty 10)
- 6 — FB Heart Reacts (qty 10)
- 7 — FB Care Reacts (qty 10)
- 8 — FB HAHA Reacts (qty 10)
- 9 — FB Sad Reacts (qty 10) 
- 10 — FB WOW Reacts (qty 10)
