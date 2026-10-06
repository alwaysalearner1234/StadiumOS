# 🏟️ StadiumOS AI

**An AI-powered operations and fan-experience platform for FIFA World Cup 2026™ stadiums.**

StadiumOS AI brings two views into one web app: a **Fan Hub** that helps attendees navigate the stadium, get answers in their own language, and travel sustainably, and a **Command Centre** that gives organizers real-time crowd intelligence and AI-generated incident response plans.

> The demo is set at **MetLife Stadium (NY/NJ)** with a live-match scenario (USA vs England).

🔗 **Live demo:** `https://alwaysalearner1234.github.io/StadiumOS/`

---

## ✨ Features

### 👥 Fan Hub
- **AI Multilingual Assistant**: a concierge chat for gates, accessibility, transit, bag policies, and match info, with language support for English, Spanish, French, Portuguese, German, and Arabic.
- **Interactive Stadium Map**: a live crowd heatmap with per-gate wait times and an **Accessible Routes** overlay.
- **Smart Gate Routing**: the digital match pass is assigned the lowest-wait gate, with an AI routing explanation.
- **Eco-Transit & Carbon Impact**: compare train, bus, rideshare, and private car, with CO₂ estimates and sustainability advice.
- **Digital Match Pass**: match, kickoff, gate, section, and seat at a glance.

### 🛡️ Command Centre (Organizers & Staff)
- **Operations Scorecard**: total attendance, crowd density index, and active incident count.
- **Scenario Simulator**: trigger Gate D congestion, a Section 104 medical emergency, a transit station delay, or a lost child at Gate A, and adjust crowd capacity with a slider.
- **Live Alarm Feed**: incidents from simulated IoT sensor and CCTV inputs.
- **AI Decision Support**: for each incident, the system generates:
  - a recommended **Standard Operating Procedure (SOP)**
  - a **multilingual fan broadcast** that can be pushed to the Fan Hub screen
  - **tactical staff instructions**
  - **suggested team allocations**, with one-click approve and dispatch
- **Field Resource Tracker**: marshals and emergency response units, with assignment, location, and status.

---

## 🧱 Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, JavaScript (ES Modules) |
| Build tool | [Vite](https://vite.dev/) |
| Hosting | Firebase Hosting |
| CI/CD | GitHub Actions |
| UI | Google Fonts (Outfit, Plus Jakarta Sans), Font Awesome |

---

## 📁 Project Structure

```
StadiumOS/
├── .github/workflows/   # CI/CD pipeline
├── public/              # Static assets
├── src/                 # Application source (entry: src/main.js)
├── index.html           # App shell: Fan Hub + Command Centre views
├── firebase.json        # Firebase Hosting config
├── vite.config.js       # Vite config
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) 18+ and npm

### Run locally

```bash
# 1. Clone the repository
git clone https://github.com/alwaysalearner1234/StadiumOS.git
cd StadiumOS

# 2. Install dependencies
npm install

# 3. Start the dev server
npm run dev
```

Open the local URL printed in your terminal (usually `http://localhost:5173`).

### Build for production

```bash
npm run build     # outputs to /dist
npm run preview   # preview the production build locally
```

### Deploy to Firebase

```bash
npm install -g firebase-tools
firebase login
npm run build
firebase deploy
```

---

## 🎮 How to Use the Demo

1. **Fan Hub**: ask the assistant a question, tap a quick chip (Gate Access, Eco Transit, Bag Rules, Matches), switch the language, hover gates on the map, and try different travel modes in the carbon calculator.
2. **Command Centre**: switch using the header toggle, then trigger a scenario in the simulator. Select the incident in the alarm feed to see the AI-generated SOP, announcement, and dispatch plan. Approve the plan to dispatch teams, or broadcast the announcement back to the Fan Hub.

> ⚠️ All crowd, weather, match, and incident data in the demo is **simulated** for demonstration purposes.

---

## 🗺️ Roadmap

- [ ] Connect to live IoT / ticketing / transit data feeds
- [ ] Real-time sync between the Fan Hub and Command Centre
- [ ] Voice input for the multilingual assistant
- [ ] Push notifications for gate and transit changes
- [ ] Multi-stadium support for all 2026 host venues

---

## 🤝 Contributing

Contributions are welcome. Fork the repo, create a feature branch, and open a pull request.

## 📄 License

Add a license of your choice (e.g. MIT) and update this section.

## 👤 Author

**Lidhiya**: [@alwaysalearner1234](https://github.com/alwaysalearner1234)

---

*StadiumOS AI is an independent project and is not affiliated with or endorsed by FIFA.*
