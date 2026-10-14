4️⃣ **Your first conversation**
Once connected, try these in order:

> "Check SimpliGen status."
The agent uses `get_status` to check the engine, your cloud credit balance, and the active project.

> "What presets do I have that are ready to run locally?"
It uses `list_capabilities` to check available presets, required inputs, and local or cloud readiness.

> "Use SimpliGen to generate a moody rain-soaked street at night with the Krea 2 preset, 16:9."
It submits the job with `generate`, waits with `wait_for_result`, and retrieves the image with `get_result_image`.

> "Use SimpliGen to turn that into a 5-second video with MiniMax H3 Image to Video."
It uploads the image as a reference with `upload_file` and runs the video preset. The server returns the finished video's file path.

5️⃣ **What the agent can do**
- **Generate:** `list_capabilities`, `generate`, `get_job`, `wait_for_result`, `list_jobs`, `cancel_job`, `get_result_image`, `prepare_preset`, `list_loras`
- **Inputs and projects:** `upload_file` (images, video, audio), `list_projects`, `create_project`
- **Characters and products:** save, list and remove characters and products; generate character images, frames and videos
- **Recipes:** build, check, publish and run multi-step recipes, and follow their runs
- **Engine:** `start_engine`, `stop_engine`, `restart_engine`

6️⃣ **Tips that save time**
- **Name SimpliGen in your request.** "Use SimpliGen to…" makes your intended tool clear.
- **Specify your options.** App slider defaults aren't applied through MCP. Include duration, aspect ratio, resolution, or other required settings.
- **Check timed-out jobs before retrying.** A wait timeout doesn't necessarily mean the render failed. Ask the agent to check `get_job` before submitting another render.
- **List capabilities before choosing a preset.** IDs can look like `anime-pack:anime-hassaku`. Let the agent read the actual list.
- **Use SimpliGen projects.** "Create a SimpliGen project called Poster Concepts and put the next renders in it."
- **Set a cloud spending rule.** "Tell me the credit cost and ask before running anything in the cloud."
- **Open the file path to see a picture.** Gemini CLI passes the image to the model but shows only a short summary in the terminal. The original output path is in the reply.
- **Approvals.** Gemini CLI asks before each tool call. Once you trust the setup, you can mark the server as trusted in its config.

7️⃣ **More presets to try**
Look for packs beginning with `Community —` in the SimpliGen Store, including MiniMax H3, LTX 2.5, Wan 2.2, Krea 2, Qwen Image 2.1, Flux, and SDXL. Full catalogue and manual downloads: <https://github.com/michaeldune/simpligen-presets#readme>
Installed presets appear in `list_capabilities`, where the agent can check their requirements and readiness.

🆘 **Troubleshooting**
- **The agent can't find SimpliGen tools:** check that SimpliGen is open, Node.js is installed, the token is configured, and the entry is in the right file for your app (see Part One). Restart the agent, and in Gemini CLI check `/mcp`.
- **engineRunning: false:** the local engine may still be starting. Wait briefly and check again.
- **A preset won't run locally:** ask the agent to check `localReady` and identify missing requirements. Install the required models through SimpliGen or the pack's installer.
- **A wait times out:** check the existing job with `get_job`. It may still be rendering.
- **Authentication fails:** confirm the configured token matches the current SimpliGen pairing token. If it was revoked or replaced, update the configuration and restart.

Questions and results welcome below. 🙌
