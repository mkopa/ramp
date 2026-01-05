# Refined Advanced Music Player

## Usage

```bash
# Play an audio file.
ramp /path/to/file

# Play an audio file and verify the decoded audio whilst playing (some formats only).
ramp --verify /path/to/file

# Seek the audio file to the desired timestamp and then play.
ramp -s <seconds> /path/to/file

# Play a specific track within the file.
ramp -t <track> /path/to/file

# Probe a file for streams and metadata (tags, visuals, etc.)
ramp --probe-only /path/to/file

# Decode and verify if the decoded audio is valid, but do not play it (some formats only).
ramp --verify-only /path/to/file

# Decode, but do not play or verify the decoded audio (benchmarking).
ramp --decode-only /path/to/file

# Do any of the above, but get the encoded audio from standard input by using '-' as the file path.
cat /path/to/file | ramp -
curl -s https://radio.station.com/stream | ramp -
youtube-dl -f 140 <url> -o - | ramp -
yt-dlp -f 140 <url> -o - | ramp -
```

## License

RAMP is provided under the MPL v2.0 license. Please refer to the LICENSE file for more details.