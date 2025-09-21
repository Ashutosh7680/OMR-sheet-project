# OMR-sheet-project
Here’s a **README.md** file you can directly upload to GitHub for your OMR Sheet Scanner project:

---

# OMR Sheet Scanner 📝

This project is an **Optical Mark Recognition (OMR) Sheet Scanner** built using **Python** and **OpenCV**.
It automatically detects the OMR answer sheet, applies perspective correction, identifies marked bubbles, compares them against an answer key, and calculates the final score.

---

## 🚀 Features

* Detects the OMR sheet automatically from an image.
* Applies perspective transform to flatten the sheet (bird’s-eye view).
* Identifies bubbles using contour detection.
* Compares answers with the predefined **Answer Key**.
* Outputs the **final score** of the student.

---

## 📂 Project Structure

```
.
├── omr_scanner.py     # Main Python script (your provided code)
├── Img5.jpeg          # Default sample image of OMR sheet (replace with your image)
├── README.md          # Project documentation
```

---

## ⚙️ Requirements

Make sure you have Python 3.x installed.
Install the required dependencies:

```bash
pip install opencv-python imutils numpy
```

---

## ▶️ Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/omr-scanner.git
   cd omr-scanner
   ```

2. Run the script with a default image (`Img5.jpeg`):

   ```bash
   python omr_scanner.py
   ```

3. Or run with your own OMR sheet image:

   ```bash
   python omr_scanner.py path_to_your_image.jpg
   ```

---

## 🛠️ Configuration

* **Answer Key** is defined inside the script as a Python dictionary:

```python
ANSWER_KEY = {
    0: 2,  # Question 1: C
    1: 1,  # Question 2: B
    2: 4,  # Question 3: E
    3: 0,  # Question 4: A
    4: 3,  # Question 5: D
}
```

👉 Update it to include all your questions and correct answers.

* **Marked bubble detection threshold** can be adjusted:

```python
if marked_pixels > 400:  # Increase/decrease depending on image clarity
    marked_bubble = j
```

---

## 📊 Output

The program prints the total score in the terminal:

```
Total Score: 4 out of 5
```

---

## 📸 Example Workflow

1. Detect OMR sheet from photo.
2. Apply perspective transform.
3. Extract and threshold bubbles.
4. Compare with Answer Key.
5. Display score.

---

## 🔮 Future Improvements

* Support for multiple-choice marking detection.
* Export results to CSV/Excel.
* GUI or Web-based interface for uploading sheets.
* Automatic answer key generation from template.

---

## 📜 License

This project is licensed under the MIT License - feel free to use and modify it.

---

Do you want me to also **add sample screenshots (like detection, thresholding, final warped image)** in the README for GitHub, or keep it only text-based?
