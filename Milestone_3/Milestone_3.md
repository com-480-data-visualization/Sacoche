# Project: Milestone 3

**Due:** 30 May 2025, 17:00

## Boston Marathon Data Visualization

An interactive data visualization exploring the Boston Marathon through race statistics, personalized pacing strategies, and animated course visualization.

**Live Demo:** [Sacoche Home Page](https://com-480-data-visualization.github.io/Sacoche/home_page.html)

---

### Overview

Three interactive components for exploring Boston Marathon data:

1. **Animated Course**  
   Watch runners race along the real GPS route.

2. **Pace Calculator**  
   Get personalized pacing strategies based on historical data.

3. **Statistics Dashboard**  
   Explore race data with interactive filtering.

---

### Technical Setup

#### Prerequisites

- Modern web browser  
- Local web server (for loading JSON data)

#### Dependencies (via CDN)

- [Chart.js 3.9.1](https://cdnjs.com/libraries/Chart.js/3.9.1)  
- [Font Awesome 6.4.0](https://cdnjs.com/libraries/font-awesome/6.4.0)  
- [Tailwind CSS 2.2.19](https://cdnjs.com/libraries/tailwindcss/2.2.19)

#### Required Files
```
├── home_page.html                          # Main page with course animation
├── pace_profile.html                       # Pacing strategy calculator
├── stats.html                              # Statistics dashboard
├── boston-marathon.gpx                     # GPS route data
├── segment_pace_profiles_all_years.json    # Pace recommendations
├── stats_marathon_2015_2017.json          # Main statistics (2015-2017)
└── stats_split_time.json                  # Split timing data
```

#### Online (Recommended)

Visit: [https://com-480-data-visualization.github.io/Sacoche/home_page.html](https://com-480-data-visualization.github.io/Sacoche/home_page.html)

### Local Development

1. Clone repository
2. Start local server:
   ```bash
   python -m http.server 8000
   # or
   npx http-server

3. Open [http://localhost:8000/home_page.html](http://localhost:8000/home_page.html)

### Features

#### Home Page
- Animated runners on the real Boston Marathon route  
- Interactive start/finish markers  
- Click runners to view level-specific statistics  

#### Pace Calculator
- Input target time and gender  
- Compute segment-by-segment pace strategy  
- Interactive pace evolution chart with elevation profile  
- Split times for all major distance markers  

#### Statistics Dashboard
- Filter by age, gender, performance level, and weather  
- Interactive charts and real-time statistics  
- Split speed analysis across race segments  

---

### Target Audience
- **Marathon Runners:** Race planning and performance analysis  
- **Data Enthusiasts:** Interactive exploration of athletic performance data  
- **Educators:** Real-world data visualization examples  

---

### Browser Requirements
A modern browser with:  
- JavaScript ES6+  
- SVG animations  
- CSS Grid support  

---

**Course:** COM-480 Data Visualization
**Team:** Sacoche
**Institution:** École Polytechnique Fédérale de Lausanne (EPFL)  
**Year:** 2024  