# Internship_As

This assignment could be 80% complted with core development finished due to large dataset and lack of resources . 

This project is a part of the Solvei8 AI/ML Internship assignment. It involves developing a booking analytics and QA system using FastAPI. The goal is to create a system that provides analytics reports and answers booking-related questions using RAG (Retrieval-Augmented Generation).

🚀 Project Overview
Booking Analytics: Analyze booking data and provide insights.

QA System: Implement a question-answering system using the RAG approach.

FastAPI: Develop a REST API with endpoints for analytics and Q&A.

Database Management: SQLite database for storing booking data.

🏗 Project Structure

├── sample_data/
│   ├── analytics.db
│   ├── cleaned_hotel_bookings.csv
├── fastapi_app.py
├── main.py
└── README.md
sample_data/analytics.db: Contains the processed booking data.

sample_data/cleaned_hotel_bookings.csv: Cleaned CSV data for reference.

fastapi_app.py: API implementation using FastAPI.

main.py: Script to run and test the API.

⚙️ Setup Instructions
1. Clone the Repository

git clone https://[github.com/BhavanaSingh28/Internship_Assignment](https://github.com/BhavanaSingh28/Internship_As).git
cd Internship_As

3. Install Dependencies
pip install -r requirements.txt


4. Run the FastAPI Server
uvicorn fastapi_app:app --host 0.0.0.0 --port 8000 --reload


5. Access the API
Open your browser and navigate to:
http://localhost:8000/docs

Explore API endpoints using Swagger UI.

📌 API Endpoints
1. Get Analytics
Endpoint: POST /analytics

Description: Retrieve booking analytics data.

Request Example:
{
  "metric": "total_bookings"
}



Response Example:
{
  "metric": "total_bookings",
  "value": 150
}
2. Ask a Question
Endpoint: POST /ask

Description: Get AI-powered responses to booking-related questions.

Request Example:
{
  "question": "What is the average booking price?"
}



Response Example:
{
  "question": "What is the average booking price?",
  "answer": "The average booking price is $120."
}


🧪 Testing
test the API using tools like:
Swagger UI at /docs
Postman or curl for API testing.

Example using curl:

curl -X POST http://localhost:8000/analytics \
-H "Content-Type: application/json" \
-d '{"metric": "total_bookings"}'


📝 Future Enhancements
1. Improve accuracy of the RAG-based QA system.
2. Implement data visualization for better insights.
3. Add additional analytics metrics.

