# SOS Emergency App for Terminally Ill Patients

## Overview
The **SOS Emergency App** is a Streamlit-based application designed to help terminally ill patients send an emergency alert when they need urgent medical assistance. The app utilizes the **DeepSeek R1** model to generate an SOS message and sends an alert to emergency services via an API.

## Features
- **SOS Alert Button**: Instantly triggers an emergency alert.
- **AI-Generated SOS Message**: Uses the DeepSeek R1 model to create a distress message.
- **Emergency API Integration**: Sends alerts to a designated emergency service endpoint.
- **Secure API Communication**: Utilizes API keys stored securely in a `.env` file.

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- pip (Python package manager)
- Streamlit
- `requests` and `transformers` libraries

### Clone the Repository
```sh
git clone <repository-url>
cd sos-emergency-app
```

### Install Dependencies
```sh
pip install -r requirements.txt
```

### Set Up Environment Variables
Create a `.env` file in the project directory and add your API keys:
```sh
HUGGINGFACE_API_KEY=your_huggingface_api_key
EMERGENCY_API_ENDPOINT=your_emergency_api_endpoint
```

## Usage
Run the Streamlit app with the following command:
```sh
streamlit run app.py
```

## How It Works
1. Click the **SOS** button.
2. The app generates an emergency message using the **DeepSeek R1** model.
3. The generated message is sent to the emergency services API.
4. Users receive confirmation that help is on the way or an error message if the request fails.

## Dependencies
- `streamlit`
- `requests`
- `transformers`
- `dotenv`

## Contributing
Feel free to contribute to this project by submitting a pull request or reporting issues.

## License
This project is licensed under the MIT License.

## Contact
For any inquiries, reach out to [your contact information].

