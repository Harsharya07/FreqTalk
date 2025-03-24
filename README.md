Frequency-Based Communication Between Two Machines
This project enables two machines to communicate using Multiple Frequency Shift Keying (MFSK). It consists of a sender that converts text into audio signals and a receiver that decodes the signals back into text.

Features
Uses MFSK modulation to transmit data via sound.

Supports ASCII character encoding with frequency mapping.

Works with standard microphones and speakers.

Implemented using Python and sounddevice.

How It Works
Sender (sender_speaker.py)

Converts text into an MFSK-encoded audio signal.

Plays the audio through the speaker.

Receiver (receiver_mic.py)

Records the MFSK audio signal via a microphone.

Decodes the frequencies back into text.

Installation
Prerequisites
Python 3.x

Required libraries:

pip install numpy sounddevice
Usage
Sending a Message
Run the sender script:

python sender_speaker.py
Enter the message you want to send.

The message is transmitted as an audio signal.

Receiving a Message
Run the receiver script:

python receiver_mic.py
Enter the expected duration of the recording (in seconds).

The script will listen and decode the received message.

MFSK Parameters
Base Frequency: 500 Hz

Step Frequency: 60 Hz per character

Duration per Character: 0.025 seconds

Sample Rate: 44.1 kHz

Potential Applications
Offline data transmission between devices.

Low-cost machine-to-machine communication without the internet.

Educational experiments in digital signal processing.

Limitations & Future Improvements
Sensitive to noise and echo.

Requires precise timing for accurate decoding.

Can be enhanced using error correction techniques.
