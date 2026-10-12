# Hi, I'm Kaan

BSc Computer Science and Engineering student at [Eindhoven University of Technology (TU/e)](https://www.tue.nl/en/), originally from Istanbul. I build AI systems end to end and ship them as real products: data pipelines, ML models, backend, frontend and the infra that keeps it all running.

I build solo with AI-assisted development (Claude Code): I design the system, make the calls and review and test what goes in.

Open to software and ML internships for summer 2027.

## What I'm building

### [Audience Labs](https://audiencelabs.net)

Clip automation for streamers. You paste a Twitch or Kick VOD link (or upload a file), the pipeline transcribes it with Whisper on GPU, adds speaker diarization and audio-emotion signals, and an LLM finds the moments worth posting. Each hook gets a virality score plus Hook / Flow / Value / Trend grades, then the app renders vertical clips with word-level animated captions and an optional on-screen hook, ready to review and schedule for TikTok, YouTube Shorts and Instagram Reels.

Next.js 16 dashboard, Python worker (yt-dlp, FFmpeg, faster-whisper, pyannote), Supabase for data and realtime, Cloudflare R2 for storage, Modal for GPU jobs. The app code is private; the scoring stage is open source as [clip-virality-scorer](https://github.com/kaankuzu1/clip-virality-scorer) and the [landing page](https://github.com/kaankuzu1/growthlanding) is public.

**Private beta, free and invite-only:** [request access at audiencelabs.net](https://audiencelabs.net/request-access)

<img src="assets/audiencelabs.png" alt="Audience Labs dashboard: a scored clip with editorial grades" width="850">

### [clip-virality-scorer](https://github.com/kaankuzu1/clip-virality-scorer)

The clip-ranking stage of Audience Labs, rewritten as a small standalone Python package. It takes candidate clips proposed by an LLM and ranks them by how likely they are to perform on short-form platforms: a heuristic score on top of the noisy LLM estimate, creator-normalised labels, and an optional XGBoost model once real engagement data exists. `pip install` it and run `clip-scorer rank` on the bundled example. Standard library only by default, tested with pytest, CI on GitHub Actions, MIT licensed.

## Before TU/e

Software team of FRC Team ROBIN (FIRST Robotics Competition), 2023 to 2025.

## Tools I use most

<img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,nodejs,nestjs,python,fastapi,pytorch,opencv,supabase,postgres,redis,docker" alt="TypeScript, React, Next.js, Tailwind, Node.js, NestJS, Python, FastAPI, PyTorch, OpenCV, Supabase, Postgres, Redis, Docker" height="40">

## Find me

[LinkedIn](https://www.linkedin.com/in/kaan-kuzu-012338292) · [X @kaankuzudev](https://x.com/kaankuzudev) · [audiencelabs.net](https://audiencelabs.net)
