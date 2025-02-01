# AWS CLI


The AWS Command Line Interface (AWS CLI) is an open-source tool that enables users to interact with AWS services via command-line commands. With minimal setup, it offers functionality similar to the AWS Management Console. Supporting Linux, macOS, and Windows, the AWS CLI provides a powerful way to manage AWS resources programmatically.

- [Download AWS CLI](#download-aws-cli)
- [Install AWS CLI](#install-aws-cli)
    - [Linux](#linux)
    - [macOS](#macos)
    - [Windows](#windows)
- [System Requirements](#system-requirements)
- [Usage](#usage)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)

## Download AWS CLI
AWS CLI 2.0.30 is the latest stable version

*   Release number: 2.0.30
*   Release date: Jan 7, 2025

| Platform | Type             | Download                                                                                                                                                                                                                             |
| -------- | ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Windows  | Standard Installer   | [64-bit version](*) [ARM64 version](*)                                                                                          |
|          | System Installer | [64-bit version](*) [ARM64 version](*)                                                                                        |
|          | .zip             | [64-bit version](*) [ARM64 version](*)                                                                                          |
| macOS    | .zip             | [Universal](*) [Intel Chip](*) [Apple Silicon](*) |
| Linux    | .tar.gz          | [64-bit version](*)                                                                                                                                                                 |
|          | .deb             | [64-bit version](*)                                                                                                                                                               |
|          | .rpm             | [64-bit version](*)              




## Install AWS CLI

### System Requirements

Before installing the AWS CLI, ensure that your system meets the following requirements:

- **Operating System**: The AWS CLI is supported on 64-bit versions of recent distributions of Linux, macOS versions 11 and later, and Microsoft-supported versions of 64-bit Windows.
- **Python**: Python 3.8 or later is required for building from source.
- **Admin Rights**: Admin rights are required to install software on Windows.

### Installation Instructions

#### Windows

To install the AWS CLI on Windows, follow these steps:

1. **Run the Installer**:
   You can run the installer by double-clicking the downloaded file or using the command line:
   ```cmd
   msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
   ```

2. **Verify the Installation**:
   Open the command prompt and check the version:
   ```cmd
   aws --version
   ```

#### Linux

To install the AWS CLI on Linux, follow these steps:

1. **Download the Installer**:
   Use the following command to download the AWS CLI installer:
   ```bash
   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
   ```

2. **Unzip the Installer**:
   Unzip the downloaded package:
   ```bash
   unzip awscliv2.zip
   ```

3. **Run the Install Program**:
   Execute the install program with the following command:
   ```bash
   sudo ./aws/install
   ```

4. **Verify the Installation**:
   Confirm the installation by checking the version:
   ```bash
   aws --version
   ```

5. **Update the AWS CLI**:
   To update your current installation, use:
   ```bash
   sudo ./aws/install --update
   ```

#### macOS

To install the AWS CLI on macOS, you can use the GUI installer or the command line:

1. **Download the Installer**:
   Download the macOS installer package:
   ```bash
   curl "https://awscli.amazonaws.com/AWSCLIV2.pkg" -o "AWSCLIV2.pkg"
   ```

2. **Run the Installer**:
   Run the downloaded file and follow the on-screen instructions. You can choose to install for all users or just the current user.

3. **Verify the Installation**:
   Open a terminal and run:
   ```bash
   aws --version
   ```
## System Requirements

- **Linux**: 64-bit versions of recent distributions (CentOS, Fedora, Ubuntu, Amazon Linux).
- **macOS**: Versions 11 and later.
- **Windows**: Microsoft-supported versions of 64-bit Windows.
- **Python**: Python 3.8 or later is required for building from source.

## Usage

Once installed, the AWS CLI allows you to manage AWS services directly from your command line. You can run commands to create, configure, and manage AWS resources. For example, to list your S3 buckets, you can use:
```bash
aws s3 ls
```

## Configuration

After installation, you need to configure the AWS CLI with your AWS credentials. You can do this by running:
```bash
aws configure
```
This command will prompt you for your AWS Access Key ID, Secret Access Key, default region name, and output format.
