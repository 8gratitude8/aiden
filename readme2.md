# Aiden Installation Guide

Inspiration
Aiden was inspired by Balaji Srinivasan's visionary tweet:

"What if we could create an open-source AI version of a political candidate? Call it Aiden. Think of it as a digital avatar trained on a human's corpus, but voting on bills in real-time based on constituent feedback. It would be more accountable than a human politician." - @balajis

The project aims to bridge the gap between constituents and their representatives, enhancing democratic processes through the use of open-source digital avatars.
Features

Real-time speech-to-text transcription
Advanced language model for generating contextual responses
High-quality text-to-speech synthesis
Lip-synced video generation
Interactive chat interface
Multi-language support

Technical Foundations
Aiden leverages cutting-edge technologies in several key areas:
Language Models and Speech Synthesis

Utilizes transformer-based models for natural language processing
Employs end-to-end neural network-based text-to-speech (TTS) systems for natural-sounding speech

Video Generation and Lip-Sync Technologies

Implements Generative Adversarial Networks (GANs) for high-quality video synthesis
Uses deep learning models for accurate lip-sync, ensuring synchronization between audio and visual elements

Real-Time Interaction

Integrates advanced text-to-speech, facial animation, and natural language understanding systems
Optimizes for low-latency performance to maintain conversational pace

Architecture Overview
Aiden's system architecture is designed for modularity, scalability, and real-time performance. Key components include:

Natural Language Processing Engine
Machine Learning Models for Facial Animation
Speech Synthesis System
Integration and Communication Layer
Cloud-based Deployment with Edge Computing Capabilities

## 1-Click Fork and Deploy

1. Create and login to your Replit account and access the project page:
   [https://replit.com/@5-DeeTV/aiden-final?v=1](https://replit.com/@5-DeeTV/aiden-final?v=1)

2. Click on the "Fork" button to duplicate the Repl into your account.

3. On the left side of the page, scroll down to the 'Secrets' tab and add the following API keys:

   - GROQ_API_KEY: [Get your API key here](https://console.groq.com/keys)
   - CARTESIA_API_KEY: [Get your API key here](https://play.cartesia.ai/console)
   - NEXT_PUBLIC_SUPABASE_URL: `https://xbcycvqsqguzliafhqrn.supabase.co`
   - NEXT_PUBLIC_SUPABASE_ANON_KEY: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhiY3ljdnFzcWd1emxpYWZocXJuIiwicm9sZSI6ImFub24iLCJpYXQiOjE3MjEzNzM1NDksImV4cCI6MjAzNjk0OTU0OX0.SB_cijxHsb970S7KHaGscmIXeZlsCK2NVkWB9R5yUoU`
   - SUPABASE_SERVICE_ROLE_KEY: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhiY3ljdnFzcWd1emxpYWZocXJuIiwicm9sZSI6InNlcnZpY2Vfcm9sZSIsImlhdCI6MTcyMTM3MzU0OSwiZXhwIjoyMDM2OTQ5NTQ5fQ.KG21oblMIW_ZMuI8Lc-xN3EoeIlpqcKuC-x88bpLmlA`
   - NEXT_PUBLIC_SYNC_API_KEY: [Get your API key here](https://app.synclabs.so/keys)

4. Once your Secrets are stored, click the 'Run' button at the top of the page. After all necessary packages are installed, the application will open in the 'Webview' panel pop-up.

5. You now have 'aiden' working in production in your local Replit environment. You can interface with the app in one of three ways:
   - Speak your question
   - Type it out in the text field
   - Click on one of the 'Question Bubbles' provided

This will start the query and generation of the lip-synced video that will display in the 'VideoBox' component at the top of the page when finished rendering.

**Note:** Don't forget to click on the "ON" button on the 'VideoBox' component to ensure you can view and playback the finished video.

## Manual Setup and Installation

If you prefer to set up Aiden locally:

1. Clone the repository:
   ```
   git clone https://github.com/your-username/aiden.git
   cd aiden
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Set up environment variables:
   - Copy `.env.example` to `.env.local`
   - Fill in the required API keys and configuration values

4. Run the development server:
   ```
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) in your browser to see the application.

# Deepfakes Landscape & Architecture

## 4 Main Categories:

1. Voice Clones
2. Video Clones
3. Real-Time Video Clones
4. 3D Clones

## Landscape

### Voice Clones

#### Open Source:
- [VoiceVox](https://voicevox.hiroshiba.jp)
- [OpenVoice (myShell)](https://github.com/myshell-ai)
- [OpenVoice xtts (Coqui)](https://buff.ly/3TP7GpG)
- [Retrieval-based VC](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI)
- [Bark](https://github.com/suno-ai/bark)
- [VALL-E X](https://www.microsoft.com/en-us/research/project/vall-e-x/vall-e/)
- [Fish](https://github.com/fishaudio/fish-speech)
- [Parler](https://github.com/huggingface/parler-tts)
- [EmotiVoice](https://github.com/netease-youdao/EmotiVoice)
- [Mars5](https://huggingface.co/CAMB-AI/MARS5-TTS)
- [UltraVox](https://github.com/fixie-ai/ultravox)

#### Closed Source:
- [playHT](https://play.ht)
- [Cartesia](https://cartesia.ai)
- [Eleven Labs](https://elevenlabs.io)
- [Lepton AI](https://blog.lepton.ai/voice-mode-comes-to-lepton-llm-apis-a5ff3db8c7bf)
- [Sarvam AI](https://www.sarvam.ai)

### Video Clones

#### Open Source:
- [ReSyncer](https://guanjz20.github.io/projects/ReSyncer/)
- [V-Express](https://github.com/tencent-ailab/V-Express)
- [RadNeRF](https://me.kiui.moe/radnerf/)
- [MetaPortrait](https://meta-portrait.github.io)
- [DreamTalk](https://huggingface.co/papers/2312.13578)
- [Wav2lip++](https://github.com/Rudrabha/Wav2Lip)
- [Hallo](https://huggingface.co/spaces/fffiloni/tts-hallo-talking-portrait)
- [AniPortrait](https://github.com/Zejun-Yang/AniPortrait)
- [AniTalker](https://x-lance.github.io/AniTalker/)
- [EMO](https://humanaigc.github.io/emote-portrait-alive/)
- [GAIA (MSFT Version)](https://microsoft.github.io/GAIA)
- [VASA-1 (MSFT V2)](https://www.microsoft.com/en-us/research/project/vasa-1/)
- [SwapTalk](https://swaptalk.cc)
- [FaceFusion](https://github.com/facefusion/facefusion)
- [EDTalk](https://tanshuai0219.github.io/EDTalk/)
- [GMTalker](https://bob35buaa.github.io/GMTalker)
- [EmoSpeaker](https://peterfanfan.github.io/EmoSpeaker/)
- [EmoTalk](https://ziqiaopeng.github.io/emotalk/)

#### Closed Source:
- [Sync Labs](http://synclabs.so/)
- [Hedra AI](https://hedra.ai)
- [HeyGen](https://www.heygen.com)
- [Infinity AI](https://infinity.ai)
- [Captions AI](https://www.captions.ai/)
- [Argil AI](https://www.argil.ai)

### Real-Time Video Clones

#### Open Source:
- [Deep Live Cam](https://github.com/hacksider/Deep-Live-Cam)
- [Relightable Gaussian Codec Avatars](https://shunsukesaito.github.io/rgca/)

#### Closed Source:
- HeyGen (livestreaming)
- [Tavus](https://www.tavus.io)

### 3D Clones
- [ExAvatar](https://mks0601.github.io/ExAvatar/)
- [Real3D-Portrait](https://real3dportrait.github.io/?ref=aiartweekly)
- [Animatable Gaussians](https://animatable-gaussians.github.io)
- [Gaussian Shell Maps](https://rameenabdal.github.io/GaussianShellMaps/)
- [Gaussian Head Avatar](https://huggingface.co/papers/2312.03029)
- [Human 3Diffusion](https://yuxuan-xue.com/human-3diffusion/)
- [MonoGaussianAvatar](https://yufan1012.github.io/MonoGaussianAvatar)
- [3DGS-Avatar](https://neuralbodies.github.io/3DGS-Avatar/)

## Latest Research
- [Interactive Gaussian Codec](https://arxiv.org/abs/2407.10707)
- [GEA](https://3d-aigc.github.io/GEA/)
- [MeGA](https://conallwang.github.io/MeGA_Pages/)
- [ASH](https://bytez.com/read/cvpr/30029)
- [EVA (Expressive Gaussian Avatars)](https://evahuman.github.io)
- [NPGA (Neural Parametric Gaussian Avatars)](https://www.appypie.com/blog/npga-neural-parametric-gaussian-avatars)
- [FAGhead (Fully Animate Gaussian Head from monocular videos)](https://arxiv.org/abs/2406.19070)
- [PSAvatar (Point-Based Real-Time Head Avatar)](https://arxiv.org/abs/2401.12900)
- [SplattingAvatar](https://bytez.com/docs/cvpr/29974/paper)
- [Surfel](https://gs-ia.github.io)

## Fingerprinting
- [Avatar Fingerprinting](https://research.nvidia.com/labs/nxp/avatar-fingerprinting/)

# Aiden Usage Instructions and Technical Overview

## Usage Instructions

1. Click the microphone button or type your question in the input field.
2. Aiden will process your input and generate a response.
3. The response will be synthesized into speech and a lip-synced video will be generated.
4. You can continue the conversation or ask new questions.

## Technologies Used

- [Next.js](https://nextjs.org/) - React framework for the frontend
- [Groq](https://groq.com/) - Fast inference for transcription and text generation
- [Cartesia](https://cartesia.ai/) - Speech synthesis
- [Sync Labs](https://www.synclabs.so/) - Lip sync technology
- [Supabase](https://supabase.com/) - Database and storage solution
- [Replit](https://replit.com/) - Deployment and hosting platform

## Architecture Overview

The application follows a client-server architecture with several external service integrations:

- Frontend (Next.js): Handles user interactions and audio/video playback
- Backend: Processes user inputs, orchestrates external API calls, and manages data flow between services
- External APIs: Groq for language processing, Cartesia for speech synthesis, and Sync Labs for lip-sync video generation
- Database: Supabase for data storage and management

## Features

- Real-time speech-to-text transcription
- Advanced language model for generating contextual responses
- High-quality text-to-speech synthesis
- Lip-synced video generation
- Interactive chat interface
- Multi-language support

## State of the Art in Video Synthesis

Aiden leverages cutting-edge technologies in video synthesis:

1. **GAN-based Methods**: Using Generative Adversarial Networks for realistic video content generation.
2. **Diffusion Models**: Employing text-to-video models for generating video content from textual descriptions.
3. **Neural Rendering**: Utilizing techniques like Neural Radiance Fields (NeRF) for 3D scene reconstruction and novel view synthesis.
4. **Lip Sync Technologies**: Implementing advanced models for generating realistic lip movements synchronized with audio.
5. **Real-time Adaptation**: Incorporating real-time facial reenactment and expression transfer for interactive and responsive avatars.

These technologies combine to create a seamless and engaging user experience with Aiden.
