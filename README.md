# Dark Pattern & UX Manipulation Detector 🔍

A high-compute scraping project that detects dark patterns and UX manipulation in e-commerce checkouts, SaaS onboarding flows, and subscription cancellation pages. Use computer vision and flow analysis to identify deceptive design patterns.

## 🎯 Project Overview

**Goal**: Build a comprehensive dark pattern detection system to:
- Scan e-commerce checkout flows for manipulation tactics
- Detect deceptive SaaS cancellation patterns
- Identify urgency indicators and fake scarcity
- Analyze subscription traps and hidden costs
- Generate compliance reports for regulators

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│              Dark Pattern & UX Manipulation Detector              │
├─────────────────────────────────────────────────────────────┤
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────────┐   │
│  │   Flow     │  │  Pattern   │  │   Computer     │   │
│  │   Crawler  │──▶│  Detector  │──▶│   Vision       │   │
│  └─────────────┘  └─────────────┘  └─────────────────┘   │
│                   └─────────────┘  ┌─────────────────┐   │
│  ┌─────────────┐  ┌─────────────┐  │   Report       │   │
│  │  Headless   │  │  Database   │  │   Generator   │   │
│  │  Browser    │  │ (PostgreSQL)│  └─────────────────┘   │
│  └─────────────┘  └─────────────┘                          │
└─────────────────────────────────────────────────────────────┘
```

## 📊 Data Sources

- **E-commerce Checkouts**: Amazon, Shopify, WooCommerce stores
- **SaaS Onboarding**: Subscription service flows
- **Cancellation Pages**: Difficult unsubscribe processes
- **Pricing Pages**: Hidden fees, drip pricing
- **Social Proof**: Fake reviews, testimonials

## 🔧 Tech Stack

- **Language**: Python + TypeScript
- **Scraping**: Playwright, Puppeteer
- **Computer Vision**: OpenCV, YOLO
- **OCR**: Tesseract, EasyOCR
- **NLP**: transformers for text analysis
- **Database**: PostgreSQL
- **API**: FastAPI
- **Queue**: Redis + Celery

## 🚀 Getting Started

```bash
# Clone the repo
git clone https://github.com/yksanjo/dark-pattern-detector.git
cd dark-pattern-detector

# Install dependencies
pip install -r requirements.txt

# Set up environment
cp .env.example .env

# Run the detector
python src/detector/checkout_scanner.py

# Start the API
uvicorn src.api.main:app --reload
```

## 📈 Features

- [ ] Automated flow crawling
- [ ] Dark pattern classification
- [ ] Computer vision element detection
- [ ] Text analysis for manipulation
- [ ] Screenshot comparison
- [ ] Compliance report generation
- [ ] Real-time alerting

## 📊 Project Phases

### Phase 1: Flow Collection
- Checkout flow crawler
- SaaS flow scanner
- Subscription page miner

### Phase 2: Detection
- Visual element detection
- Text pattern analysis
- Flow state tracking

### Phase 3: Classification
- Dark pattern taxonomy
- Severity scoring
- Category classification

### Phase 4: Reporting
- Compliance reports
- Dashboard analytics
- API access

## 📝 License

MIT License - See [LICENSE](LICENSE) for details.

## 👤 Author

Yoshi Kondo - [@yksanjo](https://github.com/yksanjo)

---

🛡️ Expose deceptive design, protect users!
