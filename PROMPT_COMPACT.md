# Scripted Cinematic Drama — VideoExpress Workflow

A reusable workflow for producing scripted episodes in VideoExpress. Start a production chat with this playbook and provide the episode topic, full script, and character reference images.

## 1. Intake

Ask for any missing required inputs in one message:

- The episode topic or premise.
- The full episode script, pasted or attached. Accept it in labeled parts if needed and confirm the final part has arrived before locking the shot plan.
- A labeled reference image for each character whose appearance needs to stay consistent. Reuse existing references when the user identifies them. Ask for a missing or ambiguous image before generating shots that depend on it. Use images the user has permission to use.

Optional inputs include an episode title, aspect ratio, target runtime override, recurring locations, wardrobe notes, and US regional accent preferences. Default to landscape 16:9, cinematic photorealism, American English accents, and a finished runtime of 9–10 minutes (540–600 seconds). There is no workflow cap on cast size, script length, or words per line. If a field or model has a technical limit, divide the work into consecutive parts and retain every scripted beat.

## 2. Break down the supplied script

Use the script as the source of truth for scene order, story days, action, dialogue, narration, reveals, and ending. Preserve the written lines and their speaker assignments. Ask before changing the script when its natural runtime falls outside the target. Offer concrete options tied to the measured difference, such as adjusting scene pacing or approving a specific script revision.

Create a scene and shot plan before generation. For every scene, record story day and time, location, characters, wardrobe, relevant props, script beats, and estimated edited duration. Mark flashbacks and time jumps explicitly. An episode can take place in one day or span several days. Derive its timeline from the script.

Estimate spoken time at the intended delivery pace, including overlap where scripted. Budget separate time for visible action, reactions, and transitions. Sum the planned edited durations and reconcile them with the target. Choose clip lengths supported by the selected VideoExpress mode. Split long dialogue at natural sentence or clause boundaries across consecutive clips, preserving every word and the speaker's performance. Let the scene determine shot count and pacing.

## 3. Lock appearance, wardrobe, and voices

Create a continuity record for each recurring character with the supplied reference image, fixed facial features and hair, voice, wardrobe by story day or scene, and any scripted changes. Use the matching image in VideoExpress Consistent Character or another reference-image control exposed by the selected mode. For scenes with several characters, use the available reference slots and divide coverage into speaker close-ups, reactions, or other suitable shots when needed.

Keep each character recognizable across the episode. Use the same wardrobe throughout continuous action and across scenes on the same story day unless the script or activity calls for a change. Choose new attire for a new story day as appropriate, keeping face, hair, age, and build consistent. Carry established clothes into repeated views of the same moment, including flashbacks. Track changes to accessories, props, and character positions alongside wardrobe.

Use natural American English accents for dialogue and narration. Default to General American unless the user specifies a regional US accent. Keep each character's pitch, cadence, and vocal character stable across scenes. Use the assigned voice or a consistent voice description every time. Review each generated line for speaker, exact wording, accent, and lip sync.

## 4. Generate and verify shots

In VideoExpress, use the Cinematic Photorealistic image type when available. Use the original realistic workflow's Creative mode off setting when that control is present. Set the project and shots to the requested aspect ratio. Use the live interface to confirm available reference, duration, audio, and lip-sync controls. Keep public gallery sharing off. Recheck options after reopening the generation form.

Use a stable shot ID such as SC03-SH02. For each shot record script location, story day, wardrobe, reference images, starting pose, camera angle, intended action, speaker, exact lines, voice, and target edited duration. For a continuous cut, carry over screen direction, eyelines, prop placement, and the relevant pose or framing from the previous shot.

- **Start image prompt** — Cinematic photorealistic live-action look, natural skin texture, motivated lighting, chosen framing, matching cast references and story-day outfits, location, poses, eyelines, and props.
- **Motion and sound prompt** — Shot ID, camera and action, performance timing, assigned speaker and verbatim dialogue, American accent profile, ambience and scripted sound. Cue visible listeners to stay silent. Give dialogue and intentional reactions enough time to play naturally.

Generate the start image and verify faces and clothing before submitting video. Check that submission succeeded before retrying. Work scene by scene, retain the shot IDs and render status, and use the app's displayed queue limits. Review rendered shots against the script and continuity record. Replace unusable takes and reconstruct required beats with alternate shots if a generation fails. Surface unresolved gaps.

## 5. Assemble, check runtime, and export

Place approved clips on the timeline in script order. Close unintended gaps and trim accidental frozen frames, silent leads and tails, and camera settling. Preserve intentional pauses, reaction shots, transitions, narration, and complete lines. Check story-day changes, matching wardrobe, eyelines, sound transitions, accent consistency, and the final timeline duration. Resolve runtime mismatches with editorial pacing where possible and get approval for script revisions when needed.

Save and export the episode using the selected aspect ratio. For the default 16:9 workflow, use Full HD 1920 × 1080 MP4 when available. Verify the completed export and provide its link and actual duration. If VideoExpress cannot finish, report the specific blocker and retain the scene and shot plan and completed work so production can resume.

---

Workflow inspiration: [Realistic Mini Dramas by ai-playbooks](https://github.com/ai-playbooks/realistic-mini-dramas).
