# Introduction

Software for vibration monitoring and anomalies based on patterns:
- Intel Xeon processors

## Functions
- Level 1 XEON: The sensor vibration detection and records a video. The video is streamed.
- Level 2 XEON: After recording video, a vibration anomaly detection model checks if a pattern is present in the video. If yes, the video and a screenshot are sent .
- When a problem occurs, a notification is send to a mobile device.

## Architecture
### Intel Xeon
![Architecture 1](https://github.com/hexagontechinc/WIP/blob/master/DOCS_ANOMALY/Arch.001.jpeg)

## Note on network latency:

In this application, the performance is limited by the bandwidth of your local network (not to be confused with convolutional neural network - CNN). All the activity can be challenging for a router to keep up with. 5 GHz(802.11 ac in marketing speak) bands are recommended.

## Development

This software was written for monitoring the vibration of rotating equipment. The system related to XEON Level 1 has been in use for about two years and there are failsafes built in to prevent issues such as loss of network connection and memory overflow. Since my requirements are well-served with the current version, more features will be added only if requests are made by raising issues.  Level 2 XEON functionality is proof of concept stage.
Model is retrained with new data collected on a monthly basis.

**Pull requests which add useful features or failsafes are more than welcome!**
