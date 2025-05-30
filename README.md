
# Windows Activation via KMS Script - Jupyter Notebook

## Overview

This Jupyter Notebook provides a step-by-step guide to activating a Windows operating system using Key Management Service (KMS) commands. It is intended for educational and testing purposes only, demonstrating how Windows can be activated using command-line tools.

> ⚠️ **Disclaimer**: This notebook is for **educational purposes** only. Unauthorized use of activation methods may violate Microsoft’s Terms of Service. Always ensure you are in compliance with licensing terms.

---

## Features

- Detects current Windows edition.
- Uninstalls any existing product keys.
- Installs a valid KMS client key.
- Connects to a KMS server.
- Activates the Windows installation via command-line tools (e.g., `slmgr.vbs`).
- Verifies activation status.

---

## Requirements

- Windows OS (preferably Pro, Enterprise, or Education editions).
- Python (optional; only used to organize command execution).
- Administrator privileges on the system.
- Jupyter Notebook installed if running interactively.

---

## How to Use

1. **Open the notebook** in Jupyter Notebook or JupyterLab.
2. **Run each cell** step by step.
3. The script will:
    - Install a default KMS client key (based on your Windows version).
    - Set a KMS server.
    - Attempt activation.
    - Display the result and activation status.

---

## Sample KMS Commands Used

```bash
slmgr /upk
slmgr /ipk <KMS_CLIENT_KEY>
slmgr /skms kms.example.com
slmgr /ato
slmgr /xpr
```

---

## Notes

- You must be connected to the internet or a valid KMS host network for activation to work.
- This notebook assumes the user is familiar with the risks of modifying Windows activation settings.

---

## License

This project is distributed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments

- Microsoft documentation on KMS client setup.
- Educational tutorials and community forums that detail command-line activation.
