# Deepfake Detection Project

Welcome to the Deepfake Detection project repository! This project utilizes ResNext50 and LSTM models together for deepfake detection. The application's frontend is built using Streamlit, providing a user-friendly interface for detecting deepfakes.

## Getting Started

To get started with this project, follow these steps:

1. **Clone the Repository**: Begin by cloning this repository to your local machine using the following command:

    ```
    git clone [https://github.com/AnshumanGiramkar/deepfake-video-detection-ML.git](https://github.com/AnshumanGiramkar/deepfake-video-detection-ML.git)
    ```

2. **Install Requirements**: Create a Python virtual environment and install all project dependencies. You can do this by running the following commands:

    ```
    cd deepfake-detection
    python -m venv venv
    source venv/bin/activate (for Unix/MacOS)
    venv\Scripts\activate (for Windows)
    pip install -r requirements.txt
    ```

    If you encounter an error during the installation due to the unavailability of the `dlib` library, follow the steps below:

    - Delete any existing virtual environment and `requirements.txt` file created for this project.
    - Ensure that your Python version is 3.11 or higher.
    - After cloning the repository, move the `dlib-19.24.1-cp311-cp311-win_amd64.whl` file obtained in the `build-tools` folder to the `C:/Downloads` folder.
    - Open the Command Prompt (CMD) or PowerShell in the `C:/Downloads` folder.
    - Run the following command to install `dlib`:

        ```
        python -m pip install "dlib-19.24.1-cp311-cp311-win_amd64.whl"
        ```

    -**Note**: You can also download the dlib file from [DLIB_File](https://github.com/Murtaza-Saeed/dlib). Check your windows version, processor also while downloading it. You can refer this video for the same [DLIB_Installation](https://www.youtube.com/watch?v=9zeb902f98s)


3. **Run the Streamlit App**: Once all requirements are installed successfully, you can run the Streamlit app using the following command:

    ```
    streamlit run app.py
    ```

    This command will start the Streamlit server, and you can access the deepfake detection application by navigating to the provided URL in your web browser.

## Project Structure

Here's a brief overview of the project structure:

- **app.py**: This file contains the Streamlit application code for the frontend.
- **model.py**: This directory contains the ResNext50 and LSTM models implemented by us for deepfake detection.
- **weighted/**: This directory contains the `best-checkpoint-model.pt` required to leverage the pretrained weights directly to your streamlit app.
- **requirements.txt**: This file lists all the Python dependencies required for the project.
- **uploaded_videos**: You can try deepfake detection on the video from this directory. Even when you put your own video file for processing, it get's uploaded here.

## Contributing

Contributions to this project are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further assistance!
