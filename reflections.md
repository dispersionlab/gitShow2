>### module2 description
>module2.js is logical comparator. It takes signal inputs in Inputs 1 & 2, and outputs the Max, Min, Mix of the two signals out Outputs 1, 2, 3, respectively.

>- Inputs: IN1, IN2
>- Outputs: OUT1, OUT2, OUT3

>## Score:

>Build a rhythmic pattern using the highlighted controls - culminating in noise morphing into tone.

A low winding sound pulsates in the left. 3 or so pulses of that winding sound begin prior to a slowly alternating low reverberation pulsates on the right.  As they slowly rise in amplitude, period after period, 19 seconds in, appears a sort of chime on the right, blending in with the reverb.  That chime gets louder, but its pitch changes back to a lower reverb, but still with higher amplitude.

><img src="https://i.imgur.com/PRBBGu9.png">

>Lfo-1 freq results in speed changes.<br/>

For at least the first minute (~60s) you don't really notice any speed changes.  This doesn't seem to happen until about ~82s into the recording.

>The left random rate results in “aftershocks” of rhythmic content.<br/>

The aftershocks heard are slightly unpleasant, but yet keeps you on the edge of your seat waiting to hear if they sharpen out their surrounding noise,  A noise, mind you, that sounds like you should be constantly on alert to lower your volume in case in clips out of control and pops your speakers!

At ~49 seconds in, the aftershock started to sound more like a smashing sound. My partner sitting beside me, reading, hears this and shouts: "Atari Pole Position!"

>[Pole Position (Wikipedia)](https://en.wikipedia.org/wiki/Pole_Position)

~82 seconds in, and the speed begins to increase.  ~10s after that, the volume increases, making the messy aftershock sound even more messy with surrounding noise.

>VCF freq results in higher overtone-like content


---

#### Initial Patch Parameters
*(file: patch.vcv)*<br />

Module | Control | Value | Type |
------ | ------- | ----- | ---- |
LFO-1  |  FREQ   | 0.35306| attenuator knob |
Random (L) |  RATE   | 0.002 | slider |
VCF    |  FREQ   | 87.206| attenuator knob |

---

#### First Edit Experiment
*(file: patch.vcv)*<br />

Module | Control | Value | Type |
------ | ------- | ----- | ---- |
LFO-1  |  FREQ   | <mark>0.047663</mark> | attenuator knob |
Random (L) |  RATE   | <mark>1.7907</mark> | slider |
VCF    |  FREQ   | <mark>8.1758</mark> | attenuator knob |

This edit attempts to slow down LFO frequency, that results into an elongated aftershock sound (approx. ~22s apart).

![VCF Setting](https://i.imgur.com/GuDCuZh.png)
![Random Rate](https://i.imgur.com/We3OF0H.png)
![LFO-1 Frequency](https://i.imgur.com/bgmG4QV.png)

---

#### Second Edit Experiment
*(file: patch.vcv)*<br />

Module | Control | Value | Type |
------ | ------- | ----- | ---- |
LFO-1  |  FREQ   | <mark>0.047663</mark> | attenuator knob |
Random (L) |  RATE   | <mark>1.7907</mark> | slider |
VCF    |  FREQ   | <mark>8.1758</mark> | attenuator knob |
