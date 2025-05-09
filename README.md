# 🖼️ Smart Image Editor – Swap Backgrounds or Subjects

## 📌 Project Summary

This app allows users to **select the subject** of an image and then either:
- 🔁 **Replace the background**, or
- 🔄 **Replace the subject** while keeping the background intact.

It's powered by the **Segment Anything Model (SAM)** for object selection and a **text-to-image diffusion model** for generating stunning new scenes or subjects.

---

## 🧠 How It Works

1. **Upload an image**
2. **Click to select** the subject (object of interest)
3. The **SAM model** detects the object and creates a **mask**
4. The user:
   - Accepts the mask OR
   - Refines it with additional positive/negative points
5. The user provides:
   - A **text prompt** for a new background (or subject)
   - Optionally, a **negative prompt**
6. The model infills the masked area using the prompt and outputs the final image
7. The user can also **invert the mask** to replace the subject instead of the background

---

## ✨ Features

- 🎯 Interactive object selection using SAM
- ✍️ Text-to-image generation with customizable prompts
- 🔄 Swap subject or background with one click
- 🧽 Object removal or clean inpainting
- 💡 Supports fine-tuning masks with extra points

---

## 💻 Project Environment

Your development environment is **pre-configured** with:
- `pytorch`
- `diffusers`
- `gradio`

No additional setup needed!

---

## 🧑‍💻 Code Responsibilities

You’ll be responsible for implementing:
- ✅ **Calling the SAM model** to generate masks
- ✅ **Selecting the best/most relevant mask**
- ✅ **Processing user feedback for mask refinement**
- ✅ **Invoking the diffusion model** to infill either background or subject

---

## 🔍 Example Use Cases

| Action              | Description                                       |
|---------------------|---------------------------------------------------|
| Background Swap     | Place your subject in a forest, beach, or city    |
| Subject Replacement | Turn a dog into a cat, or a car into a bicycle    |
| Object Removal      | Remove photobombers or unwanted items             |
| Creative Editing    | Add surreal or AI-generated elements              |

---

## 🚀 Getting Started

To run the app:

```bash
python app.py
