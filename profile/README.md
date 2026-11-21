# Tube2Vid: the video downloader API for YouTube, TikTok, Instagram and 1,800+ sites

[Tube2Vid](https://tube2vid.com) downloads video, audio and images from YouTube, TikTok, Instagram, X, Facebook, Reddit, Pinterest, Vimeo, SoundCloud, Threads and 1,800+ other sites, and serves them as MP4, MP3 or image files. Everything you can do on the website is available through a REST API, so you can add a YouTube downloader, TikTok downloader or Instagram downloader to your own app, script or AI agent without running yt-dlp, ffmpeg, proxies or cookie jars yourself.

- **One API for every site.** Submit a URL, poll the job, get a short-lived signed download link.
- **No infrastructure.** Tube2Vid handles extractor updates, rate limits, retries and storage.
- **Pay per download.** Credits, not subscriptions. [Get an API key](https://tube2vid.com/pricing).
- **Watch it work.** [Live platform status](https://tube2vid.com/status) shows what is up, per site.

Read the [Tube2Vid API documentation](https://tube2vid.com/docs) to get started.

## Repositories

| Repository | What it is | Install |
| --- | --- | --- |
| [sdk](https://github.com/Tube2Vid/sdk) | TypeScript / JavaScript SDK | `npm install @tube2vid/sdk` |
| [sdk-python](https://github.com/Tube2Vid/sdk-python) | Python SDK | `pip install tube2vid` |
| [sdk-go](https://github.com/Tube2Vid/sdk-go) | Go SDK | `go get github.com/Tube2Vid/sdk-go` |
| [sdk-java](https://github.com/Tube2Vid/sdk-java) | Java SDK | `com.tube2vid:tube2vid-sdk` (Maven Central) |
| [sdk-dotnet](https://github.com/Tube2Vid/sdk-dotnet) | C# / .NET SDK | `dotnet add package Tube2Vid` |
| [sdk-php](https://github.com/Tube2Vid/sdk-php) | PHP SDK | `composer require tube2vid/sdk` |
| [sdk-ruby](https://github.com/Tube2Vid/sdk-ruby) | Ruby SDK | `gem install tube2vid` |
| [sdk-rust](https://github.com/Tube2Vid/sdk-rust) | Rust SDK | `cargo add tube2vid` |
| [sdk-swift](https://github.com/Tube2Vid/sdk-swift) | Swift SDK for iOS and macOS | Swift Package Manager: `https://github.com/Tube2Vid/sdk-swift` |
| [mcp](https://github.com/Tube2Vid/mcp) | MCP server for Claude, Cursor and other AI tools | `npx -y @tube2vid/mcp` |
| [cli](https://github.com/Tube2Vid/cli) | The `tube2vid` command-line downloader | `npm install -g @tube2vid/cli` |
| [api](https://github.com/Tube2Vid/api) | OpenAPI 3.1 spec and curl examples | [`openapi.yaml`](https://github.com/Tube2Vid/api/blob/main/openapi.yaml) |

## Quickstart with curl

```bash
curl -s https://tube2vid.com/v1/jobs \
  -H "authorization: Bearer $TUBE2VID_API_KEY" \
  -H "content-type: application/json" \
  -d '{"url":"https://www.youtube.com/watch?v=dQw4w9WgXcQ","format":"mp4"}'
```

Then poll `GET /v1/jobs/{jobId}` and fetch `GET /v1/jobs/{jobId}/download`. The [API reference](https://tube2vid.com/docs) has the full flow.

## Links

[Website](https://tube2vid.com) · [API docs](https://tube2vid.com/docs) · [Pricing](https://tube2vid.com/pricing) · [Status](https://tube2vid.com/status) · [Help](https://tube2vid.com/help)

All Tube2Vid SDKs and tools are open source under the MIT license. Please only download content you have the right to download.
