# Serbian Geology & Fire Reporting App

An interactive web application for visualizing mining research locations and fire reports in Serbia. Combines geological data (Geo Srbija) and NASA FIRMS fire data on a modern, bilingual map with user fire reporting and voting.

## Features
- Interactive map with geology and fire layers
- User fire reporting (right-click on map)
- Date/radius filtering, media upload, voting
- Bilingual UI (Serbian/English)
- Professional info bar with Buy Me a Coffee
- Responsive, mobile-friendly design

## Demo (GitHub Pages)
The static frontend is available at:
```
https://agatonovic.github.io/serbia_mining_and_fire/
```

## Local Development
### 1. Frontend (Static Map)
You can test the static HTML/JS frontend locally:
```sh
python -m http.server 8000
```
Then open `http://localhost:8000/geology_template.html` in your browser.

### 2. Backend (Streamlit Dashboard)
For the full backend with data processing:
```sh
pip install -r requirements.txt
streamlit run main.py
```

## Project Structure
- `geology_template.html` - Main interactive map interface
- `geology_data.json` - Serbian geological data (Geo Srbija)
- `fire_data.json` - NASA FIRMS fire data
- `assets/` - Static assets (CSS, JS, images)
- `datasets/` - Additional Serbian datasets
- `requirements.txt` - Python dependencies

## Data Sources
- **Geology**: Geo Srbija (Serbian Geological Survey)
- **Fire Data**: NASA FIRMS (Fire Information for Resource Management System)
- **Additional Data**: Various Serbian government datasets

## Deployment
This project is deployed on GitHub Pages. The static frontend is automatically served from the main branch.

## License
This project is open source and available under the MIT License.