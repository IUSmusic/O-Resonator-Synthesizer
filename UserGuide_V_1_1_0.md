# O RESONATOR
**Professional User Guide, Tutorial and FAQ**
**Version 1.1.0 - MAIN, COUPLING and OUTPUT pages**
IUS Music - Research prototype documentation

# Contents
- 1. What O Resonator is
- 2. What changed in v1.1.0
- 3. Core idea: strings, flywheel and body
- 4. The three-page interface
- 5. Quick start tutorials
- 6. MAIN page control reference
- 7. COUPLING page control reference
- 8. OUTPUT page control reference
- 9. Meters, graphs and live readouts
- 10. Recommended starting settings
- 11. Recording workflow
- 12. FAQ
- 13. Rights and credits

# 1. What O Resonator is
O Resonator is a minimalist electronic rotating string-body instrument, standalone host and audio effect. Its visual and sonic model is a black circular disk containing seven internal concentric string rings. Each ring has an electronic input path. When a ring is active, that path opens and the string contributes to the shared resonant body.

O Resonator does not behave like a normal note-triggered synth, arpeggiator, sequencer, plucked string, or clock-hand trigger wheel. The flywheel does not strike or pluck the strings. It continuously shapes active string paths through motion, pressure, inertia, damping, brightness and body resonance.

## What it is not
- Not a plucked string instrument by default.
- Not an arpeggiator or step sequencer.
- Not a radial spoke or clock-hand trigger system.
- Not a bridge, grip, latch or external contact mechanism.
- Not a synth that generates random notes from rotation alone.

## Operating modes

| Mode | Use |
| --- | --- |
| Standalone host | Runs O Resonator as a self-contained application with audio device controls and optional internal excitation. |
| VST3 effect | Processes external audio through active resonant rings. |
| VST3 instrument | Provides an instrument-style version for host workflows that need an instrument plug-in. |

# 2. What changed in v1.1.0
Version 1.1.0 expands the original guide to match the current three-page O Resonator interface and the latest release behaviour. The focus is still the same rotating seven-ring resonator, but the interface now separates performance, physical coupling and final output tools.

- New three-page structure: MAIN, COUPLING and OUTPUT.
- Engine On added as the global audio engine power control.
- Disk On clarified as the motion-physics control, not a total mute.
- Clock Host replaces the older Host Sync label.
- Internal Exciter replaces the older Internal Sustain label.
- Motion Coupling page added for slip, friction, radius bias, Doppler and body field behaviour.
- OUTPUT page added for Final EQ, Output Guard, final meters and Record Output.
- DAW-style recording waveform lane added for visual feedback during standalone recording.
- Dropdown menu theme and final layout spacing refined for consistency.
- Live readouts and tables remain data-based, not decorative placeholders.

# 3. Core idea: strings, flywheel and body
## Seven string rings
The instrument contains seven internal string rings. In engine order they are:

In the visualiser and resonator bank, the outside-to-inside order is:

The strings are concentric rings, not radial spokes. Active rings contribute to one shared resonant body. They do not play one after another unless you deliberately automate activation or note assignment.

## Activation model
Activating a ring opens its input path smoothly. Deactivating a ring closes the path and lets the ring fade or damp away while other active strings continue. Changing active strings should feel like tonal arrival or removal, not a pluck.

## Standalone signal flow
## Effect signal flow
In effect mode, no external input means there is no main processed sound unless Internal Exciter is explicitly enabled. Input plus no active strings should be silent or nearly silent because all string paths are closed.

# 4. The three-page interface
The v1.1.0 interface is organised into three pages. The pages share the same black, grey, white, dark red and dark blue visual language. Global controls remain visible so the instrument feels continuous across pages.


| Page | Purpose |
| --- | --- |
| MAIN | Performance page for rings, input, primary motion, resonator bank, waveform monitors and core output level. |
| COUPLING | Physical motion page for disk and string coupling, slip, friction, radius weighting, Doppler and centre body field. |
| OUTPUT | Final shaping page for Final EQ, Output Guard, final meters, recording and output status. |

## Global controls

| Control | Meaning |
| --- | --- |
| Engine On | Turns the O Resonator audio engine on or off. Engine Off should fade O Resonator output safely to silence. |
| Disk On | Starts or stops rotating motion physics. Disk Off stops rotation, slip friction and Doppler movement, but static resonator processing may still pass audio if Engine On is active. |
| Clock Host | Uses host tempo when available. Disable it for internal free-running speed. |

## Engine On versus Disk On
Engine On is the overall audio power for O Resonator. Disk On is the motion source. This separation lets the user design a static resonator tone with Disk Off, or silence the whole O Resonator output with Engine Off.

# 5. Quick start tutorials
## A. Create a dark drone
- Open the MAIN page.
- Turn Engine On.
- Activate D2 and A3.
- Turn Disk On.
- Set Sustain Feed to a medium value.
- Raise Pressure until the tone blooms.
- Set Flywheel to a medium value.
- Increase Inertia for slower, heavier motion.
- Use Body Move and Damping to refine the body.
- Set Master to a safe output level.

Expected sound: a continuous dark drone that blooms into motion. It should not tick, pluck or play a sequence.

## B. Process external audio
- Insert the VST3 effect on an audio track.
- Send voice, guitar, synth, drums or field recording into the plug-in.
- Turn Engine On and activate one or more rings.
- Raise Input Gain and Pressure carefully.
- Increase Input Isolation for stronger transformation.
- Set Mix to taste.
- Use OUTPUT page meters to confirm input and final output levels.

## C. Shape physical slip
- Open the COUPLING page.
- Set Coupling Mode to Slip.
- Lower String Coupling to increase disk-string relative motion.
- Raise Slip Amount and Friction gradually.
- Use Radius Bias to make outer rings respond more strongly.
- Add Doppler subtly for rotating pitch and stereo motion.

## D. Finish and record a sound
- Open the OUTPUT page.
- Enable Final EQ and shape the tone.
- Enable Output Guard and set a safe Ceiling.
- Watch the Final Meters and gain-reduction display.
- Press Record Output in standalone mode.
- Stop recording when finished and check the saved file status.

# 6. MAIN page control reference
## Disk and transport

| Control | Function |
| --- | --- |
| Engine On | Global audio engine on or off. Use this to silence or activate O Resonator output. |
| Disk On | Starts or stops flywheel and motion physics. |
| Clock Host | Locks rotation to host tempo when available. |
| Speed | Internal rotation rate when free-running. Higher values increase modulation speed and motion intensity. |
| Time Mapping | Chooses how musical time maps to disk motion. |
| Reset | Controls phase reset behaviour. It resets motion, not notes. |
| Phase | Offsets circular modulation phase. |
| Direction | Reverses motion direction without creating a melody. |

## Ring selection and activation

| Control | Function |
| --- | --- |
| Harmony | Selects a preset ring combination or manual control. |
| String activation buttons | Open or close the seven ring paths. |
| Note assignment | Retunes or fingers active paths. Closed rings should not sound from MIDI alone. |

## Motion and evolution

| Control | Function |
| --- | --- |
| Rise | Adds rotational growth energy. |
| Flywheel | Controls how strongly motion shapes active string paths. |
| Inertia | Controls how slowly the flywheel responds. |
| Evolution | Selects long-term movement shape such as rise, wave, freeze or random walk where available. |
| Mod Depth | Sets overall evolution and modulation amount. |
| Period | Sets the duration of the evolution cycle. |
| Motion Drift | Adds rotation-linked timbre drift without becoming a trigger. |

## String energy and response

| Control | Function |
| --- | --- |
| Pressure | Main drive into active strings. |
| Sustain Feed | Continuous energy floor for active strings. |
| String Sustain | Controls how long string energy remains. |
| Rub Energy | Adds continuous rub-like support. |
| Bend | Adds tension or deflection behaviour to active strings. |
| Harmonics | Increases overtone emphasis. |
| Damping | Restrains ring time and brightness. |
| Bright Move | Adds brightness movement. |
| Input Response | Controls input and activation smoothing. |

## Input and body

| Control | Function |
| --- | --- |
| Input Gain | Controls external audio entering the resonant paths. |
| Input Isolation | Increases focus on processed ring output. |
| Mix | Blends processed output and original input. |
| Internal Exciter | Optional internal source for auditioning the resonator when external input is not present. |
| Body Move | Controls body resonance movement and density. |
| Body Grit | Adds optional saturation and roughness. |
| Texture | Adds subtle friction colour. Use carefully. |
| Width | Adds stereo spread or phase movement. |
| Quality | Adjusts processing quality and CPU use. |
| Oversampling | Improves high-energy processing at higher CPU cost. |

# 7. COUPLING page control reference
The COUPLING page models the relationship between the rotating disk and the string rings. It is optional. Locked behaviour preserves the original smooth rotating-body sound. Slip and orbital-style settings add friction, radius weighting, Doppler and centre-field effects.


| Control | Function |
| --- | --- |
| Coupling Mode | Selects Locked, Slip or Orbital-style motion behaviour. |
| String Coupling | How much strings follow disk rotation. Low values mean more slip and friction. |
| Slip Amount | How much relative disk-string motion becomes energy. |
| Radius Bias | How strongly outer rings receive more surface motion. |
| Friction | Amount of relative motion converted into resonator excitation. |
| Surface | Smooth to rough surface character. |
| Pressure Link | How strongly Pressure affects friction energy. |
| Noise Texture | Filtered roughness added to continuous friction. |
| Doppler | Amount of micro pitch and motion shift from rotation. |
| Trajectory | Movement interpretation such as circular, elliptic or drift where available. |
| Stereo Orbit | How much coupling motion moves across stereo space. |
| Phase Spread | Phase difference across rings and channels. |
| Body Field | Neutral, Heavy or Radiant centre-field behaviour. |
| Field Strength | How strongly the centre body affects ring energy. |
| Field Damping | How much the centre absorbs motion. |
| Radiance | How much energy spreads outward from the centre. |

## Physical meaning
In Slip mode the disk can move while the string rings resist full rotation. Relative velocity increases with radius, so outer rings can receive stronger surface energy than inner rings. This creates friction, shimmer and Doppler without introducing plucks or random triggers.

# 8. OUTPUT page control reference
The OUTPUT page is the final shaping, protection, monitoring and recording page. It should be used after the core resonator sound has been created on MAIN and physically shaped on COUPLING.

## Final EQ

| Control | Function |
| --- | --- |
| EQ On | Enables the final tone-shaping EQ. |
| Low Cut | Removes unwanted low-frequency rumble. |
| Low Gain | Boosts or reduces low body tone. |
| Mid Freq | Sets the centre frequency of the mid bell. |
| Mid Gain | Boosts or reduces the selected mid area. |
| Mid Q | Controls mid band width. |
| High Gain | Boosts or reduces brightness and air. |
| High Cut | Controls high-frequency rolloff. |

The EQ curve display is parameter-derived. It should update when EQ settings change.

## Output Guard

| Control | Function |
| --- | --- |
| Guard On | Enables final output protection and isolation assistance. |
| Ceiling | Sets maximum output ceiling. |
| Drive | Pushes the resonator into the guard for stronger focused output. |
| Release | Controls limiter recovery speed. |
| Isolation | Focuses processed resonator output and reduces unwanted dry bleed. |

The gain-reduction meter should move only when the guard is actually reducing output.

## Record Output

| Control or display | Function |
| --- | --- |
| Record Output | Starts recording the final heard output in standalone mode. |
| Stop | Stops recording and closes the file safely. |
| Time | Shows elapsed recording time. |
| Last File | Shows the most recent saved file where available. |
| Recording waveform lane | DAW-style lane showing the same final output being written to disk. |

Recording should capture the final output after Final EQ, Output Guard and Master. The preferred format is 32-bit float WAV at the current playback sample rate.

## Final meters and master status

| Readout | Meaning |
| --- | --- |
| Input | Incoming signal level. |
| Post EQ | Signal level after Final EQ. |
| Guard Reduction | Amount of gain reduction from Output Guard. |
| Final Output | Final signal leaving O Resonator. |
| Signal flow | Shows active stages: Input, Rings, Body, Space, EQ, Guard, Master, Record. |

# 9. Meters, graphs and live readouts
O Resonator uses live readouts to make the signal path visible. A display that looks like data should reflect a real processor value, buffer, parameter or derived estimate.


| Display | Source |
| --- | --- |
| Polar graph | Active rings, shared disk phase, energy, decay and motion state. |
| Resonator bank | Seven live ring rows with note, frequency, energy, damping and state. |
| Input Wave | Incoming audio scope buffer. |
| Output Wave | Processed output scope buffer. |
| Modulation cards | Real parameter values and parameter-derived curve shapes. |
| Coupling graph | Slip, radius, Doppler and body-field parameter states. |
| Output analyser | Input trace, EQ curve, guard activity and final output trace. |
| Recording waveform lane | Final output signal being recorded. |

If Input Wave is moving but Output Wave is not, check that at least one string is active and that Engine On, Mix, Master, Input Gain and Output Guard settings allow signal through.

# 10. Recommended starting settings
## Clean dark drone

| Setting | Value |
| --- | --- |
| Active rings | D2 and A3 |
| Engine On | On |
| Disk On | On |
| Speed | 120 BPM |
| Flywheel | 45 percent |
| Inertia | 60 percent |
| Sustain Feed | 55 percent |
| Pressure | 45 percent |
| String Sustain | 90 percent |
| Texture and Body Grit | 0 percent |
| Output Guard | On with safe ceiling |

## Slip friction texture

| Setting | Value |
| --- | --- |
| Active rings | G2, C3 and A3 |
| Coupling Mode | Slip |
| String Coupling | 30 to 50 percent |
| Slip Amount | 20 to 45 percent |
| Friction | Low to medium |
| Surface | Low for smooth, higher for rough |
| Doppler | Subtle |
| Output Guard | On |

## External input processor

| Setting | Value |
| --- | --- |
| Mode | VST3 effect |
| Input Gain | Raise until Input Wave moves |
| Input Isolation | Medium high |
| Internal Exciter | Off unless auditioning |
| Mix | Taste |
| Active rings | One to three rings |
| Final EQ | Use after the resonator body is balanced |

# 11. Recording workflow
Record Output is intended mainly for standalone mode. In a DAW, the host can already record the plug-in output, so the internal recorder may be optional or disabled depending on build behaviour.

- Open the OUTPUT page.
- Confirm Engine On is active and the Final Output meter is moving.
- Set Final EQ and Output Guard before recording.
- Press Record Output.
- Watch the DAW-style waveform lane fill in real time.
- Press Stop when finished.
- Check Last File and confirm the saved recording location.

# 12. FAQ
### Why is there no sound?
Turn Engine On, activate at least one ring, confirm audio input where relevant, then raise Input Gain, Pressure, Sustain Feed and Master carefully.

### What is the difference between Engine On and Disk On?
Engine On controls whether O Resonator produces output. Disk On controls rotating motion physics. Disk Off stops motion effects, but a static resonator may still pass audio if Engine On remains active.

### Why does MIDI not play closed strings?
Closed strings have closed input paths. MIDI can retune or shape active strings, but it should not arm inactive rings by itself.

### Is the moving mark a pluck point?
No. It is a motion and energy indicator. The flywheel shapes active strings continuously; it does not strike them.

### What does COUPLING add?
It adds optional disk-string relationship controls such as slip, friction, radius bias, Doppler and body field behaviour.

### What does OUTPUT add?
It provides final tone shaping, protection, recording, final meters and output status.

### Why does it sound too bright?
Lower Pressure, Bright Move, Harmonics, Texture, Body Grit and High Gain. Increase Damping or use High Cut.

### Why does it feel too static?
Increase Flywheel, Mod Depth, Motion Drift, Body Move, Slip Amount, Doppler or Radiance depending on page and sound goal.

### Why does it feel too jumpy?
Increase Inertia and Input Response smoothing. Reduce Mod Depth, Friction, Surface, Noise Texture and fast reset settings.

### Are the table and visual meters real?
They are intended as live readouts connected to processor state, buffers, parameters or documented estimates. If a meter looks wrong, check the signal path and build version.

# 13. Rights and credits
O Resonator, formerly developed under the Code O design name, is a research and demonstration instrument created by Pezhman Farhangi under the IUS Music brand. The included software and documentation are provided for study, teaching, technical explanation, research demonstration and discussion.

No commercial license, trademark license or permission to create derivative instruments is granted by this document. Refer to the rights and use notice included in the application and repository for the complete terms.

IUS Music, IUS and I/US Music identify the performing name and brand for works released under the IUS Music brand. Copyright 2026 Pezhman Farhangi. All rights reserved.
