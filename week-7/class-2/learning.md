Bilkul! Yahan main tumhein **"Images in HTML & CSS"** lecture ke liye thori si **base theory (thory)** Urdu + English mix mein de raha hoon jo easily samajhne wali ho aur beginners ke liye perfect ho. Tum isay slides, PDF, ya verbally explain karne ke liye use kar sakte ho.

---

## 🖼️ **Images in HTML & CSS – Theory**

### 🔹 **1. `<img>` Tag – HTML ka Image Element**

> HTML mein images dikhane ke liye hum `<img>` tag use karte hain. Ye self-closing tag hota hai.

**Syntax:**
```html
<img src="image-url" alt="description">
```

- **`src`** → Image ka URL ya path (source).
- **`alt`** → Alternative text (agar image load na ho to ye dikhai deta hai, aur screen readers ke liye important hota hai).

---

### 🔹 **2. CSS se Image Ko Style Karna**

Images par CSS properties apply karke hum unhein visually achha bana sakte hain:

#### ✅ **Common Properties:**

| Property | Kaam |
|---------|------|
| `width`, `height` | Image ki size set karte hain |
| `border` | Image ke around border |
| `border-radius` | Corners ko rounded banata hai |
| `object-fit` | Image ko box ke andar kaise adjust karna hai (`cover`, `contain`) |
| `box-shadow` | Shadow effect |
| `filter` | Visual effects like `grayscale`, `blur`, etc. |
| `transition`, `transform` | Hover effects, animations ke liye |

---

### 🔹 **3. Object-Fit Property (Important Concept)**

> Jab image aur container ka size alag ho, to image stretch ya distort na ho uske liye `object-fit` ka use hota hai.

- **`cover`**: Image box ko pura fill karegi, extra part cut ho sakta hai.
- **`contain`**: Image pura dikhai degi, but empty space aa sakta hai.

---

### 🔹 **4. Circle Image (Avatar / Profile Pic)**

> Circular images banane ke liye `border-radius: 50%` use karte hain.

```css
img {
  width: 150px;
  height: 150px;
  border-radius: 50%;
}
```

---

### 🔹 **5. Responsive Images**

> Web design responsive hone chahiye. Isliye images par:
```css
img {
  max-width: 100%;
  height: auto;
}
```
> Taake image apne container ke andar hi rahe aur screen ke hisaab se adjust ho jaye.

---

### 🔹 **6. Image Hover Effects**

> User experience improve karne ke liye hum hover effects use karte hain:

```css
img:hover {
  transform: scale(1.1);
  transition: 0.3s;
}
```

