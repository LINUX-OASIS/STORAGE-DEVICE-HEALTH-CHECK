# 💾 Storage Device Health Check 🩺

![GitHub repo size](https://img.shields.io/github/repo-size/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK?style=for-the-badge&logo=github&color=34A853)
![GitHub language count](https://img.shields.io/github/languages/count/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK?style=for-the-badge&logo=github&color=34A853)
![GitHub top language](https://img.shields.io/github/languages/top/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK?style=for-the-badge&logo=shell&color=34A853)
![License](https://img.shields.io/github/license/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK?style=for-the-badge&logo=gpl&color=34A853)
![GitHub issues](https://img.shields.io/github/issues/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK?style=for-the-badge&logo=github&color=yellow)


A simple yet powerful Bash script that provides a Text-based User Interface (TUI) to quickly check the S.M.A.R.T. health status of your NVMe and SATA/SCSI storage devices.

---

## ✨ Features

*   **Interactive TUI**: Uses `whiptail` to present a clean, interactive menu for easy device selection.
*   **Automatic Device Detection**: Scans and lists available NVMe (`/dev/nvme*`) and SATA/SCSI (`/dev/sd*`) drives.
*   **Dependency Auto-Installer**: Checks for required tools (`nvme-cli`, `smartmontools`) and attempts to install them if they are missing.
*   **Comprehensive Reports**: Generates detailed health reports using `nvme smart-log` and `smartctl`.
*   **Quick Summary View**: Displays a concise summary of the most critical health attributes in a dialog box.
*   **Report Logging**: Saves the full and summary reports to the `/tmp` directory for later review.
*   **Colorful Output**: Uses `tput` and `whiptail` themes for a more readable and visually appealing experience in the terminal.

---

## 🖥️ Compatibility

This script is designed to work on Debian-based Linux distributions that use the `apt` package manager. It has been tested and is known to be compatible with:

*   !Debian
*   !Ubuntu
*   !Linux Mint
*   Other Debian/Ubuntu derivatives.

---

## 🛠️ Dependencies

The script requires the following command-line tools to function correctly:

*   `nvme-cli`: For interacting with NVMe storage devices.
*   `smartmontools`: For querying S.M.A.R.T. data from SATA/SCSI devices.
*   `whiptail`: For displaying dialog boxes from shell scripts (typically pre-installed on most Debian-based systems).

> **Note**
> The script will automatically check if `nvme-cli` and `smartmontools` are installed. If they are not found, it will attempt to install them using `sudo apt install -y`. You may be prompted for your password.

---

## 🚀 Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK.git
    cd STORAGE-DEVICE-HEALTH-CHECK
    ```

2.  **Make the script executable:**
    ```bash
    chmod +x custom-STORAGE-DEVICE-HEALTH-CHECK.sh
    ```

3.  **Run the script:**
    > Administrative privileges are required to query hardware information.
    ```bash
    sudo ./custom-STORAGE-DEVICE-HEALTH-CHECK.sh
    ```

---

## 💬 Contributing

Pull requests, issues, and suggestions are warmly welcomed! We believe in the power of community collaboration to make this tool even better.

For major changes, please open an issue first to discuss what you would like to change. Please see **CONTRIBUTING.md** for detailed guidelines.

---

## 🌐 Links

| Type                                                                                                             | Link                                                                                                                            |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 🐛 **Report an Issue**                                                                                           | github.com/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK/issues     |
| 📥 **Submit a Pull Request**                                                                                     | github.com/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK/pulls      |
| 📦 **Releases**                                                                                                  | github.com/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK/releases |
| 📖 **Project Wiki**                                                                                              | github.com/LINUX-OASIS/STORAGE-DEVICE-HEALTH-CHECK/wiki         |

---

## 🧙‍♂️ Maintainer

This project is maintained by:

[!LINUX-OASIS](https://github.com/LINUX-OASIS)

---

## 📜 License

This project is licensed under the **GNU General Public License v3.0**.

See the LICENSE file for more details.

