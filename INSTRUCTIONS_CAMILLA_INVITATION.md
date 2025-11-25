# Complete Instructions: Camilla's Bowling Date Invitation

## Overview
Create a single-file, interactive HTML invitation for a bowling date with Camilla. The invitation uses a warm, earthy color palette (browns, tans, beiges) with a slide-based presentation format featuring 7 interactive slides.

---

## Personalization Variables

**Required Personalization:**
- **Her Name**: `Camilla`
- **Your Name**: `Jonathan`
- **Phone Number**: `7134372364` (formatted as `7134372364` in code, displays as `713-437-2364`)
- **Activity**: Bowling
- **Day**: Sunday
- **Message**: "Hey! I'm totally down for bowling on Sunday! Can't wait to see you there! 🎳"

---

## Design Specifications

### Color Palette
- **Primary Brown**: `#8B4513` (Saddle Brown)
- **Secondary Brown**: `#A0522D` (Sienna)
- **Light Brown**: `#CD853F` (Peru)
- **Medium Brown**: `#D2691E` (Chocolate)
- **Dark Brown**: `#654321` (Dark Brown)
- **Very Dark Brown**: `#5C4033`
- **Background Gradient**: `linear-gradient(135deg, #f5deb3 0%, #deb887 25%, #d2b48c 50%, #cd853f 75%, #f5deb3 100%)`
- **Welcome Card Background**: `rgba(255, 248, 220, 0.95)` (Corn Silk with transparency)
- **Text Colors**: 
  - White (`#fff`) for dark backgrounds
  - Dark gray (`#666`) for light backgrounds
  - Brown (`#8B4513`) for titles

### Typography
- **Primary Font**: `'Quicksand', sans-serif` (body text)
- **Heading Font**: `'Poppins', sans-serif` (titles)
- **Script Font**: `'Dancing Script', cursive` (welcome title)
- **Icon Font**: Font Awesome 6.4.0

### External Resources
- **Google Fonts**: Quicksand (300-700), Poppins (300-600), Dancing Script (400-700)
- **Font Awesome CDN**: `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`

---

## Page Structure: 7 Interactive Slides

### Slide 1: Welcome Slide
**Class**: `welcome-slide`
**Content**:
- **Title**: "Hey Camilla!" (Dancing Script, 3.5rem, color: #8B4513)
- **Message**: "I've got something to ask you..."
- **Button**: "Continue" with arrow-right icon

**Styling**:
- Background: `rgba(255, 248, 220, 0.95)`
- Border: `2px solid rgba(160, 82, 45, 0.4)`
- Border radius: `25px`
- Box shadow: `0 20px 40px rgba(139, 69, 19, 0.2)`
- Backdrop filter: `blur(10px)`

### Slide 2: Invitation Slide
**Class**: `invitation-slide`
**Content**:
- **Title**: "So here's the thing..." (Poppins, 2.2rem, white)
- **Text**: "I'd love to take you on a date!" (1.4rem, white)
- **Button**: "Tell me more" with arrow-right icon

**Styling**:
- Background: `linear-gradient(135deg, #D2691E 0%, #CD853F 100%)`
- Border: `3px solid #8B4513`
- Border radius: `25px`

### Slide 3: Tease Slide
**Class**: `tease-slide`
**Content**:
- **Text**: "Wanna see what I've got planned?" (1.5rem, white)
- **Button**: "Show me what you got!" with search icon

**Styling**:
- Background: `linear-gradient(135deg, #A0522D 0%, #8B4513 100%)`
- Border: `3px solid #654321`

### Slide 4: Activity Reveal
**Class**: `reveal-slide`
**Content**:
- **Title**: "This is gonna be fun!" (Poppins, 2rem, white)
- **Icon**: Bowling ball icon (Font Awesome, 3rem, color: #8B4513, animated bounce)
- **Text**: "I thought we could go bowling! Hit the lanes, have some laughs, maybe make a friendly bet on who scores higher 😄" (1.3rem, white)
- **Button**: "When are we doing this?" with calendar icon

**Styling**:
- Background: `linear-gradient(135deg, #D2691E 0%, #CD853F 100%)`
- Border: `3px solid #8B4513`

### Slide 5: Day Reveal
**Class**: `reveal-slide`
**Content**:
- **Title**: "Sunday works best for me" (Poppins, 2rem, white)
- **Icon**: Calendar check icon (Font Awesome, 3rem, animated bounce)
- **Text**: "I'm thinking Sunday! Perfect day to chill, have some fun, and just hang out together." (1.3rem, white)
- **Button**: "Cool, let's do it!" with check icon

### Slide 6: Day Confirmation
**Class**: `scheduling-slide`
**Content**:
- **Title**: "So yeah, Sunday it is!" (Poppins, 1.8rem, white)
- **Large Icon**: Calendar day icon (4rem, white)
- **Day Text**: "Sunday" (2rem, white, font-weight: 600)
- **Message**: "I'm really looking forward to it!" (1.2rem, white)
- **Button**: "Sounds good!" with arrow-right icon

**Styling**:
- Background: `linear-gradient(135deg, #A0522D 0%, #8B4513 100%)`
- Border: `3px solid #654321`

### Slide 7: Final Confirmation
**Class**: `confirmation-slide`
**Content**:
- **Title**: "Awesome!" (Dancing Script, 2.5rem, white)
- **Message 1**: "Can't wait to see you!" (dynamic, updates to "Can't wait to see you on Sunday!")
- **Message 2**: "Let me know if you're in! Just hit that button below 😊"
- **Button 1**: "I'm in!" with check icon (primary action)
- **Button 2**: "Start Over" with redo icon (secondary, darker gradient)

**Styling**:
- Background: `linear-gradient(135deg, #D2691E 0%, #CD853F 100%)`
- Border: `3px solid #8B4513`

---

## Interactive Elements

### Buttons
**Base Styling**:
- Background: `linear-gradient(45deg, #8B4513, #A0522D)`
- Color: White
- Padding: `18px 36px`
- Font size: `1.2rem`
- Font weight: `600`
- Border radius: `50px`
- Box shadow: `0 8px 25px rgba(139, 69, 19, 0.4)`
- Font family: Poppins
- Cursor: pointer

**Hover Effects**:
- Transform: `translateY(-3px)`
- Box shadow: `0 12px 35px rgba(139, 69, 19, 0.5)`
- Shine effect: gradient sweep animation

**Active State**:
- Transform: `translateY(-1px)`

### Progress Dots
- **Position**: Fixed bottom, centered
- **Count**: 7 dots (one per slide)
- **Inactive**: `rgba(255, 255, 255, 0.5)`, 12px diameter
- **Active**: `#8B4513`, scale 1.2
- **Functionality**: Clickable to jump to any slide

### Decorative Elements
- **Floating LEGO Bricks**: 4 animated bricks with brown gradient
  - Position: Absolute, various corners
  - Animation: Float up and down with rotation
  - Opacity: 0.15
  - Size: 40px × 20px
  - Animation delay: Staggered (0s, 1s, 2s, 4s)

- **Floating Bears**: Animated bear emojis (🐻)
  - Spawn every 5 seconds
  - Float upward with rotation
  - Font size: 25px
  - Animation: 4 seconds, fade out

---

## JavaScript Functionality

### Core Functions

1. **`showSlide(slideNumber)`**
   - Hides all slides
   - Shows target slide
   - Updates progress dots
   - Updates currentSlide variable

2. **`nextSlide()`**
   - Advances to next slide if not on last slide
   - Calls showSlide()

3. **`goToSlide(slideNumber)`**
   - Jumps directly to specified slide
   - Used by progress dots

4. **`updateProgressDots(activeSlide)`**
   - Updates visual state of progress indicators
   - Adds/removes 'active' class

5. **`selectDay(day)`**
   - Sets selectedDay variable (default: 'Sunday')
   - Updates confirmation message
   - Advances to final slide

6. **`confirmDate()`**
   - Creates SMS message: "Hey! I'm totally down for bowling on Sunday! Can't wait to see you there! 🎳"
   - Phone number: `7134372364`
   - Opens SMS/iMessage with pre-filled message
   - Uses both `sms:` and `sms:?body=` formats for compatibility

7. **`restart()`**
   - Resets to slide 1
   - Resets selectedDay to 'Sunday'

### Event Listeners

- **Button clicks**: Scale animation on click
- **Keyboard navigation**:
  - Arrow Right / Space: Next slide
  - Arrow Left: Previous slide
- **Progress dots**: Click to jump to slide

### Animations

- **Fade In**: All slides fade in from bottom (0.8s ease-in-out)
- **Bounce**: Icons bounce continuously (2s infinite)
- **Float**: LEGO bricks float with rotation (6s infinite)
- **Float Up**: Bears float upward with rotation (4s linear)
- **Pulse**: Heart icon pulses (1.5s infinite)
- **Button Shine**: Gradient sweep on hover (0.5s)

---

## Responsive Design

### Mobile Breakpoint: 768px

**Adjustments**:
- Container padding: `15px` (from 20px)
- Welcome title: `2.8rem` (from 3.5rem)
- Invitation title: `1.8rem` (from 2.2rem)
- Reveal title: `1.6rem` (from 2rem)
- Scheduling title: `1.5rem` (from 1.8rem)
- Confirmation title: `2rem` (from 2.5rem)

---

## Technical Requirements

### HTML5 Structure
- Single file HTML5 document
- Semantic HTML elements
- Proper meta tags (charset, viewport)
- External font and icon libraries loaded in `<head>`

### CSS
- All styles inline in `<style>` tag
- CSS variables not used (direct color values)
- Flexbox for layout
- CSS animations for effects
- Media queries for responsiveness

### JavaScript
- Vanilla JavaScript (no frameworks)
- All code in `<script>` tag at bottom of body
- Event-driven architecture
- DOM manipulation for slide transitions
- Local state management (currentSlide, selectedDay)

### Accessibility
- Keyboard navigation support
- Semantic HTML structure
- Focus states on interactive elements
- ARIA labels (implicit through semantic HTML)

---

## Exact Content Specifications

### Title Tag
```html
<title>Jonathan's Special Invitation for Camilla</title>
```

### Slide Content (Exact Text)

**Slide 1**:
- "Hey Camilla!"
- "I've got something to ask you..."
- Button: "Continue"

**Slide 2**:
- "So here's the thing..."
- "I'd love to take you on a date!"
- Button: "Tell me more"

**Slide 3**:
- "Wanna see what I've got planned?"
- Button: "Show me what you got!"

**Slide 4**:
- "This is gonna be fun!"
- Icon: Bowling ball
- "I thought we could go bowling! Hit the lanes, have some laughs, maybe make a friendly bet on who scores higher 😄"
- Button: "When are we doing this?"

**Slide 5**:
- "Sunday works best for me"
- Icon: Calendar check
- "I'm thinking Sunday! Perfect day to chill, have some fun, and just hang out together."
- Button: "Cool, let's do it!"

**Slide 6**:
- "So yeah, Sunday it is!"
- Icon: Calendar day (large)
- "Sunday" (large text)
- "I'm really looking forward to it!"
- Button: "Sounds good!"

**Slide 7**:
- "Awesome!"
- "Can't wait to see you!" (updates to "Can't wait to see you on Sunday!")
- "Let me know if you're in! Just hit that button below 😊"
- Button: "I'm in!"
- Button: "Start Over"

### SMS Message
```
Hey! I'm totally down for bowling on Sunday! Can't wait to see you there! 🎳
```

### Phone Number Format
- In code: `7134372364` (no dashes)
- Display: Can be formatted as `713-437-2364` if needed

---

## File Output

**File Name**: `index.html` (or `index copy.html` for backup)

**File Structure**:
1. DOCTYPE and HTML opening tags
2. Head section:
   - Meta tags
   - Title
   - External font links
   - External icon library link
   - Complete CSS in `<style>` tag
3. Body section:
   - Decorative elements container
   - Main container with 7 slides
   - Progress dots
   - Complete JavaScript in `<script>` tag
4. Closing tags

---

## Testing Checklist

- [ ] All 7 slides display correctly
- [ ] Navigation buttons work (next/previous)
- [ ] Progress dots are clickable and update correctly
- [ ] Keyboard navigation works (Arrow keys, Space)
- [ ] SMS confirmation opens with correct message
- [ ] Responsive design works on mobile (< 768px)
- [ ] All animations play smoothly
- [ ] Floating bears appear every 5 seconds
- [ ] LEGO bricks float continuously
- [ ] Button hover effects work
- [ ] "Start Over" button resets to slide 1
- [ ] Confirmation message updates when day is selected

---

## Deployment Notes

- File should be named `index.html` for GitHub Pages
- Repository: `https://github.com/jonaDaniM/camilla-invite`
- All external resources (fonts, icons) load from CDN
- No build process required - pure HTML/CSS/JS
- Works in all modern browsers
- Mobile-friendly design

---

## Special Features

1. **Slide-based presentation**: Smooth transitions between 7 interactive slides
2. **Progress indicator**: Visual dots showing current position
3. **Keyboard navigation**: Full keyboard support for accessibility
4. **Animated decorations**: Floating LEGO bricks and bears
5. **SMS integration**: One-click confirmation that opens messaging app
6. **Responsive design**: Adapts to mobile and desktop screens
7. **Smooth animations**: Fade-ins, bounces, floats, and transitions
8. **Interactive buttons**: Hover effects with shine animations

---

## Color Reference Quick Guide

```
Primary Brown:    #8B4513
Secondary Brown:  #A0522D
Light Brown:      #CD853F
Medium Brown:     #D2691E
Dark Brown:       #654321
Very Dark Brown:  #5C4033
Background:       Gradient from #f5deb3 to #cd853f
Welcome Card:     rgba(255, 248, 220, 0.95)
Text (dark bg):   #fff (white)
Text (light bg):  #666 (gray)
Title Brown:      #8B4513
```

---

## Font Reference

- **Body**: Quicksand (weights: 300, 400, 500, 600, 700)
- **Headings**: Poppins (weights: 300, 400, 500, 600)
- **Script**: Dancing Script (weights: 400, 500, 600, 700)
- **Icons**: Font Awesome 6.4.0

---

**End of Instructions**

