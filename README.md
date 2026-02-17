# Media Cutter Joiner

A web-based tool for cutting and joining media files (video/audio) built with Next.js.

## Features

- Upload media files
- Specify start and end times for cutting
- Process and download the cut segment
- Dummy implementation for demonstration

## Tech Stack

- **Frontend**: Next.js with TypeScript and Tailwind CSS
- **Backend**: Next.js API routes
- **Media Processing**: FFmpeg (simulated in dummy implementation)
- **Containerization**: Docker

## Getting Started

### Development

1. Install dependencies:
   ```bash
   pnpm install
   ```

2. Install additional media processing dependencies:
   ```bash
   pnpm run install-deps
   ```

3. Run the development server:
   ```bash
   pnpm dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

### Docker

Build and run with Docker:

```bash
docker build -t mediacutterjoiner .
docker run -p 3000:3000 mediacutterjoiner
```

## API

- `POST /api/process`: Upload a file with start and end times to process.

## Note

This is a sample implementation with dummy processing. In a real application, integrate FFmpeg for actual media cutting and joining.
