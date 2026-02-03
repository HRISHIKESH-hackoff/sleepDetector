# Alert Sounds Directory

## Audio Alert File

This directory contains the audio files used for the drowsiness detection alert system.

### Required Files

- **alert.mp3** - The audio alert sound that plays when drowsiness is detected

## Adding the Alert Audio

The alert sound referenced in the project is from:
- **Source:** YouTube Shorts - "Fahhh- sound effect (HD)"
- **URL:** https://youtube.com/shorts/TajAzT3CVJc?si=QpekO6AUVrIq6Pzl

### Steps to Add Audio

1. Download the audio from the YouTube source using a YouTube downloader tool
2. Convert the video to MP3 format if needed
3. Save it as `alert.mp3` in this directory
4. Ensure the audio file is properly compressed (recommended size: 20-100KB)

### Audio Requirements

- **Format:** MP3
- **Sample Rate:** 44.1 kHz or 48 kHz
- **Bit Rate:** 128 kbps (mono) or 192 kbps (stereo)
- **Duration:** 1-3 seconds recommended
- **Volume:** Normalized to -3dB to -6dB for optimal alert clarity

## Usage in Code

The audio is referenced in `Alert.tsx`:

```jsx
<audio
  ref={audioRef}
  src="/sounds/alert.mp3"
  loop={false}
  preload="auto"
  aria-label="Drowsiness detection alert"
  aria-hidden="false"
/>
```

The audio plays automatically when drowsiness is detected and stops when the driver becomes alert.

## Note

Make sure to respect copyright and licensing when adding audio files. The YouTube Shorts "Fahhh" sound effect appears to be a freely available sound effect suitable for this purpose.
