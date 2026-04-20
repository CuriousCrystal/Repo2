Event Crowd Management & AI Assistant

What Works (Really Well)
🎤 Voice Assistant ("August")

Listens via microphone, speaks responses
Can fetch live crowd data and make recommendations
Falls back to text input gracefully
Understands commands like "open YouTube" or "what time is it"

Example conversation:
You: "Where's the shortest wait for the restroom?"
August: *fetches wait times from API* 
        "Restrooms North has only a 1 minute wait right now!"
        
🔐 Authentication
Three default users (admin/manager/viewer) with different permissions
JWT tokens with 30-min expiration
Bcrypt password hashing
Proper role-based access control

📊 Dashboard
Real-time zone status display
Alert notifications with badges
Historical analytics (stores data every 5 seconds)
View past data with time-range queries

🚨 Alert System
Configurable thresholds for density/wait times
Three severity levels: Medium, High, Critical
Database persistence of all alerts
Audit logging of user actions


How to Actually Run This
Prerequisites
bash# You need:
- Python 3.8+
- Node.js 16+
- A microphone (for voice features)
- X.AI API key (for Grok)
Backend Setup
bash# Install dependencies
pip install -r requirements.txt
