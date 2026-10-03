\# 🎬 MovieFlix AI



\### AI-Powered Movie Prediction \& Netflix-Style Recommendation Platform



!\[MovieFlix AI Demo](docs/demo-dashboard.svg)



MovieFlix AI is a full-stack Machine Learning web application that predicts movie ratings and recommends similar movies using a dataset of \*\*5,000 movies\*\*.



The project combines \*\*Machine Learning, FastAPI, React, Vite, Tailwind CSS, and Docker\*\* to create a modern Netflix-style movie discovery platform.



\---



\## 🌟 Project Preview



MovieFlix AI provides a cinematic streaming-style interface where users can:



\- 🎬 Browse thousands of movies

\- 🔎 Search for movies

\- 🎭 Filter movies by genre

\- ⭐ View ratings and popularity

\- 🧠 Get AI-powered recommendations

\- 🤖 Predict the potential rating of a movie

\- 📊 Explore movie analytics

\- 🎯 Discover similar movies

\- 📱 Use the platform on different screen sizes



\---



\## ✨ Main Features



\### 🎥 Netflix-Style Movie Interface



A modern cinematic interface inspired by popular streaming platforms.



Features include:



\- Large hero section

\- Movie cards

\- Genre filters

\- Search bar

\- Movie details

\- Similar movie recommendations

\- High-contrast buttons

\- Glassmorphism UI

\- Neon gradient effects

\- Responsive design



\---



\### 🤖 AI Movie Rating Prediction



The application uses a \*\*Random Forest Regression\*\* model to estimate a movie's potential rating.



The model uses:



\- Release year

\- Runtime

\- Budget

\- Number of votes

\- Popularity

\- Revenue



The prediction system returns:



```text

Predicted Rating

Confidence Score

Movie Verdict

```



Example:



```text

Predicted Rating: 7.8 / 10



Confidence: 89%



Verdict: Hit Potential

```



\---



\### 🧠 AI Movie Recommendation System



Movie recommendations are generated using:



```text

TF-IDF Vectorization

&#x20;       +

Cosine Similarity

```



The recommendation engine analyzes:



\- Movie title

\- Genre

\- Subgenre

\- Director

\- Cast



When a user opens a movie, the system generates similar movies automatically.



Example:



```text

User selects:



Midnight Protocol



↓



MovieFlix AI analyzes the movie



↓



TF-IDF + Cosine Similarity



↓



Similar Movies



1\. Neon Horizon

2\. Digital Ghost

3\. Quantum Hearts

4\. Shadow Circuit

```



\---



\## 📊 Dataset



The project contains a dataset of:



\# 5,000 Movies



Each movie contains information such as:



| Field | Description |

|---|---|

| ID | Unique movie identifier |

| Title | Movie title |

| Year | Release year |

| Genre | Main genre |

| Subgenre | Secondary genre |

| Runtime | Movie duration |

| Budget | Production budget |

| Rating | Audience rating |

| Votes | Number of votes |

| Popularity | Popularity score |

| Revenue | Revenue |

| Language | Movie language |

| Platform | Streaming/platform category |

| Director | Director |

| Cast | Main cast |



The dataset is included locally, so the application does not require an external movie API or API key.



\---



\# 🛠️ Technology Stack



\## Frontend



\- React

\- Vite

\- JavaScript

\- Tailwind CSS

\- Lucide React



\## Backend



\- Python

\- FastAPI

\- Uvicorn

\- Pandas

\- NumPy

\- Pydantic



\## Machine Learning



\- Scikit-learn

\- Random Forest Regression

\- TF-IDF Vectorization

\- Cosine Similarity



\## DevOps



\- Docker

\- Docker Compose

\- Git

\- GitHub



\---



\# 🏗️ System Architecture



```text

&#x20;                   MOVIEFLIX AI

&#x20;                        │

&#x20;                        ▼

&#x20;             ┌────────────────────┐

&#x20;             │   React Frontend   │

&#x20;             │  Vite + Tailwind   │

&#x20;             └─────────┬──────────┘

&#x20;                       │

&#x20;                       │ REST API

&#x20;                       ▼

&#x20;             ┌────────────────────┐

&#x20;             │    FastAPI API     │

&#x20;             │      Backend       │

&#x20;             └─────────┬──────────┘

&#x20;                       │

&#x20;            ┌──────────┴───────────┐

&#x20;            ▼                      ▼

&#x20;    ┌───────────────┐      ┌────────────────┐

&#x20;    │ Rating Model  │      │ Recommendation │

&#x20;    │ Random Forest │      │ TF-IDF +       │

&#x20;    │               │      │ Cosine         │

&#x20;    └───────────────┘      └────────────────┘

&#x20;            │                      │

&#x20;            └──────────┬───────────┘

&#x20;                       ▼

&#x20;              ┌─────────────────┐

&#x20;              │ 5,000 Movies    │

&#x20;              │ CSV Dataset     │

&#x20;              └─────────────────┘

```



\---



\# 🧠 Machine Learning



\## Rating Prediction



The prediction model is:



```text

RandomForestRegressor

```



Input features:



```text

year

runtime

budget\_million

votes

popularity

revenue\_million

```



The model produces:



```text

Predicted Rating

Confidence

Verdict

```



The verdict is categorized as:



```text

7.2+  → Hit Potential



6.2+  → Promising



Below → Mixed

```



\---



\# 🎯 Recommendation Engine



The recommendation engine converts movie information into TF-IDF vectors.



```text

Movie Information

&#x20;      │

&#x20;      ▼

Text Processing

&#x20;      │

&#x20;      ▼

TF-IDF Vectorization

&#x20;      │

&#x20;      ▼

Cosine Similarity

&#x20;      │

&#x20;      ▼

Similarity Score

&#x20;      │

&#x20;      ▼

Recommended Movies

```



Example:



```text

Movie A

&#x20;  │

&#x20;  ├── Genre

&#x20;  ├── Subgenre

&#x20;  ├── Director

&#x20;  └── Cast

&#x20;       │

&#x20;       ▼

&#x20;  TF-IDF Vector

&#x20;       │

&#x20;       ▼

&#x20;  Similarity Calculation

&#x20;       │

&#x20;       ▼

&#x20;Recommended Movies

```



\---



\# 📁 Project Structure



```text

Movieflix-Predictor/

│

├── backend/

│   │

│   ├── app/

│   │   └── main.py

│   │

│   ├── data/

│   │   └── movies.csv

│   │

│   ├── requirements.txt

│   ├── Dockerfile

│   └── README.md

│

├── frontend/

│   │

│   ├── src/

│   │   ├── components/

│   │   ├── pages/

│   │   ├── main.jsx

│   │   └── index.css

│   │

│   ├── public/

│   │   └── images/

│   │

│   ├── package.json

│   └── vite.config.js

│

├── docs/

│   └── demo-dashboard.svg

│

├── docker-compose.yml

├── .gitignore

└── README.md

```



\---



\# 🚀 Installation



\## Option 1 — Docker



The easiest way to run the complete application.



From the project root:



```powershell

docker compose up --build

```



After Docker starts:



\### Frontend



```text

http://localhost:5173

```



\### Backend



```text

http://localhost:8000

```



\### API Documentation



```text

http://localhost:8000/docs

```



\---



\# 🐍 Option 2 — Run Backend Manually



Open PowerShell.



Navigate to the backend:



```powershell

cd backend

```



Create a virtual environment:



```powershell

python -m venv venv

```



Activate it:



```powershell

.\\venv\\Scripts\\Activate.ps1

```



Install dependencies:



```powershell

pip install -r requirements.txt

```



Start FastAPI:



```powershell

uvicorn app.main:app --reload --port 8000

```



Backend will run at:



```text

http://localhost:8000

```



\---



\# ⚛️ Run Frontend



Open another PowerShell window.



Navigate to frontend:



```powershell

cd frontend

```



Install dependencies:



```powershell

npm install

```



Start Vite:



```powershell

npm run dev

```



Open:



```text

http://localhost:5173

```



\---



\# 🔌 API Endpoints



| Endpoint | Method | Purpose |

|---|---|---|

| `/api/health` | GET | Check API status |

| `/api/movies` | GET | Search/browse movies |

| `/api/movie/{id}` | GET | Get movie details |

| `/api/recommend/{id}` | GET | Get similar movies |

| `/api/predict` | POST | Predict movie rating |

| `/api/stats` | GET | Get dataset analytics |



\---



\# 🧪 Prediction API Example



\### Request



```json

{

&#x20; "year": 2026,

&#x20; "runtime": 120,

&#x20; "budget\_million": 60,

&#x20; "votes": 50000,

&#x20; "popularity": 55,

&#x20; "revenue\_million": 220

}

```



\### Response



```json

{

&#x20; "predicted\_rating": 7.8,

&#x20; "confidence": 89.6,

&#x20; "verdict": "Hit potential"

}

```



\---



\# 🔎 Movie Search



The platform supports movie searching through the API.



Example:



```text

Search:



Midnight

```



The system returns matching movies from the 5,000-movie dataset.



\---



\# 🎭 Genre Filtering



Available genres include:



```text

Action

Adventure

Animation

Comedy

Crime

Drama

Fantasy

Horror

Mystery

Romance

Sci-Fi

Thriller

```



\---



\# 📈 Analytics Dashboard



The analytics dashboard provides information about:



\- Total movies

\- Average rating

\- Average popularity

\- Genre distribution

\- Platform distribution

\- Top movies



Example:



```text

Movies

5,000



Average Rating

6.8



Average Popularity

52.4

```



\---



\# 🎨 UI Design



MovieFlix AI uses a modern cinematic design system.



\### Design Elements



\- Dark background

\- Neon purple gradients

\- Cyan highlights

\- Glassmorphism cards

\- Rounded components

\- High-contrast buttons

\- Cinematic movie sections

\- Responsive layouts

\- Hover animations

\- AI-focused visual elements



\---



\# 🖼️ Demo Images



The project includes local demo graphics inside:



```text

frontend/public/images/

```



Available demo assets include:



```text

hero-midnight.svg

hero-neon.svg

hero-ocean.svg

hero-crimson.svg

```



The project also contains:



```text

docs/demo-dashboard.svg

```



These assets allow the repository to display visual content without depending on external image URLs.



\---



\# 📱 Responsive Design



MovieFlix AI is designed to work across:



```text

Desktop

Laptop

Tablet

Mobile

```



The layout automatically adapts movie cards, navigation, search, prediction panels and analytics sections.



\---



\# 🔐 API \& Security



The project is designed as a local academic/portfolio application.



No external API keys are required.



The frontend communicates with the FastAPI backend through REST endpoints.



\---



\# 🐳 Docker Architecture



```text

&#x20;            Docker Compose

&#x20;                   │

&#x20;         ┌─────────┴─────────┐

&#x20;         │                   │

&#x20;         ▼                   ▼

&#x20;    Frontend             Backend

&#x20;    React/Vite            FastAPI

&#x20;    Port 5173             Port 8000

&#x20;         │                   │

&#x20;         └─────────┬─────────┘

&#x20;                   │

&#x20;                   ▼

&#x20;             Movie Dataset

&#x20;                5,000

```



\---



\# 🎓 Project Applications



This project can be used as:



\- Machine Learning college project

\- Full-stack development project

\- Data Science project

\- AI/ML portfolio project

\- GitHub portfolio project

\- Resume project

\- Final-year project foundation

\- Recommendation system demonstration



\---



\# 📚 Learning Outcomes



Through this project, you can demonstrate knowledge of:



\### Machine Learning



\- Regression

\- Random Forest

\- Feature engineering

\- Model prediction

\- Similarity algorithms



\### NLP



\- Text preprocessing

\- TF-IDF

\- Vectorization

\- Cosine similarity



\### Backend Development



\- REST APIs

\- FastAPI

\- Pydantic

\- API routing



\### Frontend Development



\- React

\- Vite

\- Tailwind CSS

\- Component-based architecture

\- Responsive UI



\### DevOps



\- Docker

\- Docker Compose

\- Git

\- GitHub



\---



\# 🔮 Future Improvements



Possible future upgrades include:



\- 🎞️ Real movie posters

\- 🎬 TMDB API integration

\- 👤 User authentication

\- ❤️ Watchlist

\- ⭐ User ratings

\- 🧑 Personalized recommendation profiles

\- 🔥 Trending movies

\- 📺 Streaming availability

\- 💬 AI movie assistant

\- ☁️ AWS deployment

\- 🗄️ PostgreSQL database

\- 📊 Advanced ML evaluation

\- 🎯 Deep-learning recommendation model



\---



\# 👩‍💻 Author



\## Chaitanya Karanam



B.Tech Computer Science Student  

Data Engineering \& Machine Learning Enthusiast



GitHub:



https://github.com/chaitanyakaranam777



\---



\# ⭐ Support



If you found this project useful, consider giving the repository a ⭐ on GitHub.



\---



\## 📜 License



This project is intended for educational, academic and portfolio purposes.



The included movie dataset is synthetic/demo data created specifically for this project.



\---



\# 🎬 MovieFlix AI



\### Discover. Predict. Recommend.



\*\*Powered by Machine Learning + FastAPI + React\*\*

