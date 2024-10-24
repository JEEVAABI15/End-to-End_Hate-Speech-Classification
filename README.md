# Hate-Speech-Classification

# Gcloud cli
https://dl.google.com/dl/cloudsdk/channels/rapid/GoogleCloudSDKInstaller.exe

# Project Overview: Structured Pipeline for Data Ingestion, Model Training, and Deployment

This project focuses on creating a structured pipeline for **data ingestion**, **model training**, and **deployment**, utilizing **Google Cloud Platform (GCP)** and **Docker** to ensure efficient processing and scalability.

## 📌 Highlights

- **📦 Data Ingestion**: Data ingestion from GCP bucket serves as the foundation for the project, enabling the pipeline to initialize.
- **🗃️ Artifacts Directory**: Unzipped data is stored in an `artifacts/` directory for further processing.
- **⚙️ Modular Pipeline Structure**: The pipeline's structure promotes modularity, maintainability, and ease of debugging.
- **📊 Model Training & Evaluation**: Critical stages of the pipeline include model training and evaluation to ensure the development of a robust solution.
- **🚀 Containerization with Docker**: Docker is employed to simplify deployment, scaling, and ensure consistency across environments.
- **🌐 API Creation**: An API is developed to provide easy access to model predictions.
- **🔄 Efficient Data Processing**: Data transformation and efficient processing ensure timely analysis and insights.

## Key Insights

### 🌍 Cloud Utilization
- **GCP Integration**: Leveraging **Google Cloud Platform** for data storage and processing optimizes resource management, enhances accessibility, and ensures scalability for handling large datasets.

### 🔍 Modular Design
- **Pipeline Modularity**: By separating the pipeline into distinct classes for different stages (e.g., data ingestion, transformation, training), the project benefits from better organization, easier debugging, and maintainability, essential for handling complex ML pipelines.

### 💡 Continuous Integration & Deployment (CI/CD)
- **Smooth Updates**: The structured pipeline approach supports continuous integration and deployment, allowing seamless updates to both the model and the data ingestion process.

### 🛠️ Data Transformation
- **Preprocessing Importance**: Effective data transformation ensures that raw data is cleaned, transformed, and made relevant for model training, which is crucial to improving model performance.

### 📈 Model Evaluation
- **Performance Metrics**: Rigorous model evaluation based on performance metrics (e.g., accuracy, precision, recall) helps in assessing the model's effectiveness before deployment, ensuring reliability in production.

### 🐳 Docker Benefits
- **Consistency Across Environments**: Using Docker for containerization not only simplifies the deployment process but also ensures that the environment remains consistent, avoiding the common “it works on my machine” problem.

### 📡 API Accessibility
- **Seamless Integration**: Developing an API for the model facilitates its integration with other applications, making predictions easily accessible and enhancing the project's usability.

---

## 🚀 Technologies Used

- **Google Cloud Platform (GCP)**: For data storage and cloud processing.
- **Docker**: For containerizing the model and ensuring scalable and reproducible deployment.
- **Python**: For data processing, model training, and API development.
- **Flask/FastAPI**: For building the API to access the model's predictions.
- **TensorFlow/PyTorch**: For model development and training.
- **CI/CD**: Pipeline setup to ensure continuous integration and deployment.

---

## 🛠️ Setup Instructions

1. **Clone the Repository**
    ```bash
    git clone https://github.com/JEEVAABI15/End-to-End_Hate-Speech-Classification.git
    cd End-to-End_Hate-Speech-Classification
    ```

2. **Setup Environment**
    ```bash
    python3 -m venv env
    source env/bin/activate
    pip install -r requirements.txt
    ```

3. **Set Up GCP Access**
    - Configure your GCP bucket and download the service account key.
    - Set up the environment variable for the service account:
      ```bash
      export GOOGLE_APPLICATION_CREDENTIALS="path/to/service-account-file.json"
      ```

4. **Run Docker Container**
    ```bash
    docker build -t your-app-name .
    docker run -p 5000:5000 your-app-name
    ```

5. **Access the API**
    - The API can be accessed at `http://localhost:5000/predict`, where you can send POST requests with the necessary input to get model predictions.

---

## 📊 Future Improvements

- Implement **hyperparameter tuning** for further model optimization.
- Add **more advanced model monitoring and logging** mechanisms.
- Explore **distributed data processing** for larger datasets and faster computation times.
- Integrate **CI/CD pipelines** to further automate deployment and testing stages.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
