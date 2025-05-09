# SMStoWebhook

An Android Kotlin application that tracks SMS transactions and forwards them to Discord channels with customizable notifications.
(Made for Private Use Only, You cn use this code)

## Overview

SMStoWebhook monitors your device for incoming SMS messages, particularly focusing on transaction notifications from banking services and other financial applications. When it detects relevant messages, the app automatically forwards them to a specified Discord channel through webhooks, optionally including user pings for immediate notification.

## Features

- **SMS Monitoring**: Automatically detects and processes incoming SMS messages
- **Transaction Filtering**: Identifies transaction-related messages from banks and financial services
- **Discord Integration**: Forwards messages to Discord channels via webhooks
- **Custom Notifications**: Ability to ping specific users or roles when messages are forwarded
- **Customizable Settings**: Configure which message types to monitor and how to format Discord notifications

## Setup Requirements

- Android device running Android 8.0 (Oreo) or higher
- Permission to read SMS messages
- Discord webhook URL from a channel where you have webhook creation permissions

## Installation

1. Download the latest APK from the [Releases](https://github.com/lakshrajj/SMStoWebhook/releases) section
2. Install the APK on your Android device
3. Grant the necessary permissions for SMS access when prompted

## Configuration

### Setting up a Discord Webhook

1. Open Discord and navigate to the server and channel where you want to receive notifications
2. Click the gear icon next to the channel name to access channel settings
3. Select "Integrations" from the left sidebar
4. Click "Create Webhook"
5. Customize the webhook name and avatar if desired
6. Copy the webhook URL

### Configuring the App

1. Open the SMStoWebhook app
2. Paste your Discord webhook URL in the designated field
3. Configure notification settings:
   - Select which SMS senders to monitor
   - Set up custom filters for transaction detection
   - Configure user IDs or role IDs to ping in notifications
4. Save your settings and enable the service

## Usage

Once properly configured, the app will run in the background and:

1. Monitor incoming SMS messages
2. Filter for transaction-related content
3. Format and send relevant messages to your Discord channel
4. Include pings if configured to do so

The app will also display a notification to confirm when messages have been successfully forwarded.

## Permissions

This app requires the following permissions:

- `READ_SMS`: To monitor incoming SMS messages
- `RECEIVE_SMS`: To be notified when new messages arrive
- `INTERNET`: To communicate with Discord webhooks
- `FOREGROUND_SERVICE`: To run reliably in the background

## Privacy Notice

This application only forwards the SMS messages you explicitly configure it to monitor. No data is stored on external servers, and communication occurs directly between your device and Discord's webhook API using encrypted HTTPS connections.

## Contributing

Contributions to SMStoWebhook are welcome! If you'd like to contribute:

1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the Discord API for providing webhook functionality
- Special thanks to all contributors who have helped improve this application
