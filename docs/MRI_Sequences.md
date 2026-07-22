# MRI Sequences

Before studying brain tumors, it is essential to understand the major MRI sequences. The appearance of a tumor depends not only on its pathology but also on the imaging sequence used. Radiologists interpret multiple MRI sequences together because each highlights different tissue characteristics.

A CNN trained on MRI images also learns these sequence-specific intensity patterns. Understanding what each sequence emphasizes helps explain why certain tumor features are more visible on one sequence than another.

---

## T1-Weighted Imaging (T1)

### Purpose

T1-weighted imaging provides excellent anatomical detail and is commonly used to evaluate normal brain anatomy.

### Typical Appearance

| Structure | Appearance |
|-----------|------------|
| White Matter | Bright |
| Gray Matter | Gray |
| Cerebrospinal Fluid (CSF) | Dark |
| Fat | Bright |
| Edema | Dark |
| Most Tumors | Isointense to Hypointense |

### Clinical Use

- Evaluating normal anatomy
- Detecting hemorrhage (depending on age)
- Baseline imaging before contrast administration

---

## T2-Weighted Imaging (T2)

### Purpose

T2-weighted imaging is highly sensitive to water content.

Because edema contains excess extracellular water, it appears very bright on T2 images.

### Typical Appearance

| Structure | Appearance |
|-----------|------------|
| CSF | Bright |
| Edema | Bright |
| Tumor | Often Bright |
| Gray Matter | Intermediate |
| White Matter | Slightly Darker |

### Clinical Use

- Detecting edema
- Visualizing tumor extent
- Assessing cystic components

---

## FLAIR (Fluid-Attenuated Inversion Recovery)

### Purpose

FLAIR is a modified T2 sequence that suppresses the signal from cerebrospinal fluid (CSF).

This makes abnormalities adjacent to the ventricles much easier to detect.

### Typical Appearance

| Structure | Appearance |
|-----------|------------|
| CSF | Dark |
| Edema | Bright |
| Tumor | Bright |
| White Matter Lesions | Bright |

### Clinical Use

- Detecting vasogenic edema
- Identifying infiltrative tumor margins
- Evaluating multiple sclerosis and other white matter diseases

---

## Diffusion-Weighted Imaging (DWI)

### Purpose

DWI measures the movement of water molecules within tissue.

Highly cellular tumors restrict diffusion because densely packed cells limit water movement.

### Restricted Diffusion Appears

- Bright on DWI
- Dark on ADC

### Clinical Use

- Acute ischemic stroke
- Brain abscess
- Hypercellular tumors
- Certain high-grade gliomas

---

## Apparent Diffusion Coefficient (ADC)

### Purpose

ADC is calculated from DWI and helps confirm whether diffusion is truly restricted.

### Interpretation

| DWI | ADC | Meaning |
|-----|-----|---------|
| Bright | Dark | Restricted diffusion |
| Bright | Bright | T2 Shine-through |
| Dark | Bright | Increased diffusion |

### Clinical Use

- Confirming diffusion restriction
- Characterizing tumor cellularity
- Differentiating tumor from abscess

---

## T1 Post-Contrast (T1+C)

### Purpose

After intravenous administration of gadolinium contrast, regions where the blood-brain barrier is disrupted become bright.

Normal brain tissue does not significantly enhance because the intact blood-brain barrier prevents gadolinium from entering the brain parenchyma.

### Typical Appearance

| Structure | Appearance |
|-----------|------------|
| Normal Brain | Minimal Enhancement |
| Enhancing Tumor | Bright |
| Necrotic Core | Dark |
| Blood Vessels | Bright |

### Clinical Use

- Detecting blood-brain barrier disruption
- Identifying active tumor
- Surgical planning
- Assessing tumor recurrence

---

# Why Different Tumor Features Appear on Different MRI Sequences

Understanding MRI sequences explains why radiologists use multiple images to evaluate a single tumor.

### Ring Enhancement

High-grade gliomas often contain a necrotic center surrounded by viable tumor tissue.

After gadolinium administration:

- The necrotic center remains dark because it contains no viable blood supply.
- The surrounding tumor enhances brightly due to disruption of the blood-brain barrier.

This produces the classic **thick, irregular ring-enhancing lesion** seen on T1 post-contrast imaging.

---

### Vasogenic Edema

Tumor-induced disruption of the blood-brain barrier allows plasma fluid to leak into surrounding white matter.

Because edema contains excess water, it appears:

- Bright on T2
- Bright on FLAIR
- Less conspicuous on T1

FLAIR is particularly useful because suppression of CSF makes edema easier to distinguish from normal ventricular fluid.

---

### Necrosis

Necrotic tissue contains dead cells and little blood flow.

Therefore it typically appears:

- Dark on T1
- Bright on T2
- Non-enhancing after contrast administration

The combination of a non-enhancing necrotic core and an enhancing tumor rim is a hallmark of glioblastoma.

---

### Tumor Cellularity

Highly cellular tumors restrict water diffusion.

These tumors typically appear:

- Bright on DWI
- Dark on ADC

Diffusion imaging provides additional information about tumor aggressiveness beyond conventional MRI.

---

# Why Multiple MRI Sequences Are Necessary

No single MRI sequence provides all the information needed to characterize a brain tumor.

Radiologists combine multiple sequences because each reveals different pathological features:

| MRI Sequence | Best Demonstrates |
|--------------|-------------------|
| T1 | Normal anatomy |
| T2 | Water and edema |
| FLAIR | Edema without bright CSF |
| DWI | Restricted diffusion |
| ADC | Diffusion confirmation |
| T1 Post-Contrast | Blood-brain barrier disruption and tumor enhancement |

A CNN trained on MRI images should learn not only the appearance of tumors but also the sequence-specific imaging patterns that reveal edema, necrosis, enhancement, and tissue infiltration.

