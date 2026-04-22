# Shopify D2C Animation

## 👩‍💻 Author

Mrunali Patil

---

## 📌 Overview

This project is a Shopify-based D2C storefront focused on animation and interaction.
It includes a **brand loader animation with homepage transition** and a **scroll-driven product animation**, implemented using GSAP.

The goal was to replicate premium D2C interaction patterns with smooth sequencing and scroll-linked behavior.

---

## ✨ Features

### 🔹 Loader Animation + Hero Transition

* Full-screen black loader overlay on page load
* SVG-based logo animation using:

  * Stroke draw (`stroke-dashoffset`)
  * Directional fill using `clip-path` (bottom → top)
* Smooth transition from loader to homepage
* Hero headline is pre-rendered behind loader
* Product image slides in from the right after loader exit
* No animation overlap between loader and hero

---

### 🔹 Scroll-Based Product Animation

* Built using GSAP ScrollTrigger
* 3 vertically stacked sections
* Product bottle moves horizontally across sections
* Movement is fully tied to scroll (`scrub`)
* Animation:

  * Stops when scrolling stops
  * Reverses smoothly on scroll up
* Bottle remains vertically centered and appears above content
* Native scrolling preserved (no scroll-jacking)

---

## 🛠️ Tech Stack

* Shopify (Liquid)
* HTML, CSS, JavaScript
* GSAP (GreenSock Animation Platform)
* GSAP ScrollTrigger

---

## 📁 Project Structure

```
sections/
  loader-hero.liquid
  scroll-bottle.liquid

layout/
  theme.liquid

assets/
config/
snippets/
```

---

## 🎯 Key Implementation Details

* Used **clip-path instead of opacity** for directional fill animation
* Maintained **clear sequencing** between loader and hero transition
* Ensured **scroll-based animation is reversible and responsive**
* Structured code using **modular Shopify sections**

---

## 🚀 How to Run

1. Open the live store link
2. Enter the password
3. Observe:

   * Loader animation
   * Hero transition
   * Scroll-based product animation

---

## 📌 Notes

* No external animation plugins used
* No scroll-jacking implemented
* Focused on animation quality and performance

---

## 💬 Final Thought

This project focuses on replicating real-world D2C animation patterns with clean implementation, smooth transitions, and user-driven interactions.
