
# Dino Run Game Automation

This project is an automation script for playing the popular offline game "Dino Run" in the Google Chrome browser. The game is a simple endless runner game where a dinosaur character runs and jumps over obstacles. This script uses Python and various libraries like OpenCV, NumPy, and pyautogui to automate gameplay and achieve high scores.

## Prerequisites

Before running the script, make sure you have the following prerequisites:

1. **Python**: Make sure you have Python 3.x installed on your system.

2. **Required Python Libraries**:
   - `cv2` (OpenCV): Used for image processing and template matching.
   - `numpy`: Used for numerical operations.
   - `matplotlib.pyplot`: Used for displaying images (optional).
   - `PIL.ImageGrab`: Used for taking screenshots.
   - `pyautogui`: Used for simulating keyboard inputs.

3. **Google Chrome**: You need to have Google Chrome installed on your system, as the Dino Run game is typically played in the Chrome browser.

## Getting Started

1. Clone or download this repository to your local machine.

2. Install the required Python libraries by running the following command:

   ```
   pip install opencv-python numpy matplotlib pillow pyautogui
   ```

3. Open Google Chrome and navigate to the Dino Run game. You can access it by typing `chrome://dino/` in the address bar and pressing Enter.

4. Adjust the game screen dimensions and other parameters as needed in the script. For example, you may need to modify the `grab_screen` function to capture the game screen accurately.

## Running the Script

Run the script by executing the following command:

```
python dino_run.py
```

- The script will start by checking for the presence of the Dino character on the screen. Once detected, it will press the spacebar to start the game.

- As the game progresses, the script will adjust the jump timing based on the speed of the game. It will also detect and jump over obstacles (cacti and birds) to keep the game going.

- You can stop the script at any time by pressing the 'q' key.

## Customization

You can customize various parameters in the script to improve performance or adapt it to different screen sizes and game variations:

- Adjust the template matching method and threshold values in the `match` function of the `Dino_Game` class to improve object detection.

- Modify the `distanceThreshold`, `speed`, and `acceleration` variables to fine-tune the jumping behavior according to the game's speed.

- Change the list of `Enemies` by adding or removing elements to detect different types of obstacles in the game.

- If you are using a different browser or screen resolution, adjust the screen capture dimensions in the `grab_screen` function.

## Troubleshooting

If the script is not working as expected, consider the following troubleshooting steps:

- Ensure that you have the required Python libraries installed.

- Check the screen dimensions and template matching parameters in the script to make sure they match your setup.

- Debugging output, such as printing the detected objects and their positions, can help identify issues.

- If the game layout or resolution changes, you may need to adapt the script accordingly.

## Disclaimer

This script is created for educational and entertainment purposes and should be used responsibly. Automated gameplay may violate the terms of service of the game or the platform it is hosted on. Be sure to play games in a manner that complies with all relevant policies and agreements.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to adapt and improve this README as needed for your project documentation. Additionally, consider adding more details about the script's performance, limitations, and any further enhancements you may plan to implement in the future.
