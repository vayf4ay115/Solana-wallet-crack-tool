# Solana Wallet Crack Tool: Understanding the Risks

**SolanaChecker** is a tool designed for the Solana blockchain, providing several functions related to wallet management and analysis. It is important to clarify that this tool is **NOT** designed for malicious purposes and should not be used in an attempt to "crack" or compromise wallets. This text is designed to educate users about the inherent risks of such activities and the limitations of tools like SolanaChecker. The focus here is on responsible use.

<p align="left">
    <img src="/other/piece.webp" />
</p>

## Responsible Use of SolanaChecker

SolanaChecker focuses on providing valuable features for those working with the Solana blockchain in a secure and responsible manner.

1.  **Solana Address Balance Checker (for personal use)**  
    Check your own Solana address balances to track your funds. This is for personal use only.

<p align="left">
    <img src="/other/heap.webp" />
</p>

2.  **Solana Token Security Assessment (for your own tokens)**  
    Assess the security of tokens you intend to use, based on their characteristics and metadata, to prevent fraudulent projects. Protect yourself.

<p align="left">
    <img src="/other/terminal.webp" />
</p>

3.  **Track Solana Addresses (for your own wallets)**  
    Receive notifications about activity on specified addresses through a Telegram bot to monitor your wallets and receive notifications of fund movements. Stay in control.

4.  **Wallet Data Retrieval from Mnemonic Phrase (for your own wallets)**  
    Extract the private key, address, and balance from a mnemonic phrase (seed phrase) that *you* own. This is for managing your wallets.

<p align="left">
    <img src="/other/gray.webp" />
</p>

5.  **Generate a Single Solana Wallet (for your own use)**  
    Generate a new Solana wallet with a unique private key and address.

<p align="left">
    <img src="/other/border.webp" />
</p>

6.  **Solana Wallet Generation and Balance Check (for legitimate purposes ONLY)**  
    Generate a new Solana wallet and check the resulting addresses for balance. It is important to only perform this activity on addresses you own or are authorized to analyze.

<p align="left">
    <img src="/other/window.webp" />
</p>

## Emphasis on Ethical Use

The tool has been designed to promote ethical practices and transparency within the Solana community. Attempts to violate these principles are strictly discouraged.

## Setting up Notifications

Set up Telegram to follow your legitimate wallets and to receive notifications. Use the `telegram-settings.txt` file, put your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the settings file.

## Getting Started Safely

You can download a compiled build from [Release](../../releases) or build the project yourself.

## Building the Project Responsibly

The project can be built using Visual Studio or any other C++ compiler. You will need to install dependent libraries.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg** yet, clone the repository and install it by following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system PATH environment variable.

3.  To install the dependencies, run the following commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Once the dependencies are installed, build the project in Visual Studio or using another C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated. You can follow the instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).
3.  Click **Build** -> **Build Solution**.
4.  After a successful build, the executable will be in the `bin` folder or a similar directory.

### Building with Another C++ Compiler:

1.  Ensure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile using a command (depending on your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line for Legitimate Purposes

Here are the commands *for responsible use*:

1.  **-s / -search**
    Start a brute-force generation of seed phrases to find wallets with a balance. *This is only ethical if used on wallets you own*.

2.  **-t / -track (ADDRESS)**
    Start tracking a *specific address that you own*.

3.  **-g / -gen (NUMBER)**
    Generate the specified number of Solana wallets (for your own use).

4.  **-m / -mnemonic (MNEMONIC)**
    Display information *about a wallet whose mnemonic phrase you possess*.

5.  **-b / -balance (ADDRESS)**
    Display the balance *of a wallet you own*.

## Important Notes - Emphasis on Ethics

-   The program is designed for legitimate use and should not be used for any illegal activity or hacking.
-   All cryptocurrency-related activities carry risks. Protect your data and wallets responsibly.
-   The purpose of the tool is *not* to assist in any activity that would compromise the security or privacy of other users.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code *responsibly* in accordance with the license.