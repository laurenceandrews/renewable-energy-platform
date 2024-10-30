# ⚡ Renewable Energy Monitoring and Forecasting Platform

## 📄 Overview
The Renewable Energy Monitoring and Forecasting Platform is a full-stack application aimed at real-time monitoring, data visualization, and forecasting for renewable energy assets such as solar panels and wind turbines. With an interactive dashboard, users can observe and analyze energy production, consumption, and storage patterns. The project combines a robust backend with a user-friendly frontend and supports predictive analytics for energy management optimization.

## 🛠️ Technologies Used
- **Backend**: Python, FastAPI, PostgreSQL (with TimescaleDB for time-series data), Apache Kafka, Redis
- **Frontend**: React, D3.js, Plotly, Mapbox for interactive data visualizations and geolocation mapping
- **Data Processing and ML**: Python, TensorFlow, Scikit-Learn, Pandas
- **Orchestration and Infrastructure**: Docker, Kubernetes
- **IoT Integration**: MQTT for IoT device communication (simulated for testing)

## 📂 Project Structure
- `app/`: Core application code with backend API setup, database models, and business logic.
  - `main.py`: Main entry point for running the FastAPI backend.
  - `config.py`: Configuration settings for environment variables and database connections.
  - `models/`: Database models for time-series data storage and other records.
  - `routes/`: API endpoints for managing energy data and user interactions.
- `frontend/`: React-based frontend with visualization components.
  - `dashboard/`: Contains dashboard components for real-time data visualization and interaction.
- `tests/`: Unit and integration tests to validate data processing and API functionality.
- `requirements.txt`: Python dependencies required for the backend.
- `requirements-dev.txt`: Development dependencies for testing and linting.
- `.github/workflows/ci.yml`: GitHub Actions workflow for continuous integration.
- `Dockerfile` and `docker-compose.yml`: Container setup files for local development and deployment.

## ⭐ Features
- **Real-Time Monitoring**: Captures and displays live data from energy sources to enable immediate insights.
- **Time-Series Data Storage and Analysis**: Uses PostgreSQL with TimescaleDB for efficient time-series data management and querying.
- **Energy Forecasting and Anomaly Detection**: Predictive models trained on historical data help forecast energy trends and identify anomalies.
- **Interactive Dashboards**: Provides users with intuitive visualizations of energy metrics through charts, graphs, and maps.
- **Scalable Microservices Architecture**: Uses Docker and Kubernetes for easy scaling and deployment.

## 📋 Data Handled
The platform handles various metrics related to renewable energy assets, including:
- **Energy Production** and **Consumption**: Real-time data on generated and consumed energy.
- **Battery Storage Levels**: Tracks energy storage and usage patterns.
- **Asset Location** and **Status**: Monitors the operational status and geolocation of assets like wind turbines and solar panels.
- **Forecasted Trends**: Predictive analytics based on historical data, including energy production and usage forecasts.

## 🌱 Setup and Installation

### 📋 Requirements
- **Python 3.8+**: Required for the backend components.
- **Virtual Environment**: Recommended for dependency management.
- **Docker**: For containerization and orchestration setup.
- **Node.js and npm**: Required for running the frontend.

### 🚀 Getting Started

1. **Clone the repository**:
    ```bash
    git clone https://github.com/laurenceandrews/renewable-energy-platform.git
    cd renewable-energy-platform
    ```

2. **Set up a virtual environment for the backend**:
    ```bash
    python -m venv venv
    ```

3. **Activate the virtual environment**:
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install backend dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

5. **Run the backend API**:
    ```bash
    uvicorn app.main:app --reload
    ```

6. **Set up the frontend (React)**:
   - Navigate to the frontend directory:
     ```bash
     cd frontend
     ```
   - Install dependencies:
     ```bash
     npm install
     ```
   - Start the frontend development server:
     ```bash
     npm start
     ```

### 🔄 Additional Setup for Docker and Kubernetes (Optional)
- Build and run Docker containers:
  ```bash
  docker-compose up --build

### 📝 Contributing
Contributions are welcome! Please feel free to fork this repository, submit issues, or create pull requests for new features, improvements, or bug fixes.

### 📜 License
This project is licensed under the MIT License – see the LICENSE file for details.