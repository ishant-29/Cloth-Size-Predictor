# Smart Clothing Size Predictor

An AI-powered web application that predicts clothing sizes based on user measurements and preferences.

## Features

- AI-powered size prediction
- Support for multiple brands (Adidas, H&M, Nike, Uniqlo, Zara)
- Support for multiple item types (Dress, Jacket, Jeans, Shirt, T-Shirt)
- Modern, responsive UI with animations
- Real-time form validation and progress tracking


## File Structure
```
Size_predictor/
├── main.py              # Flask application
├── wsgi.py              # WSGI configuration for PythonAnywhere
├── requirements.txt     # Python dependencies
├── model.pkl           # Trained ML model
├── brand_encoder.pkl   # Brand label encoder
├── item_encoder.pkl    # Item type encoder
├── scaler.pkl          # Feature scaler
├── selector.pkl        # Feature selector
├── Cloth_dataset.csv   # Training dataset
├── static/             # Static files (CSS, JS)
│   ├── css/
│   │   └── style.css
│   └── js/
│       └── script.js
└── templates/          # HTML templates
    ├── index.html
    └── prediction_result.html
```

## Troubleshooting

### Common Issues:

1. **Import Errors**: Make sure all `.pkl` files are in the same directory as `main.py`

2. **Static Files Not Loading**: Check that static file paths are correctly configured in PythonAnywhere

3. **Model Loading Errors**: Ensure all model files are uploaded and have correct permissions

4. **500 Internal Server Error**: Check the error logs in PythonAnywhere's "Web" tab

### Error Logs:
- Go to "Web" tab → "Error log" to see detailed error messages
- Check "Server log" for additional debugging information

## Local Development

To run locally:
```bash
pip install -r requirements.txt
python main.py
```

The app will be available at `http://localhost:5000`

## Technologies Used

- **Backend**: Flask, Python
- **Machine Learning**: scikit-learn, joblib
- **Frontend**: HTML5, CSS3, JavaScript
- **UI/UX**: Custom CSS animations, responsive design
- **Deployment**: PythonAnywhere 
