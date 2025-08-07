## 📚 Personal Library Barcode Scanner

### Overview
This project is a Python-based barcode scanner designed to help organize personal book collections by scanning ISBN barcodes and retrieving book information from the Google Books API. The data is automatically saved into an Excel file for easy tracking and management.

> 📝 **Note:** I developed this tool while organizing my own library to separate books I’ve read from those I haven’t, and to keep track of the ones I own but haven’t yet explored.


### 🔧 Features
- 📖 Automatically fetches book title and author using the ISBN
- 📊 Saves scanned data to an Excel file (`books.xlsx`)
- ✅ Prevents duplicate entries by checking previously scanned ISBNs
- 🎯 Real-time barcode detection using your webcam
- 💬 Displays a confirmation message when a book is successfully saved


### 🛠️ Technologies Used
- `Python`
- `OpenCV` for webcam access and frame rendering
- `pyzbar` for barcode decoding
- `requests` for API communication
- `openpyxl` for Excel file handling


### 🚀 How to Run
1. Make sure you have a webcam connected.
2. Install the required libraries:
   ```bash
   pip install opencv-python pyzbar requests openpyxl
   ```
3. Run the script:
   ```bash
   python barcode_scanner.py
   ```
4. Point your book’s barcode toward the camera. If the book is found via Google Books API, its details will be saved to `books.xlsx`.

5. Press `q` to exit the scanner.


### 📁 Output
The Excel file will contain:
| ISBN | Title | Author |
|------|-------|--------|
| 9781234567897 | Example Book | John Doe |


### 💡 Use Cases
- Organizing personal libraries
- Tracking unread vs. read books
- Creating a digital inventory of physical books


### 🧠 Future Improvements
- Add GUI for easier interaction
- Support for multiple languages
- Export to other formats (CSV, PDF)
- Integration with Goodreads or other book platforms

⚠️ The Excel file (books.xlsx) is automatically generated when you run the script. No need to create it manually.

