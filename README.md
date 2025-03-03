# Nautilus MetaTrader 5 Adapter

This adapter allows for seamless integration between the Nautilus Trader and MetaTrader 5, providing capabilities for market data retrieval, order execution, and account management through the MetaTrader 5 Terminal API. It utilizes [metatrader5ext](https://github.com/quantspub/metatrader5ext) to enable the use of [MetaTrader5](https://pypi.org/project/MetaTrader5) on the Nautilus Trader.

## Installation

To install the MetaTrader 5 Adapter, follow these steps:

1. Clone the repository:

   ```sh
   git clone https://github.com/quantspub/nautilus_metatrader5.git
   ```

2. Navigate to the project directory:

   ```sh
   cd /nautilus_metatrader5
   ```

3. Pull the Docker image:

   ```sh
   docker pull docker.io/quantspub/metatrader5-terminal:latest
   ```

4. Install the required Python packages:
   ```sh
   poetry install
   ```

## Usage

To run the MetaTrader 5 Adapter, execute the following commands:

```bash
cd examples
```

```bash
cp .env.example .env
```

```bash
python connect_with_dockerized_terminal.py
```

**NOTE:** Make sure to configure the .env file properly before running the script or the docker image.

### Detailed Steps:

1. Ensure Docker is installed and running on your machine.
2. Clone the repository and navigate to the project directory.
3. Pull the Docker image for MetaTrader 5 Terminal.
4. Install the required Python packages using Poetry.
5. Navigate to the `examples` directory.
6. Copy the `.env.example` file to `.env` and configure it with your MetaTrader 5 credentials.
7. Run the `connect_with_dockerized_terminal.py` script to start the adapter.

## Project Structure

The project structure is organized as follows:

```
nautilus_metatrader5/
├── nautilus_metatrader5/
│   ├── __init__.py
│   ├── adapter.py
│   ├── client.py
│   └── ...
├── examples/
│   ├── connect_with_dockerized_terminal.py
│   ├── .env.example
│   └── ...
├── tests/
│   ├── test_adapter.py
│   └── ...
├── pyproject.toml
├── README.md
└── ...
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes.
4. Commit your changes (git commit -m 'Add some feature').
5. Push to the branch (git push origin feature-branch).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.LICENSE file for details.
