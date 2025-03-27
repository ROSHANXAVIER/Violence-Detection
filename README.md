# Violence Detection System using CNN-LSTM

A real-time violence detection system that uses a hybrid Convolutional Neural Network (CNN) and Long Short-Term Memory (LSTM) model. This system is designed for implementation in CCTV networks of high-security environments like jails and mental asylums. Upon detecting violent activity, the system captures a snapshot, identifies the involved individuals, and sends an alert to a Telegram bot with the incident details.

## Features
- **Real-Time Violence Detection:** Utilizes a CNN-LSTM model to analyze CCTV footage and detect violent activities.
- **Telegram Bot Notifications:** Sends alerts containing:
  - Location of the incident
  - Timestamp
  - Snapshot of the event
  - Detected faces of culprits
- **Face Detection:** Extracts and identifies the individuals involved in the violent act.
- **Scalable and Deployable:** Designed for continuous surveillance in sensitive areas.

## Project Structure
```
.
├── cnn_lstm.py               # Main model script
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation
```

## Prerequisites
Ensure you have the following installed:
- Python 3.x
- OpenCV
- TensorFlow/Keras
- Telegram Bot API

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/violence-detection-system.git
   cd violence-detection-system
   ```

2. Set up a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up your Telegram bot:
   - Create a bot on Telegram using [BotFather](https://t.me/botfather)
   - Obtain the bot token
   - Update the bot token in the script

## Usage

1. Run the violence detection script:
   ```bash
   python cnn_lstm.py
   ```

2. Monitor your Telegram bot for alerts on violent activities.

## Model Overview

The model integrates:
- **CNN (Convolutional Neural Network):** Extracts spatial features from video frames.
- **LSTM (Long Short-Term Memory):** Captures temporal dependencies across video sequences.

Workflow:
1. Capture real-time video from CCTV.
2. Analyze frame sequences with CNN-LSTM.
3. Detect violent actions and extract faces.
4. Send incident reports to the Telegram bot.

## Customization
- **Modify Detection Sensitivity:** Adjust the model's sensitivity thresholds in `cnn_lstm.py`.
- **Telegram Bot Integration:** Ensure your bot token and chat ID are correctly set.

## Future Enhancements
- Improve model accuracy with a larger dataset.
- Implement multi-camera support.
- Enhance face recognition with a database of known individuals.

## Contributions
Contributions are welcome! Feel free to fork this repository and submit a pull request.

## License
This project is licensed under the MIT License. See `LICENSE` for more details.

![image](https://github.com/user-attachments/assets/db5d6533-697b-4f1e-a82a-53597ec0bf27)


