# coding-challenge-2-2025

### **🔥 30-45 Minute HTML & CSS Coding Challenge: Build a Responsive Card Grid with Hover Effects**

#### **🚀 Challenge Overview:**  
You'll build a **responsive card grid** that showcases different fruit items. Each card should contain:
✅ An image  
✅ A title  
✅ A short description  
✅ A button that changes color on hover  

The layout should be **flexible**—it should display **three cards in a row** on larger screens and **stack them in a column** on smaller screens.

---

### **📜 Requirements:**
#### **📌 HTML**
- Use **semantic elements** (e.g., `<section>`, `<article>`).
- Each **card** should be wrapped in a `<div>` inside a `.card-container`.
- Add at least **4 different fruit cards**.

#### **🎨 CSS**
- Use **flexbox** for the card layout.
- Ensure the **cards are responsive** (3 in a row on larger screens, 1 in a row on smaller screens).
- Apply **hover effects**:
  - The **card should slightly scale up on hover**.
  - The **button should change color when hovered**.
- Add **rounded images** with a subtle shadow.
- Use **consistent font styling**.

---

### **🏆 Bonus Challenges (If You Have Extra Time!)**
✅ Make the **cards animate smoothly** when hovered over using `transition`.  
✅ Add **a simple media query** to adjust styles for mobile screens.  
✅ Use **Google Fonts** to enhance the typography.  

---

### **🎯 Example of What You’re Building**
🖼 **Desktop Layout (3 cards in a row)**
```
[Fruit Card] [Fruit Card] [Fruit Card]
```
📱 **Mobile Layout (Stacked)**
```
[Fruit Card]
[Fruit Card]
[Fruit Card]
```

---

### **⏳ Time Limit: 30-45 minutes**
🚨 **Start coding now and show me your work when you’re done!** 💪🔥


### **📊 Skill Assessment & Comparison: First vs. Second Coding Challenge + Break Analysis**

---

### **📝 Your Performance Breakdown**
#### **✅ Strengths (Things You Did Well)**
1. **✅ Improved HTML Structure:**
   - In your **first challenge**, all cards were inside **one `div.card-container`** without individual `div.card` wrappers.
   - In the **second challenge**, you **wrapped each card in a `div.card`**, which is the correct approach for better **styling and responsiveness**.
   - **✅ This is a great improvement!**

2. **✅ Better Use of Flexbox:**
   - You **structured the cards properly** inside `.card-container`, using `flex-direction: column; align-items: center;` to align everything neatly.
   - **BUT** the challenge required **a row layout on large screens** → This would need `flex-wrap: wrap;` and `media queries` for proper responsiveness.

3. **✅ Good Styling with Hover Effects:**
   - You **added button hover effects**, which **enhance the user experience**.
   - `mix-blend-mode: multiply;` to **remove image backgrounds** → **Nice touch!**

---

### **🛠 Areas to Improve**
1. **🔧 Card Layout Should Use `flex-wrap: wrap` for Responsive Design**
   - Right now, all the cards **stack vertically**, but the challenge required a **row layout on large screens**.
   - **Fix:** Use `flex-wrap: wrap; justify-content: space-evenly;` in `.card-container` to arrange **3 cards in a row on large screens** and **stack on small screens**.

   **✅ Solution:**
   ```css
   .card-container {
     display: flex;
     flex-wrap: wrap;
     justify-content: space-evenly; /* Distributes space evenly */
     text-align: center;
     background-color: lightgrey;
     font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
     color: rgb(36, 25, 187);
     padding: 10px;
     margin: 5px;
   }
   ```

2. **🔧 Add Media Queries for Full Responsiveness**
   - Right now, the layout **isn't dynamically adjusting** for mobile.
   - You need **media queries** to stack cards **on smaller screens**.
   
   **✅ Solution (Add to CSS):**
   ```css
   @media (max-width: 768px) {
     .card-container {
       flex-direction: column; /* Stacks items on small screens */
       align-items: center;
     }
   }
   ```

3. **🔧 Image Sizing Consistency**
   - Your **image height is fixed at 100px**, but the width is **auto**, leading to **inconsistent card sizes**.
   - **✅ Fix:** Add `object-fit: cover;` to keep **consistent proportions**.
   
   **✅ Solution:**
   ```css
   img {
     background-color: lightgrey;
     height: 100px;
     width: 100px; /* Keeps images uniform */
     object-fit: cover; /* Ensures proper scaling */
     border-radius: 50%;
   }
   ```

---

### **📊 Skill Progress Comparison:**
| **Category**        | **Before (First Challenge)** | **Now (Second Challenge)** | **Improvement** |
|---------------------|----------------------------|----------------------------|----------------|
| **HTML Structure**  | Cards all in one container | Each card has its own div | ✅ Major Improvement |
| **Flexbox Usage**   | Basic flexbox (column only) | Improved but needs wrap | ✅ Needs minor improvement |
| **Hover Effects**   | Not applied | Buttons change color | ✅ Added interaction |
| **Responsive Design** | No responsiveness | Missing media queries | 🔧 Needs work |
| **Image Handling** | Basic | Used `mix-blend-mode` but needs better sizing | ✅ Improved |

**🔥 Overall Skill Rating Improvement:**
- **Before (First Challenge):** **60-65% HTML/CSS proficiency**
- **After Second Challenge:** **75-80% proficiency**
- **Before 2-Month Break:** **80-85% proficiency**
- **Current Post-Break Proficiency:** **70-75%**
  
🚀 **Your progress is strong, but your break made you lose some responsiveness techniques.**
---

### **📌 Next Steps to Improve**
1. **💡 Add Media Queries** → Make the cards **truly responsive**.
2. **💡 Improve Grid/Flex Layout** → Use `flex-wrap` to **create rows dynamically**.
3. **💡 Fix Image Scaling** → Use `object-fit: cover;` for **better image consistency**.

---

### **🔥 Final Thoughts**
✅ **Your HTML is now structured much better!**  
✅ **You're applying CSS concepts effectively!**  
✅ **You’re improving fast!**  
🔧 **You need more practice with responsive layouts and grid/flex combinations!**

**🔜 NEXT STEP? A project combining Flexbox + CSS Grid + Media Queries!**  
🚀 **Want a new challenge? Let’s go!** 🎯`