# aiden: open-source democracy

aiden is an AI-powered avatar chat interface that aims to revolutionize democratic engagement through open-source technology. It combines advanced language models, speech synthesis, and video generation to create an interactive digital representative.

*** MAIN PROJECT FILES HOSTED ON REPLIT ***

![3dneural.png](3dneural.png)

## 1-Click Fork and Deploy

1. Create and login to your Replit account and access the project page:

   [![Fork Repl](https://replit.com/badge/github/replit/replit.github.io)](https://replit.com/@5-DeeTV/aiden-final?v=1)

3. Click on the "Fork" button to duplicate the Repl into your account.

4. On the left side of the page, scroll down to the 'Secrets' tab and add the following API keys:

   - GROQ_API_KEY: [Get your API key here](https://console.groq.com/keys)
   - CARTESIA_API_KEY: [Get your API key here](https://play.cartesia.ai/console)
   - NEXT_PUBLIC_SUPABASE_URL: `https://xbcycvqsqguzliafhqrn.supabase.co`
   - NEXT_PUBLIC_SUPABASE_ANON_KEY: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhiY3ljdnFzcWd1emxpYWZocXJuIiwicm9sZSI6ImFub24iLCJpYXQiOjE3MjEzNzM1NDksImV4cCI6MjAzNjk0OTU0OX0.SB_cijxHsb970S7KHaGscmIXeZlsCK2NVkWB9R5yUoU`
   - SUPABASE_SERVICE_ROLE_KEY: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InhiY3ljdnFzcWd1emxpYWZocXJuIiwicm9sZSI6InNlcnZpY2Vfcm9sZSIsImlhdCI6MTcyMTM3MzU0OSwiZXhwIjoyMDM2OTQ5NTQ5fQ.KG21oblMIW_ZMuI8Lc-xN3EoeIlpqcKuC-x88bpLmlA`
   - NEXT_PUBLIC_SYNC_API_KEY: [Get your API key here](https://app.synclabs.so/keys)

5. Once your Secrets are stored, click the 'Run' button at the top of the page. After all necessary packages are installed, the application will open in the 'Webview' panel pop-up.

6. You now have 'aiden' working in production in your local Replit environment. You can interface with the app in one of three ways:
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

## Features

- Real-time speech-to-text transcription
- Advanced language model for generating contextual responses
- High-quality text-to-speech synthesis
- Lip-synced video generation
- Interactive chat interface
- Multi-language support

![image1.png](image1.png)

![image2.png](image2.png)

![image3.png](image3.png)

## State of the Art in Video Synthesis

The landscape of video synthesis has seen remarkable advancements in recent years:

1. **GAN-based Methods**: Generative Adversarial Networks have been pivotal in creating realistic video content, with models like StyleGAN-V achieving high-quality video generation.

2. **Diffusion Models**: Text-to-video models like Stable Diffusion Video have shown impressive results in generating video content from textual descriptions.

3. **Neural Rendering**: Techniques like Neural Radiance Fields (NeRF) have revolutionized 3D scene reconstruction and novel view synthesis.

4. **Lip Sync Technologies**: Advanced models can now generate highly realistic lip movements synchronized with audio, as demonstrated by tools like Wav2Lip and Sync Labs.

5. **Real-time Adaptation**: Recent advancements allow for real-time facial reenactment and expression transfer, enabling more interactive and responsive avatars.

Aiden leverages these cutting-edge technologies to create a seamless and engaging user experience.

## Technologies Used

- [Next.js](https://nextjs.org/) - React framework for the frontend
- [Groq](https://groq.com/) - Fast inference for transcription and text generation
- [Cartesia](https://cartesia.ai/) - Speech synthesis
- [Sync Labs](https://www.synclabs.so/) - Lip sync technology
- [Supabase](https://supabase.com/) - Database and storage solution
- [Replit](https://replit.com/) - Deployment and hosting platform

## Architecture Overview

![Architecture Diagram](image1.png)

The application follows a client-server architecture with several external service integrations. The frontend, built with Next.js, handles user interactions and audio/video playback. The backend processes user inputs, orchestrates external API calls, and manages data flow between services.

## Setup and Installation Guide

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

## Usage Instructions

1. Click the microphone button or type your question in the input field.
2. Aiden will process your input and generate a response.
3. The response will be synthesized into speech and a lip-synced video will be generated.
4. You can continue the conversation or ask new questions.

## Contributing

We welcome contributions to the Aiden project! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch: `git checkout -b feature-branch-name`
3. Make your changes and commit them: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature-branch-name`
5. Submit a pull request

Please read our [Contributing Guidelines](CONTRIBUTING.md) for more details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Balaji Srinivasan for the inspiring concept
- The teams at Groq, Cartesia, and Sync Labs for their cutting-edge APIs
- The open-source community for their invaluable tools and libraries
- Built using AI-NG's OS Project Swift (https://github.com/ai-ng/swift)

---

For more information, please visit our [website]([https://replit.com/@5-DeeTV/aiden-final?v=1]) or contact us at gratitude@5-dee.com.
