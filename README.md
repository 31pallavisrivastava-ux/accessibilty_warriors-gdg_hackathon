# 🏟️ PS-25: Lucknow Agentic Sports Discovery & Booking Platform

**Team**: [Your Team Name]  
**Members**: [Name/GitHub], [Name/GitHub], [Name/GitHub]  
**Project**: Autonomous AI agent that discovers, recommends, books, and cancels sports facilities across Lucknow based on skill level, location, and budget.

### Problem Addressed
Lucknow lacks a unified layer for sports infrastructure discovery and booking. Venues are scattered, unindexed, and require manual coordination. Our agent centralizes discovery, autonomously handles bookings/cancellations, and personalizes recommendations.

### Tech Stack & AI Tools
- Backend: FastAPI, LangChain (Tool-Calling Agent), Python 3.10+
- Frontend: HTML/JS, Leaflet.js, Tailwind CSS (CDN)
- Data: JSON mock dataset (Lucknow-specific)
- AI Tools Used: GitHub Copilot (code scaffolding), ChatGPT/Claude (prompt engineering & agent logic), LangChain docs
- LLM Provider: [OpenAI/Groq/Anthropic] via API key

### Setup & Run
1. `cd backend && pip install -r requirements.txt`
2. `cp .env.example .env` → add `OPENAI_API_KEY` (or GROQ/ANTHROPIC)
3. `python main.py` → runs on `http://localhost:8000`
4. Open `http://localhost:8000` for UI

### Known Limitations
- Venue data is mocked for hackathon demo
- Booking/cancellation simulates real-world flow (no payment gateway)
- Real-time sync uses local state; production would use WebSockets + DB