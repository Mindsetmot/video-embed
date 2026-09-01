# YouTube Video Embed

"video-embed" is a simple standalone HTML page for embedding and displaying YouTube videos in a fullscreen iframe. The video URL can be provided dynamically through the "?url=" query parameter.

# ✨ Features

- 🎬 Display YouTube videos using an iframe.
- 🔗 Accept video URLs through the "?url=" query parameter.
- 🔍 Automatically extract the YouTube Video ID from the provided URL.
- 📺 Supports multiple YouTube URL formats:
  - "youtu.be"
  - "youtube.com/watch?v="
  - "youtube.com/embed/"
  - "youtube.com/shorts/"
  - "youtube.com/live/"
- 📱 Fully responsive and fills the entire screen.
- ⚫ Black background with no scrollbars.
- ❌ Displays an error message when the provided URL is invalid.
- 🖥️ Supports fullscreen playback.

# 🚀 Usage

Open the page and provide a YouTube URL through the "url" query parameter:

https://mindsetmot.github.io/video-embed?url=youtu.be/VIDEO_ID

For example:

https://mindsetmot.github.io/video-embed?url=youtu.be/dQw4w9WgXcQ

The page extracts the "VIDEO_ID" and converts it into a YouTube embed URL:

https://www.youtube.com/embed/VIDEO_ID

You can also use other supported YouTube URL formats:

https://mindsetmot.github.io/video-embed?url=www.youtube.com/watch?v=VIDEO_ID

# 🔧 How It Works

1. JavaScript reads the "url" parameter using "URLSearchParams".
2. The "getYoutubeId()" function checks the URL against several supported YouTube URL patterns.
3. If a valid Video ID is found, it is assigned to the iframe's "src".
4. The video is displayed through the YouTube Embed Player.
5. If the URL does not match any supported format, an invalid URL message is displayed.

# 📁 File Structure

index.html

The file is completely standalone and does not require any external JavaScript libraries, frameworks, or additional files.

# ⚙️ YouTube Embed Parameters

The YouTube player is loaded with the following parameters:

autoplay=0
rel=0
modestbranding=1

This keeps autoplay disabled, limits related videos, and uses a more minimal YouTube branding configuration.

# 📝 Default Video

If no "url" parameter is provided, the page falls back to a default YouTube URL defined in the JavaScript code.

Simply opening:

https://mindsetmot.github.io/video-embed

will load the default video.
