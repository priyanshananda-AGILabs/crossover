# Cursor prompt: generate or re-record the Fraction Studio demo video

You are helping me create a 3-5 minute product design assessment demo video.

Use the local prototype folder named `fraction_mvp_prototype`.

Open:

```text
fraction_mvp_prototype/index.html?demo=1
```

Record a browser walkthrough at 1280x720 or 1920x1080. Use the voiceover script in `demo_walkthrough_script.txt`.

Show these flows in order:

1. Start screen: emphasize private algebra-readiness framing, not elementary remediation.
2. First comparison problem: show the student can begin immediately.
3. Correct answer feedback: show lightweight confirmation and momentum.
4. Same-numerator wrong answer: intentionally choose the wrong option.
5. Strategy card: show the type-specific explanation and visual model.
6. Paired retry: answer the follow-up problem correctly.
7. Adaptive note and skill panel: show that the app is adjusting based on performance by type.
8. Benchmark comparison: show a different visual model, ideally a number line.
9. Summary screen: show private evidence of progress and completion.

Tone and pacing:

- Calm, professional, product-design oriented.
- No music, cartoons, flashy transitions, or gamified effects.
- Keep the framing focused on user empathy, design tradeoffs, and MVP scope.
- Avoid saying the app is for 4th grade or elementary math in the student-facing walkthrough.

If direct screen recording is available:

- Use the browser, microphone, and built-in screen recording.
- Export as `fraction_studio_demo_video.mp4`.

If direct screen recording is not available:

- Write a Playwright script that opens `index.html?demo=1`, clicks through the states listed above, and captures screenshots.
- Write an ffmpeg script that stitches the screenshots into an MP4 with captions and the voiceover script as narration or text overlays.
- Export the final file as `fraction_studio_demo_video.mp4`.

Final check before export:

- The video is between 3 and 5 minutes.
- The prototype shows wrong-answer feedback and paired retry.
- The video explains why the design avoids public leaderboards, childish visuals, harsh red-X feedback, and timed pressure in the MVP.
