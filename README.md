# CCD Backend

Backend server for the Cancer Cell Detection project using Flask and ONNX Runtime.

## Setup

1. Clone the repository
```bash
git clone https://github.com/Js0326/CCD-BACKEND.git
cd CCD-BACKEND
```

2. Download the model file
- Download the Swin Transformer model file (`swin_model.onnx`) from [Google Drive](your-drive-link)
- Place it in the root directory of the backend

3. Install dependencies
```bash
pip install -r requirements.txt
```

4. Run the server
```bash
python app.py
```

The server will start at `http://localhost:5000`

## Model File
The ONNX model file (`swin_model.onnx`) is not included in this repository due to size limitations. Please download it separately from the provided link and place it in the project root directory before running the server.

## API Endpoints

- `POST /upload` - Upload and analyze histopathological images
- `GET /results/<id>` - Get analysis results by ID

## Environment Variables
Create a `.env` file with:
```
FLASK_ENV=development
``` 