# Personalized Travel Itinerary Planner

An interactive Streamlit-based travel planning application that creates personalized, day-by-day travel itineraries based on destination, travel preferences, budget, pace, interests, and trip duration.

## Features

- **Smart destination recommendations** — recommends up to 3 cities when the user wants inspiration.
- **Personalized trip preferences** — destination, travel vibe, trip duration, dates, budget, party size, pace, and interests.
- **Day-by-day itinerary generation** — organizes activities into Morning, Lunch, Afternoon, and Evening slots.
- **Location-aware day planning** — groups activities by area to reduce unnecessary backtracking.
- **Live budget tracking** — estimates trip costs in USD, local currency, and INR.
- **Activity swapping** — replace an individual activity/slot while keeping the rest of the itinerary intact.
- **Trip history** — save and reopen generated trips during the session.
- **Offline PDF travel guide** — generate and download a printable itinerary PDF.
- **Backup and restore** — export saved trips as JSON and restore them later.
- **Demo mode** — the core application can be demonstrated without an external API key.

## Tech Stack

- Python
- Streamlit
- Pandas
- Requests
- fpdf2

## Project Structure

```text
TravelPlanner/
├── app.py
├── requirements.txt
└── README.md
```

## Installation

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Install the required packages:

```bash
pip install -r requirements.txt
```

4. Start the Streamlit application:

```bash
streamlit run app.py
```

5. Open the local URL shown by Streamlit, usually:

```text
http://localhost:8501
```

## Demo Mode

The application includes a **Demo mode** so the main travel-planning workflow can be demonstrated without configuring an external API key.

## Deployment

The application is designed to run on **Streamlit Community Cloud**.

For deployment:

1. Push `app.py`, `requirements.txt`, and `README.md` to a public GitHub repository.
2. Open Streamlit Community Cloud.
3. Select the GitHub repository.
4. Select the `main` branch.
5. Set the main file path to `app.py`.
6. Deploy the application.

## Usage

1. Choose whether you already know your destination or want destination inspiration.
2. Configure trip preferences.
3. Generate recommendations or plan the selected destination.
4. Generate the itinerary.
5. Review the daily plan and budget.
6. Customize or swap activities when needed.
7. Save the trip.
8. Generate and download the PDF travel guide.

## Notes

- Budget values and exchange rates are estimates and should be verified before actual travel.
- Saved trips are session-based unless exported using the JSON backup feature.
