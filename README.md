Here is a concise, punchy version of your paper formatted exactly for your GitHub `README.md`. It strips out the generic filler, focuses strictly on your real numbers, and highlights your pipeline.

```markdown
# Differentiating Cognitive Strain from Passive Disengagement: A Dual-Axis EEG Analysis of Objective Complexity vs. Subjective Confusion

**Author:** Mihika Saraf  

---

##  The Core Thesis
Traditional educational models assume a uniform physiological response to difficult content. This study proves a profound divergence between external material difficulty (**Objective Complexity**) and internal student comprehension (**Subjective Confusion**). Using single-channel EEG data, we map how these two states produce completely opposite physical and mental profiles.

---

##  Methodology & Pipeline
* **Hardware & Dataset:** Analyzed multi-subject brainwave data (10 students, 512 Hz sample rate) captured via a single-channel NeuroSky MindSet headset.
* **Automated Blink Detection:** Built an automated electromyographic (EMG) artifact filter using a strict statistical boundary:
  $$\text{Threshold} = \mu + 3\sigma$$
  Evaluating the raw EEG array yielded an empirical threshold of **1859.26 μV** to automatically isolate and count eye-blinks without manual verification.
* **Timeline Masking:** Isolated self-reported confusion intervals to create a distinct sub-timeline containing exactly **6,567 data points** for internal neuro-metric analysis.

---

##  Core Findings & Results

### 1. Ocular Dynamics (The Physical Split)
External difficulty and internal confusion trigger diametrically opposed physical behaviors:
* **Objective Complexity (+12.90% blink rate):** Transitioning to dense, complex video modules increases eye-blink frequency due to elevated cognitive load and visual scanning demands.
* **Subjective Confusion (-24.92% blink rate):** True personal misunderstanding severely suppresses the natural blinking reflex.

### 2. Cognitive State Mapping (The Mental Split)
To find out what drives the unblinking stare during confusion, we cross-referenced the 6,567 confused data points against Beta-wave (Attention) and Alpha-wave (Meditation) metrics[cite: 1]. The data soundly rejects the idea that confusion triggers active focus, showing that students spend nearly double the time zoned out:
* **Blanking Out / "Blank Stare" (High Meditation):** **27.97%** of the timeline[cite: 1]. Brainwaves reflect mental paralysis/stalling where the student hits an intellectual wall and experiences an involuntary zone-out.
* **Active Focus (High Attention):** Only **16.22%** of the timeline.
* **Neutral Baseline:** **55.81%** of the timeline.

---

##  Engineering Impact
Assuming a drop in blinking always means "intense focus" completely misinterprets a struggling student. This study proves that subjective confusion is primarily a state of **passive cognitive disengagement** rather than heightened concentration. By embedding this automated pipeline, future ed-tech platforms can detect a prolonged drop in blinking alongside falling attention scores to dynamically pause content and intervene before a student completely checks out.

```
