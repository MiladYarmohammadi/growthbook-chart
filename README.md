# Growthbook Chart

This project is used to deploy growthbook to manage and visualize growth metrics using a Helm chart.

## Table of Contents

- [Installation and Usage](#installation-and-usage)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)

## Installation and Usage

To upgrade the Helm chart, run:

```bash
helm upgrade --install growthbook -n growthbook --create-namespace ./path-to-your-chart -f values.yaml
```

To uninstall the Helm chart, run:

```bash
helm uninstall growthbook -n growthbook
```

## Configuration

Configuration options can be set in the `values.yaml` file. Below is an example configuration:

```yaml
apiEndpoint: 'https://api.example.com'
apiKey: 'your-api-key'
chartOptions:
  type: 'line'
  color: '#00ff00'
```

## Contributing

We welcome contributions! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
