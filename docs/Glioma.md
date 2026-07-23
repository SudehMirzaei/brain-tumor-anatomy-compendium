# 🧠 Glioma

← [MRI Sequences](MRI_Sequences.md) | → [Meningioma](Meningioma.md)

---

## Overview

Glioma is the most common primary **intra-axial** brain tumor and originates from **glial cells**, the supporting cells of the central nervous system. Unlike many other brain tumors, gliomas infiltrate and destroy normal brain tissue while simultaneously compressing adjacent structures.

Among all glioma subtypes, **glioblastoma (GBM)** is the highest-grade and most aggressive form.

---

# What Should Be Studied?

For every tumor type, four major aspects should be understood:

- Origin
- Typical anatomical location
- Clinical manifestations
- MRI characteristics

These features are the primary cues used by both radiologists and deep learning models for tumor classification.

---

# Origin

Gliomas arise from **glial cells** rather than neurons.

Major glial cell types include:

- Astrocytes
- Oligodendrocytes
- Ependymal cells

Because these cells are naturally found within the brain parenchyma, gliomas are classified as **primary intra-axial brain tumors**.

---

# Biological Behavior

The defining characteristic of glioma is **infiltration**.

Unlike meningiomas, gliomas do not simply compress the brain. They invade normal brain tissue, making complete surgical removal extremely difficult.

Consequences include:

- Poorly defined tumor margins
- Destruction of healthy brain tissue
- Microscopic tumor spread
- High recurrence rate

Treatment usually combines:

- Surgery
- Radiation therapy
- Chemotherapy

---

# Mechanism of Brain Injury

Gliomas damage the brain through two mechanisms.

## 1. Infiltration

Tumor cells invade and replace healthy brain tissue.

## 2. Mass Effect

As the tumor enlarges, it compresses adjacent brain structures.

Because both mechanisms occur simultaneously, gliomas often produce more severe neurological deficits than purely compressive tumors.

---

# Vasogenic Edema

Gliomas frequently disrupt the blood-brain barrier (BBB).

This permits plasma fluid to leak into surrounding white matter, producing **vasogenic edema**.

Consequences include:

- Cerebral swelling
- Increased intracranial pressure (ICP)
- Compression of nearby brain tissue

> [cerebral_swelling_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/cerebral_swelling.jpg)

---

# Increased Intracranial Pressure (ICP)

Because the skull is a rigid structure, expanding tumor volume and edema elevate intracranial pressure.

Common symptoms include:

- Headache
- Nausea
- Vomiting
- Blurred vision
- Drowsiness
- Reduced consciousness

Severe ICP elevation may result in **brain herniation**, a neurological emergency.

---

# Clinical Manifestations

Symptoms depend on the anatomical region involved.

## Frontal Lobe

- Personality changes
- Poor judgment
- Behavioral abnormalities
- Apathy
- Aggression

## Motor Cortex

- Progressive limb weakness
- Difficulty moving an arm or leg
- Paralysis in advanced disease

## Language Areas

### Broca's Area

- Preserved comprehension
- Difficulty producing speech

### Wernicke's Area

- Fluent but meaningless speech
- Impaired language comprehension

## Seizures

Gliomas commonly irritate the cerebral cortex, disrupting electrical activity and producing seizures.

## Rapid Progression

High-grade gliomas may double in size within weeks, distinguishing them from slowly growing tumors such as many meningiomas.

---

# MRI Characteristics

## 1. Intra-Axial Location

Gliomas arise within the **brain parenchyma**, usually involving the white matter.

This differentiates them from:

- Meningioma (extra-axial)
- Pituitary tumor (sellar)

> [intra_axial_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/intra_axial_glioma.jpg)

---

## 2. Corpus Callosum Involvement

Aggressive gliomas frequently spread across the corpus callosum.

This creates the classic **Butterfly Glioma**, one of the strongest imaging clues for glioblastoma.

> [butterfly_glioma_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/butterfly_glioma.jfif)

---

## 3. Tumor Heterogeneity

High-grade gliomas commonly contain:

- Viable tumor tissue
- Necrosis
- Hemorrhage
- Vasogenic edema

Multiple tissue types coexist within the same lesion.

> [Heterogeneity_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/necrotic_core.jpg)

---

## 4. Ring Enhancement

Following gadolinium administration:

- The necrotic center remains dark.
- Viable tumor enhances brightly.

This produces the characteristic **thick irregular ring-enhancing lesion**.


---

## 5. Vasogenic Edema

Glioma-associated edema is typically:

- Extensive
- Finger-like
- Irregular

These findings often extend well beyond the visible tumor.

> [vasogenic_edema_1_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/vasogenic_edema_1.jpg)
> [vasogenic_edema_2_img](brain-tumor-anatomy-compendium/tree/main/images/glioma/vasogenic_edema_2.jpg)

---

## 6. Mass Effect

Large tumors may produce:

- Ventricular compression
- Midline shift
- Increased intracranial pressure

Significant midline shift represents a radiological emergency.

---

## 7. Poorly Defined Borders

Gliomas usually demonstrate:

- Irregular margins
- Infiltrative borders
- Blending with surrounding edema

Unlike meningiomas, there is rarely a sharp boundary between tumor and normal brain tissue.

---

# CNN-Relevant Imaging Features

A CNN trained for glioma classification should learn:

- Intra-axial location
- White matter involvement
- Corpus callosum invasion
- Butterfly configuration
- Tumor heterogeneity
- Necrotic core
- Thick irregular ring enhancement
- Finger-like vasogenic edema
- Ventricular compression
- Midline shift
- Poorly defined infiltrative borders

These imaging characteristics are considerably more informative than tumor size alone.

---

# Data Augmentation Considerations

Medical image augmentation should preserve clinically meaningful imaging features.

Recommended augmentations:

- Rotation
- Small zoom
- Mild brightness adjustment
- Mild contrast adjustment
- Horizontal and vertical flipping (when anatomically appropriate)

Avoid aggressive intensity transformations that alter:

- Dark necrotic core
- Bright enhancing rim

Destroying these relationships may prevent the model from learning important imaging biomarkers of glioblastoma.

---

# Key Takeaways

- Gliomas originate from glial cells within the brain parenchyma.
- Their defining biological behavior is infiltration rather than simple compression.
- Vasogenic edema contributes significantly to neurological deterioration.
- MRI commonly demonstrates intra-axial location, heterogeneous enhancement, necrosis, edema, and infiltrative borders.
- CNNs should learn anatomical location and pathological imaging features rather than relying solely on tumor size.

---

## Next Chapter

➡️ [Meningioma](Meningioma.md)

