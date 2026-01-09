CircuitGuard is an AI-based PCB defect detection system powered by deep learning, utilizing the YOLOv11m model. It uses a custom-trained YOLO model and provides an interactive Streamlit interface for uploading images, visualizing defect locations, viewing defect summaries, and exporting reports.
#Key Features

Automatic PCB defect detection from uploaded images
Exact defect location with bounding box visualizations
Defect summary dashboard (bar graph showing count per defect )
Model performance indicators (mAP, precision, recall)
Downloadable final results in zip file format containing: CSV having the exact defect location Annotated image (image with drawn bounding boxes)
100% Streamlit-based — no external backend required
#Tech Stack Component Technology Model YOLO (Ultralytics) Language Python 3.11.6 Framework Streamlit Deployment Local/Cloud via Streamlit

#Project Structure

CircuitGuard/ │ ├── app.py # Main Streamlit app (UI + inference) ├── predict.py # Script for running predictions ├── best.pt # Trained YOLO model weights ├── requirements.txt # dependencies for the website ├── packages.txt # Extra packages list ├── runtime.txt # Python runtime version (for deployment 3.11) ├── README.md # Project documentation │ ├── .devcontainer/ │ └── devcontainer.json # Dev container config ├── .gitattributes # Git attributes configuration

#Model Performance CircuitGuard was trained on a custom PCB defect dataset with an 80:20 train-test split. CircuitGuard accuracy

🔎 High precision and recall show strong defect detection reliability with minimal false positives/negatives.
#How to Use Run the app locally

Upload an image (drag-and-drop or file picker)

View annotated output + defect summary

Download report and annotated image (optional)

#Sample outputs:

Annotated images CircuitGuard accuracy CircuitGuard accuracy

CSV file having exact defect location:
CircuitGuard accuracy
#Screenshots of the website CircuitGuard accuracy CircuitGuard accuracy CircuitGuard accuracy CircuitGuard accuracy

#Acknowledgements

Ultralytics YOLO
Streamlit
PCB defect datasets used for research and training

