Here’s a clean README.md you can use for the PowerPoint generator project:


---

🖼️ AI-Powered PowerPoint Generator

This project helps you create a professional 5-slide PowerPoint presentation in minutes using either:

OpenAI (ChatGPT/Gemini style prompt → structured slide content)

Or a plain text file with slide titles and bullet points


It automatically builds a .pptx file with proper layouts and editable text using python-pptx.


---

✨ Features

🔹 Generate slides from a topic using OpenAI API

🔹 Or supply a text file with your own content

🔹 Auto-formats titles and bullet points into 5 slides

🔹 Exports to editable .pptx (works in PowerPoint, Google Slides, Canva)

🔹 Simple command-line tool, easy to customize



---

📦 Installation

Clone this repo and install dependencies:

git clone https://github.com/yourusername/ppt-generator.git
cd ppt-generator
pip install -r requirements.txt

requirements.txt should contain:

python-pptx
openai   # optional, only if using AI generation


---

🚀 Usage

1. Generate from OpenAI (AI Mode)

Requires OpenAI API key:

export OPENAI_API_KEY="sk-..."   # Linux / macOS
setx OPENAI_API_KEY "sk-..."     # Windows PowerShell

python generate_ppt.py --topic "Future of Electric Vehicles in India" --output ev_india.pptx

2. Generate from a Text File (Manual Mode)

Create a file slides.txt like this:

Future of Electric Vehicles in India
- Growth drivers: policy, subsidies, charging infra
- Consumer interest rising in metros
- Manufacturing hub potential

Market Size & Trends
- EV sales CAGR expected high
- Two-wheelers dominate early adoption
- Battery cost decline helps affordability

Charging Infrastructure
- Public chargers in cities & highways
- Fast charging hubs for intercity trips
- Private home charging solutions

Policy & Incentives
- Purchase subsidies and tax benefits
- FDI and manufacturing incentives
- Scrappage and emissions regulations

Challenges & Opportunities
- Grid readiness & charging standardization
- Battery recycling and second-life solutions
- Opportunity for local supply chain growth

Run:

python generate_ppt.py --input slides.txt --output my_presentation.pptx


---

📂 Output

A .pptx file with 5 slides:

Slide 1: Title + subtitle

Slides 2–5: Title + bullet points



You can open/edit in Microsoft PowerPoint, Google Slides, or Canva.


---

🛠️ Customization

Change fonts, sizes, or colors by editing `build_presentation


