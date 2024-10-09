
---

# DocTalk - Medical Report Q&A App

## Overview

**DocTalk** is a web application designed to assist users in uploading medical reports (PDF or images) and extracting key information from them using advanced AI models. Users can ask questions about the reports and receive answers backed by an expert medical knowledge base. The app uses Google Gemini for AI vision tasks and Pinecone for retrieving relevant medical data.

## Key Features

- **Medical Report Upload**: Upload medical reports (PDF or image formats) and extract essential details.
- **AI-powered Q&A**: Ask questions about the medical report and get personalized responses using LangChain and Google Gemini AI.
- **Editable Report Data**: Users can edit the extracted data and input additional information such as patient symptoms, age, and gender.
- **Dark Mode**: The application supports dark mode for easier viewing during nighttime.
- **Mobile and Desktop Support**: The app is fully responsive and works well across desktop and mobile devices.
- **Streamed AI Responses**: Users receive real-time streaming answers from the LLM.

## Tech Stack

- **Frontend**: Next.js, TypeScript, TailwindCSS, ChatCNY for UI components
- **Backend**: API calls to Google Gemini AI and Pinecone
- **Database**: Pinecone for managing the medical knowledge base
- **AI/ML**: Google Gemini for vision tasks, LangChain for language model integration
- **Deployment**: Vercel

## How It Works

1. **Upload a Report**: Users can select and upload a medical report in image or PDF format.
2. **Data Extraction**: The app extracts key data from the report using Google Gemini Vision capabilities.
3. **Personalization**: The user can edit the extracted data, input patient symptoms, and correct any inaccuracies.
4. **Q&A**: Users can ask questions based on the report, and the system provides answers by querying Pinecone's knowledge base and generating a response through Google Gemini.
5. **Real-time Recommendations**: Get personalized medical insights like potential diagnoses, further tests, or expert recommendations.

## Installation and Setup

### Prerequisites
- Node.js
- NPM or Yarn
- Pinecone API key
- Google Gemini API key

### Steps

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/DocTalk.git
   ```

2. **Install dependencies**:
   ```bash
   cd DocTalk
   npm install
   ```

3. **Set up environment variables**:
   Create a `.env` file in the project root and add your API keys:
   ```bash
   NEXT_PUBLIC_GEMINI_API_KEY=your-gemini-api-key
   NEXT_PUBLIC_PINECONE_API_KEY=your-pinecone-api-key
   ```

4. **Run the development server**:
   ```bash
   npm run dev
   ```
   Open [http://localhost:3000](http://localhost:3000) to view the app.

## Usage

1. Upload a medical report (PDF or image).
2. Wait for the report to be processed and extracted.
3. Edit the extracted information if necessary (e.g., add patient symptoms, correct report details).
4. Ask questions related to the report and receive AI-powered responses in real-time.

## Future Enhancements

- **PDF Compression**: Client-side compression for PDFs will be implemented in the future to reduce file size without compromising on report extraction quality.
- **Enhanced Error Handling**: Provide detailed user feedback for API errors and file type validation.
- **Multiple Report Support**: Extend functionality to allow the upload of multiple reports simultaneously.

## Contributing

Feel free to submit issues or pull requests if you have ideas for improvements or encounter any bugs.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---