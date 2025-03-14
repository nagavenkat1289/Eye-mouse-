# Eye Mouse Control Application

This project is an Eye Mouse Control Application that uses OpenCV, Mediapipe, and PyAutoGUI to control the mouse pointer with eye movements. The application is built with Flask to provide a web interface.

## Features

- Control mouse pointer using eye movements.
- Left click and right click using eye gestures.
- Real-time face mesh detection with Mediapipe.
- Adjustable camera scaling and cropping.

## Requirements

- Python 3.6+
- OpenCV
- Mediapipe
- PyAutoGUI
- Flask

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/eye-mouse-control.git
    cd eye-mouse-control
    ```

2. Create and activate a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Run the Flask application:

    ```bash
    python app.py
    ```

2. Open a web browser and navigate to `http://127.0.0.1:5000/` to access the interface.

3. Click on "Run App" to start the Eye Mouse Control.

## File Structure

- `app.py`: Main application file containing the Flask app and the eye mouse control logic.
- `templates/index.html`: HTML template for the web interface.
- `requirements.txt`: List of required Python packages.

## How It Works

1. The application uses OpenCV to capture video frames from the webcam.
2. Mediapipe's Face Mesh solution is used to detect facial landmarks in real-time.
3. The application processes the landmarks to control the mouse pointer using PyAutoGUI.
4. Eye gestures are detected to perform left and right-click actions.

## Troubleshooting

- **Webcam not detected**: Ensure that your webcam is properly connected and recognized by your operating system.
- **Application not starting**: Check for any error messages in the terminal and ensure that all required packages are installed.
- **Mouse pointer not moving**: Make sure that the face is well-lit and clearly visible to the webcam.

## Customization

- **Adjusting Sensitivity**: You can adjust the sensitivity of the eye movement detection by modifying the threshold values in the `process_landmarks` function.
- **Changing Camera Scale**: The `scale` variable can be adjusted to change the cropping size of the camera input.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [OpenCV](https://opencv.org/)
- [Mediapipe](https://mediapipe.dev/)
- [PyAutoGUI](https://pyautogui.readthedocs.io/)
- [Flask](https://flask.palletsprojects.com/)

## Contributing

Contributions are welcome! Please create an issue or submit a pull request for any improvements or bug fixes.

## Contact

For any questions or suggestions, feel free to reach out to [nagavenkat1289@gmail.com](nagavenkat1289@gmail.com).
