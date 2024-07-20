# Warframe Market Prime Trash Buyer Go CLI

## Overview

The **Warframe Market Prime Trash Buyer CLI** is a command-line interface tool designed for Warframe players to manage profitable orders from the Warframe Market API. This application acts as a wrapper around the [Warframe Market Prime Trash Buyer Go Library](https://github.com/FreePhoenix888/warframe-market-prime-trash-buyer-go-lib), which provides the core functionality for identifying and handling profitable orders with a high platinum-to-ducats ratio.

## Features

- **Fetch Profitable Orders:** Retrieves orders from the Warframe Market API with a high platinum-to-ducats ratio.
- **Generate Purchase Messages:** Creates messages based on profitable orders for easy copying.
- **Clipboard Integration:** Copy purchase messages directly to the clipboard using the `clipboard` package.
- **Dynamic Filtering:** Excludes previously copied messages to avoid redundancy.
- **Real-time Updates:** Provides real-time updates and error handling with a user-friendly interface.

## Installation

Ensure you have Go installed on your system. You can install the CLI application using the following command:

```bash
go install github.com/freephoenix888/warframe-market-prime-trash-buyer-go-cli@latest
```

This will install the application and make it available in your `GOPATH/bin` directory. Ensure this directory is included in your system's `PATH` environment variable.

## Usage

Run the CLI application from your terminal:

```bash
warframe-market-prime-trash-buyer-go-cli
```

### Commands

- **`exit`**: Exit the application.
- **`regen`**: Regenerate the list of profitable orders and refresh the available messages.
- **Enter Message Number**: Copy the selected message to the clipboard by entering its corresponding number.

### Example Workflow

1. The application starts and fetches profitable orders based on the platinum-to-ducats ratio.
2. If no profitable orders are found or an error occurs, you will be prompted to type `regen` to fetch new orders or `exit` to quit.
3. After generating messages, a list of available messages is displayed.
4. Enter the number of a message to copy it to the clipboard or use `regen` to refresh the list of messages.

## Configuration

The application does not require any additional configuration. It uses environment variables to manage log levels and other settings. Ensure you have set the appropriate environment variables for logging if necessary.

## Contributing

Contributions are welcome! If you have suggestions or improvements, please submit an issue or a pull request on GitHub. For more details on contributing, please refer to the [CONTRIBUTING.md](CONTRIBUTING.md) file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please reach out via [GitHub Issues](https://github.com/freephoenix888/warframe-market-prime-trash-buyer-go-cli/issues).

