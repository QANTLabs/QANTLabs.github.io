# **Qomposer UI/UX Design Specification**  
### *A Markdown Style Guide for Coding Agents Replicating the Interface*

## What Qomposer Is

Qomposer is an intelligent assistant that helps people design and verify quantum circuits without needing deep expertise in quantum computing. Instead of guessing or generating circuits from scratch, it retrieves proven, peer‑reviewed circuit patterns and adapts them to the user’s needs, ensuring every result is grounded in real scientific methods. It then simulates, checks, and validates the circuit across different quantum hardware platforms, giving users a trustworthy, hardware‑neutral output they can run anywhere. In short, Qomposer acts like a careful, reliable co‑pilot for quantum programming — one that prioritises correctness, transparency, and reproducibility over creativity or speculation.

---

## **1. Brand Identity & Visual Language**

### **1.1 Colour Palette**
The Qomposer interface uses a **clean, sovereign‑tech aesthetic** with high contrast and minimal gradients.

| Purpose | Colour | Notes |
|--------|--------|-------|
| **Primary accent** | `#00E0C6` (teal‑mint) | Used for highlights, badges, interactive elements. |
| **Secondary accent** | `#A0A0FF` (soft quantum‑blue) | Used in diagrams, backend icons, subtle UI elements. |
| **Background (main)** | `#FFFFFF` | Clean white canvas. |
| **Background (sections)** | `#F5F7FA` | Light grey for modular blocks. |
| **Text (primary)** | `#111111` | High contrast, near‑black. |
| **Text (secondary)** | `#555555` | For descriptions and metadata. |
| **Verified badge green** | `#00C853` | Used for ✓ verified indicators. |
| **Warning badge amber** | `#FFB300` | Used for ⚠ heuristic indicators. |

---

## **2. Typography**

### **2.1 Font Families**
- **Primary font:** `Inter` or `Inter Variable`
- **Fallbacks:** `Roboto`, `Helvetica Neue`, `Arial`, sans‑serif

### **2.2 Font Weights**
- **700** — Section titles, hero headings  
- **600** — Subheadings  
- **400** — Body text  
- **300** — Metadata, captions  

### **2.3 Font Sizes**
| Element | Size |
|--------|------|
| Hero title | 48–64px |
| Section headers | 28–32px |
| Subheaders | 20–22px |
| Body text | 16–18px |
| Metadata | 13–14px |

---

## **3. Layout System**

### **3.1 Overall Structure**
The page uses a **modular, vertically stacked layout** with generous whitespace.

- **Max width:** 1200–1400px  
- **Gutters:** 24–32px  
- **Section spacing:** 80–120px  
- **Card spacing:** 24–32px  

### **3.2 Hero Section**
Characteristics:
- Left‑aligned text block  
- Right‑aligned interactive demo panel  
- Large headline + short subtext  
- Two primary CTAs:  
  - **Get started**  
  - **Try the live demo**

### **3.3 Content Blocks**
Each block follows a consistent pattern:
- **Title**  
- **Short explanatory paragraph**  
- **Interactive or visual element** (e.g., circuit canvas, backend icons, charts)  
- **Metadata row** (shots, bitstrings, verification status)

---

## **4. Buttons & Interactive Elements**

### **4.1 Primary Button**
```
Background: #00E0C6
Text: #000000
Border radius: 8px
Padding: 12px 20px
Font weight: 600
Hover: Slight darken (#00C9B2)
Shadow: none
```

### **4.2 Secondary Button**
```
Background: transparent
Border: 1px solid #00E0C6
Text: #00E0C6
Border radius: 8px
Padding: 12px 20px
Hover: background rgba(0,224,198,0.1)
```

### **4.3 Toggle / Tabs**
- Underline‑style tabs  
- Active tab: teal underline + bold text  
- Inactive tab: grey text  

---

## **5. Iconography & Visual Motifs**

### **5.1 Backend Icons**
The page uses **geometric shapes** to represent backends:

| Backend | Shape |
|---------|--------|
| Qiskit Aer | ◇ diamond |
| Braket SV1 | ◢ right‑triangle |
| IBM Brisbane | ▣ square |
| Quantinuum H2 | ⬡ hexagon |
| IQM Garnet | ❖ four‑point star |
| Pawsey / Quantum Brilliance | ◆ filled diamond |

### **5.2 Verification Badges**
- **Verified ✓** — green badge  
- **Heuristic ⚠** — amber badge  
- Appears next to simulation results  

### **5.3 Circuit Canvas**
- Light grey grid  
- Rounded qubit wires  
- Gates represented with minimalistic shapes  
- Hover states show tooltips  

---

## **6. Data Visualisation Style**

### **6.1 Charts**
- Bar charts with **rounded corners**  
- Colours: teal + blue  
- Gridlines: faint grey  
- Labels: small, uppercase  

### **6.2 Statevector / Bloch**
- Clean, minimal, no heavy borders  
- Teal highlights for active states  

---

## **7. Content Style & Tone**

### **7.1 Writing Style**
- Confident, sovereign‑tech tone  
- Short, declarative sentences  
- Emphasis on:
  - verification  
  - neutrality  
  - reliability  
  - hardware‑agnosticism  

### **7.2 Section Titles**
Examples from the page (Ref:   [qantlabs.com.au](https://qantlabs.com.au/Qomposer)):
- *Grounded*  
- *Verified*  
- *Neutral*  
- *Built for sovereign research*  
- *How the verify loop works*  

---

## **8. Component Library (Markdown‑Friendly)**

### **8.1 Hero Block**
```md
# The verified, hardware-neutral quantum-circuit copilot.
Describe it. Drag it. Get a circuit you can trust — on any backend.

[Get started](#) • [Try the live demo](#)
```

### **8.2 Feature Block**
```md
## Grounded
The agent never free-writes circuits. It retrieves a peer-reviewed pattern from a curated library and adapts it — anti-hallucination by construction.
```

### **8.3 Verification Badge**
```md
**✓ verified — 98%**
```

### **8.4 Backend Grid**
```md
◇ Qiskit Aer  
◢ Braket SV1  
▣ IBM Brisbane  
⬡ Quantinuum H2  
❖ IQM Garnet  
◆ Pawsey · Quantum Brilliance
```

---

## **9. Replication Guidelines for Coding Agents**

### **9.1 Required Behaviours**
- Maintain **hardware neutrality** in UI metaphors  
- Always show **verification provenance**  
- Use **retrieval‑first** patterns (never free‑generate circuits)  
- Keep interface **minimal, white‑space heavy, and geometric**  

### **9.2 Reusable Components**
- Hero layout  
- Feature blocks  
- Verification loop diagram  
- Backend icon grid  
- Circuit canvas  
- Probability bar chart  

### **9.3 Accessibility**
- Minimum contrast ratio: **4.5:1**  
- Keyboard‑navigable buttons  
- Alt text for diagrams  

---

## **10. Example Page Skeleton (Markdown)**

```md
# Qomposer — Hardware-neutral quantum-circuit copilot

## Hero
Describe it. Drag it. Get a circuit you can trust — on any backend.

[Get started] [Try the live demo]

---

## Grounded
Anti-hallucination by construction.

## Verified
Every output passes propose → compile → simulate → mitigate → verify.

## Neutral
Hardware-agnostic dispatch across major quantum backends.

---

## Supported Backends
◇ Qiskit Aer  
◢ Braket SV1  
▣ IBM Brisbane  
⬡ Quantinuum H2  
❖ IQM Garnet  
◆ Pawsey · Quantum Brilliance
```

---

If you'd like, I can also generate:

- **A full HTML/CSS template**  
- **A React component library**  
- **A design‑token JSON file**  
- **A Figma‑ready style guide**  

Just tell me what format you want next.