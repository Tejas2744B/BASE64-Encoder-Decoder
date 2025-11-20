
# ✍️ Base64 Encoder/Decoder Tool

This is a simple command-line utility for converting text strings to and from **Base64** format. Base64 is a crucial encoding scheme in cybersecurity, used primarily to safely transmit binary data (like images or encrypted keys) across systems that are designed to handle only text (like email or HTTP forms).

This project was developed as a solution for **Task 5: Base64 Encoder/Decoder**.

## ✨ Features

* **Bi-Directional Conversion:** Supports both encoding (Text to Base64) and decoding (Base64 to Text).
* **Standard Library Use:** Implemented using Python's built-in `base64` module, ensuring reliability and efficiency.
* **Robust Error Handling:** Gracefully handles invalid Base64 input, incorrect padding, and potential non-UTF-8 output during decoding.
* **Simple CLI:** Provides an easy-to-use, interactive command-line interface for function selection.
* **Edge Case Handling:** Ensures safe operation with empty input strings.

## ⚙️ Requirements & Installation

### Prerequisites

* Python 3.x (Uses standard library only)

### Setup

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/YourUsername/base64-tool.git](https://github.com/Tejas2744B/base64-tool.git)
    cd base64-tool
    ```

2.  **No external dependencies are required.**

## 💻 Usage

Run the script directly from your terminal:

```bash
python base64_tool.py
