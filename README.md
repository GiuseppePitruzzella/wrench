<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
<!--
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]
-->


<!-- PROJECT LOGO -->
<br />
<div align="center">

<h2 align="center">Wrench</h2>

  <p align="center">
Display text into your led matrix using a telegram bot  🤖
    <br />
    <br />
    <br />
    ·
    <a href="https://github.com/GiuseppePitruzzella/wrench/issues">Report Bug</a>
    ·
    <a href="https://github.com/GiuseppePitruzzella/wrench/issues">Request Feature</a>
  </p>
</div>



<!-- GETTING STARTED -->
## Getting Started

This project allows you to display horizontally scrolling text on two LED matrices using an ESP32, Wi-Fi, and a Telegram bot. It's perfect for remotely displaying customized messages through Telegram.

## Requirements

Before starting, ensure you have the following hardware and software components:
- 1 x ESP32
- 2 x LED Matrix (8x8 or 16x16)
- Jumper wires to connect the LED matrices to the ESP32
- Power supply for the ESP32
- Your Telegram Bot
- Your Telegram Chat ID

## Hardware Setup
1. Connect the two LED matrices together.
2. Connect the first LED matrix to the ESP32 according to the following scheme:

   | ESP32 Pin | LED Matrix Pin |
   | --------- | -------------- |
   | 5V        | VCC            |
   | GND       | GND            |
   | D23       | DIN            |
   | D22       | CLK            |
   | D21       | CS             |

3. Ensure stable and sufficient power supply for the ESP32 and the LED matrices.

## Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/GiuseppePitruzzella/wrench
   cd wrench
   ```

2. **Configure credentials and token**:
   ```cpp
   #define WIFI_SSID "your-wifi-ssid"
   #define WIFI_PASSWORD "your-wifi-password"
   #define BOT_TOKEN "your-bot-token"
   #define CHAT_ID "your-chat-id"
   ```

3. **Upload the code to the ESP32**:

<!-- USAGE EXAMPLES -->
## Usage

<!-- Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources. -->
1. **Power on the ESP32** and ensure it connects to the Wi-Fi network. You will see connection details in the Arduino IDE serial monitor.
2. **Interact with the Telegram bot**:
   - Open Telegram and find your bot.
   - Send a text message to the bot. The text will be displayed in scrolling mode on the two LED matrices.



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


<!-- LICENSE -->
## License
Distributed under the GNU GPLv3 License. See `LICENSE.txt` for more information.



<!-- CONTACT -->
## Contact

Project Link: [https://github.com/GiuseppePitruzzella/wrench](https://github.com/GiuseppePitruzzella/wrench)
