# Modern AI-Powered Shopify Theme

A modern, customizable Shopify theme built with performance and user experience in mind. This theme features a clean, minimalist design with powerful AI-driven customization options and advanced features.

## Features Currently

- 📱 Fully responsive design
- 🎨 Customizable color schemes
- 🏷️ Modern product grid layouts
- 🔍 Featured product sections with flexible layouts
- 📢 Announcement bar
- 📰 Newsletter popup
- 👥 Testimonials section
- 🏢 Brand logos showcase
- 🦸‍♂️ Hero banner
- 📝 Rich text sections
- 🛒 Optimized product pages
- 🎯 Conversion-focused design

## Upcoming AI Features

### 🤖 AI-Powered Personalization
- Product recommendations using LightFM
- Personalized user experiences
- Behavioral analysis and adaptation

### ✍️ AI-Generated Content
- Automatic product descriptions using GPT-NeoX/GPT-J
- SEO-optimized content generation
- Dynamic content adaptation

### 🖼️ Smart Image Processing
- Automatic image tagging using DeepDetect/YOLO
- Visual search capabilities
- Image-based recommendations

### 💬 AI Customer Support
- Intelligent chatbot using Rasa
- Automated customer service
- 24/7 support availability

### 🗣️ Voice Search & Navigation
- Voice-enabled search using Vosk/Coqui STT
- Voice navigation support
- Accessibility improvements

### 📊 AI-Driven Analytics
- Advanced analytics using Metabase
- Predictive inventory management
- Customer behavior insights

### 🔍 Quick Look Features
- Popup product preview
- Quick add to cart
- Image/video gallery
- Product details and variants

## Getting Started

### Prerequisites

- [Shopify CLI](https://shopify.dev/themes/tools/cli) installed
- [Node.js](https://nodejs.org/) (version 14 or higher)
- A Shopify store (Development or Production)
- Python 3.8+ (for AI features)
- Virtual Environment Manager (pipenv, venv, or conda)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ebattleGWT/bits-shopify-theme
cd bits-shopify-theme
```

2. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your credentials
```

3. Choose your environment setup method:

#### Option A: Using Python Virtual Environment (venv)
```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
.\venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

#### Option B: Using Conda
```bash
# Create a conda environment
conda create -n shopify-theme python=3.8
conda activate shopify-theme
pip install -r requirements.txt
```

4. Use Shopify CLI to push the theme to your store:
```bash
shopify theme push
```

### Development

To start development with live reloading:
```bash
shopify theme dev
```

For AI features development:

#### Start Individual Services

1. Start the Recommendation System:
```bash
# In a new terminal
source venv/bin/activate  # or conda activate shopify-theme
python scripts/services/recommendation_service.py
```

2. Start the Content Generation Service:
```bash
# In a new terminal
source venv/bin/activate  # or conda activate shopify-theme
python scripts/services/content_service.py
```

3. Start the Image Processing Service:
```bash
# In a new terminal
source venv/bin/activate  # or conda activate shopify-theme
python scripts/services/image_service.py
```

4. Start the Main Development Server:
```bash
npm run dev
```

## AI Services Setup

### Local Setup (Without Docker)

1. Set up PostgreSQL:
   - Install PostgreSQL from [postgresql.org](https://www.postgresql.org/download/)
   - Create a database named 'shopify_theme_db'
   - Update .env with your database credentials

2. Set up Redis (Optional - for caching):
   - Install Redis from [redis.io](https://redis.io/download)
   - Start Redis server locally
   - Or use a cloud Redis service

3. Install Model Dependencies:
```bash
# Download required models
python scripts/setup/download_models.py

# Initialize services
python scripts/setup/init_services.py
```

### Individual Service Setup

#### Recommendation System
```bash
python scripts/train_recommendations.py
```

#### Content Generation
```bash
python scripts/setup_gpt.py
```

#### Image Processing
```bash
python scripts/setup_image_processing.py
```

## Theme Customization

### Theme Settings

The theme can be customized through the Shopify Theme Editor. Major customization options include:

- Color schemes
- Typography
- Header layouts
- Footer configurations
- Product grid layouts
- Button styles

### Featured Sections

#### Featured Products Grid
- Customizable grid layout (3x3 or 2x4)
- Optional featured large product
- Configurable number of products to display
- Optional "Buy Now" buttons
- Responsive design for all devices

#### Hero Banner
- Full-width design
- Customizable content
- Mobile-optimized layouts

#### Newsletter Popup
- Customizable timing and frequency
- Mobile-friendly design
- GDPR compliant

## Contributing

We welcome contributions! Please read our contributing guidelines before submitting pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Support

For support, please open an issue in the GitHub repository or contact our support team.

## Acknowledgments

- Built with Shopify Liquid
- Designed for modern e-commerce
- Optimized for performance and conversion
- Powered by open-source AI technologies

---

Made with ❤️ by Emmanuel Battle & The Battle IT Solutions' Team  