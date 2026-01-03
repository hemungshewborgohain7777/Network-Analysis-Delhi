# 🚦 Network Analysis of Delhi (Route, Closest Facility & Service Area)

## 🔹 Project Overview / Problem Statement
Network analysis is a critical GIS technique used for solving transportation and accessibility problems such as finding optimal routes, identifying nearest facilities, and determining service coverage areas.  
This project applies **Network Analyst tools in ArcMap** to perform **Route Analysis, Closest Facility Analysis, and Service Area Analysis** within a selected region of **Delhi**, using a road network dataset.

---

## 🎯 Objectives
- To analyze shortest and optimal routes between important locations  
- To identify the **closest facility** based on network distance  
- To generate **service areas** showing accessibility within defined travel distances  
- To demonstrate practical applications of **GIS-based network analysis**

---

## 📍 Study Area
The study area covers a selected urban region of **Delhi**, characterized by a dense road network and important landmarks such as:
- India Gate  
- Delhi High Court  
- Supreme Court  
- Golf Link  
- Haryana Estate  
- Modern School  


---

## 🗂 Data Sources
- **Road Network Data (Polyline Shapefile)**  
  Source: OpenStreetMap / Open Government Data portals
  DivaGIS

- **Landmark / Facility Locations (Point Data)**  
  Digitized and prepared in ArcMap 10.8 

---

## 🛠 Tools & Methodology

### Software Used
- ArcMap 10.8
- Topology Correction
- Network Analyst Extension

---

### Methodology: Network Analysis in ArcMap

#### 1. Prepare the Data
- A road/transportation polyline shapefile was prepared with attributes such as **road length, speed, and travel cost**.
- Topology checks were performed to fix errors such as dangling nodes and disconnected road segments.
- Attribute fields used for cost calculations (length, time, speed) were ensured to be **numeric**.

---

#### 2. Create a Network Dataset
- Open **ArcCatalog** (or Catalog window in ArcMap).
- Navigate to the **feature dataset** containing the road data (must be inside a geodatabase).
- Right-click the feature dataset → **New > Network Dataset**.
- Follow the wizard to:
  - Select road features as sources  
  - Define connectivity policy (Endpoint connectivity)  
  - Set impedance attributes (distance or time)  
- Build the network dataset.

---

#### 3. Enable Network Analyst Extension
- Go to **Customize > Extensions** and enable **Network Analyst**.
- Enable the **Network Analyst Toolbar** from Customize > Toolbars.

---

#### 4. Add Network Dataset to Map
- Drag the network dataset from the Catalog window into ArcMap.
- This activates the network analysis tools.

---

#### 5. Choose Type of Network Analysis
Using the Network Analyst toolbar, the following analyses were performed:

- **Route Analysis**  
  - Finds the shortest path between selected locations  

- **Closest Facility Analysis**  
  - Identifies the nearest facility from given incidents  

- **Service Area Analysis**  
  - Determines areas reachable within a specified distance  

---

#### 6. Network Analysis Steps
1. **Understand the goal**  
   - Define the analysis type (Route, Closest Facility, or Service Area).  

2. **Add locations**  
   - Load stops, facilities, or incidents using “Load Locations” or manual placement.  

3. **Run the analysis**  
   - Click the **Solve** button to execute the network computation.  

4. **Export the result**  
   - Symbolize routes, service areas, and facilities.  
   - Export the final maps for visualization.

---

## 🗺 Key Outputs
- Route Analysis Map (Shortest paths between landmarks)  
- Closest Facility Analysis Map  
- Service Area Analysis Map  

📌 **Final Map Files:**
- `Network Analysis Delhi.jpg`
- `Network Analysis Delhi Whole.jpg`
- EXTRA created Assam Network Analysis with shortest distance from Kamrup to Tinsukia.

---

## 📊 Results & Interpretation
- Route analysis successfully identifies **shortest and optimal paths** between key locations.
- Closest facility analysis highlights **minimum-distance access** to essential facilities.
- Service area analysis clearly shows **zones of accessibility**, helping assess coverage gaps.
- The results demonstrate how network-based distance differs from straight-line distance in urban environments.

---

## 📘 What I Learned
- Creation and management of **network datasets** in ArcMap  
- Practical use of **Network Analyst tools**  
- Importance of clean topology for accurate results  
- Real-world applications of route, service area, and closest facility analysis  

---

## 🔮 Future Improvements
- Incorporation of **travel time and traffic conditions**
- Multi-modal network analysis (walking, driving, public transport)
- Accessibility analysis for emergency services
- Integration with real-time or historical traffic data

---
