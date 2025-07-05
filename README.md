# AVCMT-PY: AI-Powered Commit Message Generator 🚀

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg) ![License](https://img.shields.io/badge/license-MIT-green.svg) ![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg) ![GitHub Releases](https://img.shields.io/badge/releases-latest-orange.svg)

Welcome to **AVCMT-PY**, your go-to tool for generating semantic Git commit messages automatically. This project leverages AI to streamline your workflow, ensuring your Python projects maintain high code quality and efficient release management. 

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Features

- **AI-Powered**: Utilize advanced algorithms to generate meaningful commit messages.
- **Fully Automated**: Set up your workflow to handle commit messages without manual input.
- **Semantic Release Style**: Follow best practices in versioning and release management.
- **CLI Tool**: Easy-to-use command-line interface tailored for Python projects.
- **Integration with GitHub Actions**: Seamlessly incorporate into your CI/CD pipeline.
- **Open Source**: Contribute and collaborate with a community of developers.
- **Pre-commit Hooks**: Ensure commit messages meet standards before they are finalized.

## Installation

To get started with AVCMT-PY, you need to have Python installed on your machine. Follow these steps:

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Jhdkb/avcmt-py.git
   cd avcmt-py
   ```

2. **Install dependencies**:

   Use pip to install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the tool**:

   You can start using AVCMT-PY right away:

   ```bash
   python avcmt.py
   ```

## Usage

Using AVCMT-PY is straightforward. The command-line interface allows you to generate commit messages with a simple command. 

### Basic Command

To generate a commit message, simply run:

```bash
avcmt generate
```

This command will provide you with a suggested commit message based on the changes you've made.

### Customization

You can customize the output by providing flags. For example:

```bash
avcmt generate --type feat --scope ui --description "Add button styles"
```

This command will generate a commit message like:

```
feat(ui): Add button styles
```

### Integration with GitHub Actions

To automate the commit message generation in your CI/CD pipeline, you can add the following snippet to your GitHub Actions workflow file:

```yaml
jobs:
  commit-message:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout code
        uses: actions/checkout@v2
      
      - name: Generate Commit Message
        run: |
          python avcmt.py generate
```

This setup will ensure that every commit in your repository follows the semantic release style.

## Contributing

We welcome contributions to AVCMT-PY! If you would like to contribute, please follow these steps:

1. **Fork the repository**.
2. **Create a new branch**:
   ```bash
   git checkout -b feature/YourFeature
   ```
3. **Make your changes** and commit them:
   ```bash
   git commit -m "Add your commit message"
   ```
4. **Push to your branch**:
   ```bash
   git push origin feature/YourFeature
   ```
5. **Create a Pull Request**.

Please ensure that your code adheres to our coding standards and includes appropriate tests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Links

For more information, visit the [Releases](https://github.com/Jhdkb/avcmt-py/releases) section to download the latest version and execute it on your machine. You can also check out the releases for updates and new features.

If you have any questions or need assistance, feel free to reach out through issues or discussions in the repository.

## Conclusion

AVCMT-PY is designed to enhance your development experience by automating commit message generation and ensuring code quality. By integrating this tool into your workflow, you can save time and focus on what truly matters: writing great code.

Explore the power of AVCMT-PY today and transform the way you manage your Git commits!