**Temperature Logger and Data Analyzer** is a Python project that collects temperature data from a logger, stores it in CSV format, and provides statistical analysis and graphical visualization, including real-time temperature changes and derivative calculations.

-----

# Temperature Logger and Data Analyzer

## Overview

**Temperature Logger and Data Analyzer** is a Python-based project designed to interface with a temperature monitoring device via a serial port. This project captures temperature data at configurable intervals, stores the data in CSV files, and provides both statistical analysis and graphical visualizations, including the temperature derivative. It is suitable for monitoring environmental conditions over extended periods.

## Features

- **Real-Time Temperature Logging**: Configurable data collection intervals from a connected data logger.
- **Data Persistence**: All logged data is saved in a CSV format for easy post-processing.
- **Statistical Analysis**: Automatic calculation of minimum, maximum, mean, and standard deviation of temperature readings.
- **Graphical Visualization**: Graphs displaying temperature changes over time and the rate of change (derivative).
- **User-Defined Sampling Intervals**: Flexible input for data collection frequency and duration.

## Project Structure

- `logger.py`: Main script to collect temperature data from a data logger and save it to a CSV file.
- `analysis.py`: Script to analyze the saved temperature data, compute statistics, and generate visualizations.
- `utils.py`: Helper functions for configuring the data logger and managing user inputs.

## How to Run the Project

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/temperature-logger-data-analyzer.git
    cd temperature-logger-data-analyzer
    ```

2. Install required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Configure the data logger:
   - Ensure your data logger is connected to the correct port (e.g., `COM15` on Windows or `/dev/ttyUSB0` on Linux).
   - Update the `config1.txt` file as per the device specifications.

4. Run the logger script to start collecting data:
    ```bash
    python logger.py
    ```

5. After data collection is complete, analyze and visualize the data:
    ```bash
    python analysis.py
    ```

## Sample Output

### Temperature Data Graph

![Temperature Data](path/to/graph.png)

The graph shows the temperature readings over time with the corresponding derivative (rate of temperature change).

## Future Improvements

- Implement real-time plotting of data during the acquisition process.
- Add support for multiple sensors and data loggers.
- Implement a web-based interface for remote monitoring.

## Requirements

- Python 3.x
- numpy
- matplotlib
- csv
- datetime
- uLogg

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

---

### Contributions

Feel free to contribute to this project by submitting issues or pull requests. All contributions are welcome!

---

### Contact

- **Author**: Santiago Ismael Flores Chávez
- **GitHub**: [santigoxfc](https://github.com/santigoxfc)


