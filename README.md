# Weather Contract

## Overview
The Weather Functions contract is a Solidity smart contract designed to interact with Chainlink external adapters for retrieving weather data. The contract allows users to request weather information for a specific city, leveraging Chainlink's off-chain computation capabilities to fetch real-time data from external APIs.

## Features
- **Weather Data Retrieval:** Users can request weather information for a specific city by calling the `getTemperature` function and providing the city name as input.
- **Chainlink Integration:** Utilizes Chainlink's Functions external adapters to make HTTP requests and retrieve weather data from external APIs.
- **Event Logging:** Logs responses and errors for each weather data request, providing transparency and traceability.

## Contracts
- **WeatherFunctions.sol:** Main smart contract implementing the functionality for weather data retrieval.

## Usage
To interact with the contract, follow these steps:
1. Deploy the WeatherFunctions contract on the desired blockchain network.
2. Configure the Chainlink router address and subscription ID in the contract constructor.
3. Call the `getTemperature` function with the desired city name to request weather data.
4. Monitor the emitted `Response` event to retrieve the weather information and any associated errors.
5. Query the contract's state variables or use the provided getter functions to access weather data and request status.

## Deployment
- Network: Sepolia
- Chainlink Oracle: Weather (Address: 0xA9d587a00A31A52Ed70D6026794a8FC5E2F5dCb0)

## Security Considerations
- Ensure that the Chainlink router address and subscription ID are correctly set to interact with the desired Chainlink network.
- Implement access controls and authorization mechanisms to restrict weather data requests to authorized users if necessary.
- Thoroughly review and test the contract code to verify its correctness and security before deployment.

## License
This project is licensed under the terms of the MIT license. See the [LICENSE](LICENSE) file for details.

## Disclaimer
This contract is provided as an educational example and should be thoroughly tested and audited before use in production environments. Use at your own risk.
