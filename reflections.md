> >### module2 description
> >module2.js is logical comparator. It takes signal inputs in Inputs 1 & 2, and outputs the Max, Min, Mix of the two signals out Outputs 1, 2, 3, respectively.
> 
> >- Inputs: IN1, IN2
> >- Outputs: OUT1, OUT2, OUT3
> 
> >## Score:
> 
> >Build a rhythmic pattern using the highlighted controls - culminating in noise morphing into tone.
> 
> A low winding sound pulsates in the left. 3 or so pulses of that winding sound begin prior to a slowly alternating low reverberation pulsates on the right.  As they slowly rise in amplitude, period after period, 19 seconds in, appears a sort of chime on the right, blending in with the reverb.  That chime gets louder, but its pitch changes back to a lower reverb, but still with higher amplitude.
> 
> ><img src="https://i.imgur.com/PRBBGu9.png">
> 
> >Lfo-1 freq results in speed changes.<br/>
> 
> For at least the first minute (~60s) you don't really notice any speed changes.  This doesn't seem to happen until about ~82s into the recording.
> 
> >The left random rate results in “aftershocks” of rhythmic content.<br/>
> 
> The aftershocks heard are slightly unpleasant, but yet keeps you on the edge of your seat waiting to hear if they sharpen out their surrounding noise,  A noise, mind you, that sounds like you should be constantly on alert to lower your volume in case in clips out of control and pops your speakers!
> 
> At ~49 seconds in, the aftershock started to sound more like a smashing sound. My partner sitting beside me, reading, hears this and shouts: "Atari Pole Position!"
> 
> >[Pole Position (Wikipedia)](https://en.wikipedia.org/wiki/Pole_Position)
> 
> ~82 seconds in, and the speed begins to increase.  ~10s after that, the volume increases, making the messy aftershock sound even more messy with surrounding noise.
> 
> >VCF freq results in higher overtone-like content
> 
> 
> ---
> 
> #### Initial Patch Parameters
> *(file: patch.vcv)*<br />
> 
> Module | Control | Value | Type |
> ------ | ------- | ----- | ---- |
> LFO-1  |  FREQ   | 0.35306| attenuator knob |
> Random (L) |  RATE   | 0.002 | slider |
> VCF    |  FREQ   | 87.206| attenuator knob |
> 
> ---
> 
> #### First Edit Experiment
> *(file: patch.vcv)*<br />
> 
> Module | Control | Value | Type |
> ------ | ------- | ----- | ---- |
> LFO-1  |  FREQ   | <mark>0.047663</mark> | attenuator knob |
> Random (L) |  RATE   | <mark>1.7907</mark> | slider |
> VCF    |  FREQ   | <mark>8.1758</mark> | attenuator knob |
> 
> This edit attempts to slow down LFO frequency, that results into an elongated aftershock sound (approx. ~22s apart).
> 
> ![VCF Setting](https://i.imgur.com/GuDCuZh.png)
> ![Random Rate](https://i.imgur.com/We3OF0H.png)
> ![LFO-1 Frequency](https://i.imgur.com/bgmG4QV.png)
> 
> ---
> 
> #### Second Edit Experiment
> *(file: patch.vcv)*<br />
> 
> Module | Control | Value | Type |
> ------ | ------- | ----- | ---- |
> LFO-1  |  FREQ   | <mark>0.047663</mark> | attenuator knob |
> Random (L) |  RATE   | <mark>1.7907</mark> | slider |
> VCF    |  FREQ   | <mark>8.1758</mark> | attenuator knob |
> 
> ---
> 
> #### Happy Accidental Trip
> 
> ![Happy Accidental Trip](https://i.imgur.com/huYLC1B.png)
> 
> The above screenshot shows an amendment to patch.vcv that seems to generate a slow sweeping rise and fall sound while generating little blips (which I can only imagine is derived from the random generators' STEP output).  Those blips have a slight echo around them, giving them a pleasant, yet glitchy digital sound.  Would these be called timbres?
> 
> ---
> 
> #### Ring the Alarm
> 
> _Highlighted in blue are the LFO-1 and SEQ-3 modules.  Use the FREQ and STEPS knobs (respectively) to alter the siren._
> 
> ![Ring the Alarm](https://i.imgur.com/WAVyhMN.png)
> 
> Siren sound is the base of this patch.  With MIDI-CV module part of the flow, use keyboard to alter the siren and create your own alarm sounds.
> 
> Increase the frequency of the LFO-1 module to shorten the alarm time span.  An identifiable range for this would be keeping the knob between 9 o'clock (0.047663 Hz) and 12 o'clock (2.0125 Hz).
> 
> Turn on the sequencer module (SEQ-3) for further play.  Change the STEPS knob, to give a "gear changing" effect to the alarm sounds.
> 
> ---
> 
> #### Third Improvisation
> 
> ![Third Improvisation](https://i.imgur.com/vhRjtia.png)
> 
> Came across an issue attempting to create a recording, that didn't take into account the use of the sequencer in the performance.  A cable was not set to the recording module to incorporate the sequencer sounds.  To fix this, CH 1 (MIXER) -> L/MON (REC) cable was removed, and instead added a MIX (MIXER) -> L/MON (REC) cable.
> 
> The purpose of this improvisation was to attempt using the sequencer STEPS knob as the main melody changer int he performance.  Next steps could include controlling the FREQ values of both LFO-1 and VCF from the sequencer.
> 
> ---

## Listening to recording

It starts with a very low sound that goes fora second or so and then a much higher pitch sound starts. It has a lot fo reverb and because it doesn't have many layers of sound, I can concentrate in each sound. I found it very meditative. 
It reminds me of the sound of tibetan bowls. 
I put in a loop and it goes almost as a continuum. 

After listening to the recording, I want ot create a very minimalist, slow and mellow sound. 

## Experimenting with the score

When I open the score, I let it play and there were many different sounds generating on their own. 
lots of low frequency in combination with high pitch frequencies.  

First, turn FREQ knob from VCF to the left to work only with the low frequencies. 

![First change for low frequencies](https://i.imgur.com/CZxr2tb.png)
 
		
				
>>   **Block Size Value**  
>> Fixed crackling sound by changing the **block size** value in the Audio module from 256(5.3ms) to 4096 (85.3ms)  
Choose 4096 from the menu and the module display shows 3840. 
See pic below  

![Block Size 4096](https://i.imgur.com/qieA3Wo.png)

