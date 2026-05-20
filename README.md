# acrux-ffmpeg-prebuilts

Public release-only repo holding prebuilt static **ffmpeg libs**
(LGPLv3, mux+RTMP+OpenSSL, no encoders) consumed by Acrux's
`build.rs` to skip the 15-minute ffmpeg-from-source compile.

These are **build-time inputs only** — the libs get statically
linked into the Acrux binary at compile time, so they never ship to
end users.

Refresh recipe: see `app/src-tauri/tools/build-ffmpeg-prebuilt.md`
in the main Acrux repo.

Release tags follow the ffmpeg version they were cut from:
`ffmpeg-prebuilt-v8.1.0`, `ffmpeg-prebuilt-v8.2.0`, etc.
