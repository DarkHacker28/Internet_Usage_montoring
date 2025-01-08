# Internet Usage Monitoring using Python

## Overview
This project provides a simple Python script to monitor internet usage. It tracks data transfer (upload and download) in real-time and logs the usage over time. The script can be used to analyze network activity and ensure efficient bandwidth utilization.

## Features
- Real-time monitoring of internet usage (upload and download speeds).
- Logs data usage to a file for later analysis.
- Configurable update intervals.
- Lightweight and easy to set up.

## Prerequisites
- Python 3.6 or later
- Required Python libraries:
  - `psutil`
  - `time`
  - `csv` (built-in)

You can install `psutil` using pip:
```bash
pip install psutil
```

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/internet-usage-monitoring.git
   ```
2. Navigate to the project directory:
   ```bash
   cd internet-usage-monitoring
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the script:
   ```bash
   python monitor.py
   ```
2. The script will display real-time upload and download speeds in the console.
3. Logs will be saved to a file named `internet_usage_log.csv` in the same directory.

## Configuration
You can configure the monitoring behavior by editing the `monitor.py` file:
- **Update Interval:** Change the `INTERVAL` variable to set the time interval (in seconds) for monitoring updates.
- **Log File Name:** Modify the `LOG_FILE` variable to specify a custom log file name.

## Example Output
### Console Output:
```
Time: 12:00:00 | Download Speed: 3.5 Mbps | Upload Speed: 1.2 Mbps
Time: 12:00:01 | Download Speed: 3.8 Mbps | Upload Speed: 1.1 Mbps
```

### Log File (`internet_usage_log.csv`):
```
Timestamp,Download Speed (Mbps),Upload Speed (Mbps)
2024-01-08 12:00:00,3.5,1.2
2024-01-08 12:00:01,3.8,1.1
```

## Contributing
Contributions are welcome! Feel free to:
- Open an issue for bugs or feature requests.
- Submit a pull request with improvements or bug fixes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Inspired by the need for lightweight internet usage tracking tools.
- Thanks to the contributors of the `psutil` library for their excellent work.

