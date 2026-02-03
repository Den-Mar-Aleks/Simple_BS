---
license: other
tags:
  - lora
  - body-slider
  - stylized
  - chest-shape
pipeline_tag: text-to-image
---

# 🔵 Simple_BS — Upper-Body Volume Slider LoRA  
**ZIT compatible · Safe · Stylized chest-shape manipulation**

---

## ⚡ Quick Links

| Version | Weights | Preview |
|--------|---------|---------|
| **Main** | [/model/Simple_BS.safetensors](https://huggingface.co/dmsnoa/Simple_BS/resolve/main/model/Simple_BS.safetensors) | <img src="https://huggingface.co/dmsnoa/Simple_BS/resolve/main/model/2026-01-14-15.png" width="120"> <img src="https://huggingface.co/dmsnoa/Simple_BS/resolve/main/model/2026-01-14.png" width="120"> |

---

## 🔍 Overview
**Simple_BS** is a stylized body-geometry LoRA that modifies **only the artistic volume of the upper body**.  
It adjusts the **shape and silhouette of the chest area** while keeping all realism-critical traits unchanged:

- identity  
- age  
- ethnicity  
- facial structure  
- body proportions outside the chest zone  

All effects remain **non-realistic, stylized, and safely bounded**.

---

## ⚙️ How the Slider Works

Move the `network_multiplier` to control chest-volume stylization:

| Multiplier | Effect |
|-----------:|--------|
| `-2 → -0.7` | noticeably reduced chest volume |
| `-0.6 → -0.2` | mild flattening |
| `0` | neutral (no change) |
| `+0.2 → +0.7` | moderate volume increase |
| `+0.8 → +2` | strong stylized fullness |

The slider **does not** alter anatomy outside the chest silhouette.

---

## 🧩 Example Usage (ComfyUI / AITS Toolkit)

```yaml
lora:
  name: "dmsnoa/jix/Simple_BS"
  multiplier: 0.8   # fuller stylized result
```

### Recommended Base Prompt
```
person, solo, standing or seated,
neutral pose, looking at camera,
plain background, soft lighting,
realistic anatomy, photorealistic
```

💡 No need to mention breast size —  
the LoRA handles stylization automatically.

---

## 🔐 Safety Notice
- **Artistic stylization only** — not intended for realistic biological or medical modification  
- Does **not** change identity, age, or realism-critical anatomy  
- Safe for commercial and non-commercial usage under included license  

---


## 🧾 License
**CreativeML OpenRAIL-M**

---

## ✏️ Author  
Created by **dmsnoa / jix**

⭐ If this model helped you — consider starring the repository!
