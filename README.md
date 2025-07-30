# EEG Simulator - Brain-Computer Interface Demo

A sophisticated brain-computer interface (BCI) simulator built with Next.js that demonstrates real-time EEG signal processing, emotion detection, and intent prediction. This application simulates the capture and analysis of electroencephalogram (EEG) data to predict user emotions and intentions, providing a comprehensive demonstration of modern BCI technology.

![EEG Simulator](public/placeholder.svg)

## 🧠 Features

### Core Functionality
- **Real-time EEG Simulation**: Generate realistic EEG signals with configurable parameters
- **Emotion Detection**: AI-powered emotion classification from simulated brain patterns
- **Intent Prediction**: Predict user intentions based on EEG data analysis
- **Brain State Visualization**: Interactive charts and real-time data visualization
- **Processing Pipeline**: Visual representation of the BCI data processing flow

### Advanced Features
- **AI-Powered Advisor**: Personalized wellness and productivity recommendations
- **Text-to-Speech**: Audio feedback for detected emotions and intents
- **PDF Report Generation**: Export comprehensive analysis reports
- **Signal Upload**: Import and analyze custom EEG data files
- **Auto Mode**: Continuous monitoring and analysis
- **Mood Journaling**: Track emotional states over time

### User Interface
- **Modern Design**: Clean, responsive interface built with Tailwind CSS
- **Dark/Light Themes**: Theme switching with next-themes
- **Interactive Components**: Rich UI components powered by Radix UI
- **Real-time Charts**: Data visualization with Recharts
- **Responsive Layout**: Optimized for desktop and mobile devices

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ 
- pnpm (recommended) or npm
- Modern web browser with JavaScript enabled

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd eeg-simulator
   ```

2. **Install dependencies**
   ```bash
   pnpm install
   # or
   npm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env.local
   ```
   Configure your Supabase credentials if using authentication features.

4. **Run the development server**
   ```bash
   pnpm dev
   # or
   npm run dev
   ```

5. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

## 🛠️ Technology Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **React 19** - UI library
- **TypeScript** - Type-safe development
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Headless UI component library

### Data & Visualization
- **Recharts** - Chart library for data visualization
- **jsPDF** - PDF generation for reports
- **React Hook Form** - Form handling with validation
- **Zod** - Schema validation

### Backend & Services
- **Supabase** - Backend-as-a-Service (optional for auth)
- **Web Speech API** - Text-to-speech functionality

### Development Tools
- **PostCSS** - CSS processing
- **ESLint** - Code linting
- **Geist Font** - Typography

## 📊 Project Structure

```
├── app/                    # Next.js App Router pages
│   ├── globals.css        # Global styles
│   ├── layout.tsx         # Root layout
│   ├── page.tsx          # Home page
│   └── auth/             # Authentication pages
├── components/            # React components
│   ├── ui/               # Reusable UI components
│   ├── bci-simulator.tsx # Main simulator component
│   ├── eeg-visualization.tsx # Data visualization
│   ├── ai-assistant.tsx  # AI advisor component
│   └── ...               # Other components
├── lib/                   # Utility libraries
│   ├── eeg-generator.ts  # EEG data simulation
│   ├── ai-advisor.ts     # AI recommendation engine
│   ├── signal-generator.ts # Signal processing
│   ├── brain-state-classifier.ts # ML classification
│   ├── pdf-generator.ts  # Report generation
│   ├── tts-engine.ts     # Text-to-speech
│   └── utils.ts          # General utilities
├── hooks/                 # Custom React hooks
├── public/               # Static assets
└── styles/               # Additional stylesheets
```

## 🎯 Usage

### Basic Operation

1. **Start Simulation**: Click "Start Processing" to begin EEG signal generation
2. **Monitor Data**: Watch real-time emotion and intent detection
3. **View Insights**: Get AI-powered recommendations based on brain state
4. **Export Reports**: Generate PDF reports of your session data

### Advanced Features

#### Custom Signal Upload
1. Click the "Upload Signal Data" button
2. Select a CSV file with signal data (one value per line)
3. The simulator will process your custom data

#### Auto Mode
- Enable continuous monitoring for long-term analysis
- Automatic emotion and intent detection
- Real-time AI advisor feedback

#### Audio Feedback
- Toggle text-to-speech for audio notifications
- Hear detected emotions and intents
- Accessibility-friendly operation

## 🔧 Configuration

### EEG Parameters

The simulator supports various configurable parameters:

- **Frequency Bands**: Alpha, Beta, Theta, Delta wave simulation
- **Noise Levels**: Adjustable signal-to-noise ratio
- **Sampling Rate**: Configurable data capture frequency
- **Electrode Channels**: Multi-channel EEG simulation

### AI Model Tuning

Customize the AI advisor behavior in `lib/ai-advisor.ts`:

```typescript
export const AI_CONFIG = {
  confidenceThreshold: 0.7,
  emotionWeights: { ... },
  intentMapping: { ... }
}
```

## 📈 Data Processing Pipeline

1. **Signal Generation**: Synthetic EEG data creation
2. **Preprocessing**: Noise filtering and normalization
3. **Feature Extraction**: Brain pattern analysis
4. **Classification**: Emotion and intent prediction
5. **Post-processing**: Confidence scoring and validation
6. **Output**: Real-time results and recommendations

## 🧪 Development

### Running Tests
```bash
pnpm test
# or
npm test
```

### Building for Production
```bash
pnpm build
pnpm start
```

### Code Quality
```bash
pnpm lint
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- EEG research community for scientific foundations
- Open-source contributors for essential libraries
- Brain-computer interface pioneers for inspiration

## 📞 Support

For questions, issues, or contributions:

- Create an issue on GitHub
- Check the documentation
- Review existing discussions

## 🔮 Future Enhancements

- [ ] Real hardware EEG integration
- [ ] Machine learning model training
- [ ] Multi-user session support
- [ ] Advanced signal processing algorithms
- [ ] Mobile application development
- [ ] Cloud-based data storage
- [ ] Integration with medical devices

---

**Disclaimer**: This is a simulation tool for educational and demonstration purposes. It should not be used for medical diagnosis or treatment decisions.
