# 120 Dots - Mindfulness Web App

A minimalist 2-minute meditation experience using visual dot progression.

[claude artifact](https://claude.ai/public/artifacts/e0ba3ed7-bdc6-4d75-9b75-892ff68fa959)

## Features
- 120 dots that fill over 2 minutes
- Mouse movement detection with reset functionality
- Email collection after completion
- Responsive, calming design

# 120 Dots - Product Requirements Document

## Product Overview

**Product Name:** 120 Dots  
**Type:** Minimalist meditation/focus web application  
**Inspiration:** thewayofcode.com aesthetic  
**Core Concept:** A 2-minute mindfulness experience using visual dot progression

## Product Vision

Create a calming, minimalist web experience that guides users through a 2-minute mindfulness session using animated dot filling, promoting focus and digital wellness.

## Core Features

### 1. Visual Display
- **120 Dots Grid:** Display exactly 120 dots in an artistic, aesthetically pleasing arrangement
- **Initial State:** All dots appear dimmed/unfilled
- **Progressive Filling:** One dot fills every second (1 dot/second for 120 seconds = 2 minutes)
- **Visual Style:** Clean, minimalist design inspired by thewayofcode.com

### 2. Timer Functionality
- **Duration:** Exactly 2 minutes (120 seconds)
- **Auto-start:** Timer begins automatically when page loads
- **Visual Progress:** Dots serve as both timer and progress indicator
- **Completion:** All dots filled indicates session complete

### 3. Mouse Interaction
- **Interrupt Trigger:** Any mouse movement stops the timer immediately
- **Modal Display:** Interruption triggers a reset confirmation modal
- **Reset Option:** Modal allows user to restart the 2-minute session
- **No Accidental Interruptions:** Clear intentional interaction required

### 4. Email Collection (Post-Session)
- **Trigger:** Appears only after successful 2-minute completion
- **Email Input:** Simple, clean email collection form
- **Future Integration:** Prepared for backend integration (placeholder for now)
- **Optional:** User can skip email entry

## Technical Requirements

### Design Specifications
- **Responsive Design:** Works on desktop, tablet, and mobile
- **Minimalist Aesthetic:** Clean typography, ample whitespace
- **Color Palette:** Muted, calming colors (grays, soft blues/greens)
- **Dot Styling:** 
  - Unfilled: Semi-transparent or outlined
  - Filled: Solid color with subtle animation
  - Size: ~8-12px diameter
- **Grid Layout:** Artistic arrangement (not strict rows/columns)

### Interaction Flow
1. **Page Load:** 120 dimmed dots displayed, timer auto-starts
2. **Progress:** Dots fill sequentially, one per second
3. **Mouse Movement:** Timer pauses, modal appears with reset option
4. **Reset:** Clears all dots, restarts timer from beginning
5. **Completion:** All dots filled, email collection appears
6. **Email Submit:** Thank you message or next steps

### Performance Requirements
- **Load Time:** Under 2 seconds
- **Smooth Animation:** 60fps dot filling animations
- **Timer Accuracy:** Precise 1-second intervals
- **Responsive:** No lag on mouse movement detection

## User Experience Goals

### Primary Objectives
- **Mindfulness:** Encourage 2 minutes of focused, calm attention
- **Simplicity:** Zero learning curve, intuitive interaction
- **Beauty:** Visually pleasing, art-like experience
- **Interruption Awareness:** Make users conscious of digital distractions

### Success Metrics
- **Completion Rate:** Percentage of users who complete full 2-minute session
- **Interruption Rate:** How often users trigger mouse interruption
- **Return Usage:** Users who restart after interruption
- **Email Collection:** Conversion rate for email signups

## Content & Messaging

### Modal Text (Mouse Interruption)
```
Pause for focus?
Your 2-minute mindfulness session was interrupted.

[Restart Session] [Continue Browsing]
```

### Completion Message
```
Well done.
You've completed 2 minutes of focused attention.

[Optional: Share your email for mindfulness tips]
[Email Input Field]
[Submit] [Skip]
```

### Thank You Message
```
Thank you.
Check your email for mindfulness resources.
```

## Technical Implementation Notes

### Frontend Framework
- **Vanilla JS + HTML/CSS** or **React** (for artifact compatibility)
- **No external dependencies** for core functionality
- **CSS animations** for dot filling effects

### State Management
- Timer state (running/paused/completed)
- Dots filled count (0-120)
- Mouse movement detection
- Modal visibility state
- Email collection state

### Future Considerations
- **Backend Integration:** Email collection API
- **Analytics:** User behavior tracking
- **Customization:** Different dot counts, colors, or patterns
- **Sound:** Optional ambient sounds or completion chime
- **Sharing:** Social sharing of completed sessions

## Development Phases

### Phase 1 (MVP)
- Basic dot grid display
- Timer functionality with dot filling
- Mouse interruption detection
- Reset modal

### Phase 2 (Enhancement)
- Email collection interface
- Improved visual design
- Mobile responsiveness
- Smooth animations

### Phase 3 (Future)
- Backend integration
- User accounts
- Session history
- Customization options

## Success Definition

A successful "120 Dots" application will:
1. Load quickly and display 120 artistically arranged dots
2. Fill one dot every second for exactly 2 minutes
3. Detect mouse movement and offer reset functionality
4. Collect user emails after successful completion
5. Provide a calming, meditative user experience
6. Maintain visual appeal inspired by thewayofcode.com

---

*This PRD serves as a blueprint for creating a minimalist, mindfulness-focused web application that combines visual beauty with intentional user interaction design.*
