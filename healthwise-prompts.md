## V0 Prompts for HealthWise AI Components

### Prompt 1: Landing Page with Hero Section

```
Create a modern healthcare landing page for "HealthWise AI" with these sections:

HERO SECTION:

- Large heading: "Your Medical Reports, Simplified by AI"
- Subheading: "Upload your medical reports and get personalized health recommendations, dietary guidance, and condition-specific exercises - all powered by AI"
- Two CTA buttons: "Upload Report" (primary, gradient blue-purple) and "See Demo" (secondary, outlined)
- Background: Subtle gradient from light blue to white with floating medical icons (heart, stethoscope, chart)
- Hero image: Modern illustration of person looking at health dashboard on tablet

FEATURES SECTION (3 columns):

1. "AI-Powered Analysis" - Icon: brain/sparkles - Text: "Gemini AI analyzes your reports and explains results in simple language"
2. "Personalized Exercises" - Icon: dumbbell/activity - Text: "Get animated exercise routines designed for your specific condition"
3. "Smart Nutrition Guide" - Icon: apple/utensils - Text: "Know exactly what to eat and avoid based on your health"

HOW IT WORKS (4 steps with numbers):

1. Upload your medical report (PDF or image)
2. AI analyzes key metrics and findings
3. Get personalized DO's, DON'Ts, and diet plan
4. Start your custom exercise routine

TRUSTED BY section:

- Stats: "10,000+ Reports Analyzed" | "15 Conditions Supported" | "98% User Satisfaction"

FOOTER:

- Links: About, Privacy, Terms, Contact
- Social icons: Twitter, Instagram, LinkedIn
- Copyright: "© 2024 HealthWise AI"

DESIGN STYLE:

- Modern, clean, healthcare aesthetic
- Color palette: Primary blue (#3B82F6), accent purple (#8B5CF6), success green (#10B981)
- Use Lucide React icons
- Smooth animations on scroll
- Mobile responsive
- Use Inter or similar modern font
```

---

### Prompt 2: Report Upload & Analysis Dashboard

```
Create a medical report upload and analysis interface with these components:

LEFT PANEL - UPLOAD SECTION (40% width):

UPLOAD AREA:

- Dashed border rectangle with upload cloud icon
- Text: "Drop your medical report here or click to browse"
- Accepted formats: "PDF, JPG, PNG (Max 10MB)"
- After upload, show file preview card with:
  - File name and size
  - Small thumbnail preview
  - Remove button (X icon)
  - "Analyzing..." loading state with animated progress bar

FILE TYPE SELECTOR (chips):

- "Blood Test" | "Ultrasound" | "X-Ray" | "Prescription" | "Other"
- Selected state with blue background

PATIENT INFO (optional fields):

- Age input (number)
- Gender selector (Male/Female/Other)
- Existing conditions (multi-select chips: Diabetes, Hypertension, Pregnancy, etc.)

ANALYZE BUTTON:

- Large, gradient button at bottom
- "Analyze Report with AI" text
- Disabled state until file uploaded

RIGHT PANEL - ANALYSIS RESULTS (60% width):

LOADING STATE (while analyzing):

- Animated pulse loader
- Text: "AI is analyzing your report..."
- Progress steps: "Reading document → Extracting data → Generating insights"

RESULTS VIEW:

SUMMARY CARD (top):

- Alert banner with severity color (green/yellow/red)
- Main finding: "Blood sugar levels detected: 145 mg/dL (Moderate Risk)"
- Date analyzed
- Report type badge

TABBED SECTIONS:

Tab 1 - KEY FINDINGS:
- List of metrics with normal range indicators:
  - "Glucose: 145 mg/dL" [Yellow indicator] "Normal: 70-100"
  - "Hemoglobin: 11.2 g/dL" [Red indicator] "Normal: 12-16"
- Each with small info icon for explanation

Tab 2 - RECOMMENDATIONS:
Two columns:
DO's (green left border):
- ✓ Check blood sugar after meals
- ✓ Walk for 30 minutes daily
- ✓ Stay hydrated (8-10 glasses)
- ✓ Monitor weight weekly
- ✓ Sleep 7-8 hours nightly

DON'Ts (red left border):
- ✗ Avoid sugary drinks
- ✗ Skip meals
- ✗ Exercise on empty stomach
- ✗ Ignore warning signs
- ✗ Self-medicate

Tab 3 - DIET PLAN:

FOODS TO INCLUDE (grid layout):
- Cards with food emoji, name, benefit
- "🥦 Broccoli - Fiber, blood sugar control"
- "🥜 Almonds - Healthy fats, protein"
- Hover: Shows portion size

FOODS TO AVOID:
- Similar card layout with red accent
- "🍰 Pastries - Spikes blood sugar"

Tab 4 - EXERCISE PLAN:
- Button: "View Personalized Exercises →"
- Preview: 3 exercise cards with thumbnails

ACTIONS (bottom):
- "Download PDF Report" button
- "Share with Doctor" button
- "Save to Profile" button

DESIGN:
- Clean, medical dashboard aesthetic
- Use shadcn/ui components
- Smooth transitions between states
- Color coding for severity (green/yellow/red)
- Responsive layout (stack on mobile)
```

---

### Prompt 3: Interactive Exercise Player with Timer

```
Build an interactive exercise player interface for condition-specific workouts:

LAYOUT (3 sections):

LEFT SIDEBAR (25%):

WORKOUT INFO CARD:
- Condition badge: "Pregnancy - 2nd Trimester" (with icon)
- Workout title: "Prenatal Strength & Flexibility"
- Duration: "15 minutes"
- Difficulty: "Beginner" (with 1/5 dots)
- Benefits list: "Prepares body for labor, Reduces back pain, Improves circulation"

EXERCISE LIST:

Scrollable list showing all exercises in routine:
1. [ACTIVE] Pelvic Tilts - 1:00
2. [ ] Pregnancy Squats - 1:30
3. [ ] Cat-Cow Stretch - 1:00
4. [ ] Side Leg Raises - 2:00
5. [ ] Rest Period - 0:30
(continue pattern...)
- Active exercise highlighted with blue accent
- Completed exercises show green checkmark
- Show individual duration for each

MAIN AREA (50%):

ANIMATION DISPLAY:
- Large centered area with exercise animation
- Use placeholder: Animated illustration/Lottie animation of person doing exercise
- For MVP: Can use static illustration with pulsing effect
- Rounded corners, subtle shadow

CURRENT EXERCISE INFO (overlay bottom):
- Exercise name in large text: "Pelvic Tilts"
- Current set: "Set 1 of 3"
- Instruction overlay (can be toggled):
  - Step-by-step bullets
  - "1. Lie on your back with knees bent"
  - "2. Tighten abdominal muscles"
  - Auto-scrolls with timer

TIMER DISPLAY (center):
- Large circular progress ring
- Time remaining in center: "0:42"
- Progress percentage
- Color changes: Blue → Yellow (last 10 sec) → Green (complete)

RIGHT SIDEBAR (25%):

TIMER CONTROLS:
- Large Play/Pause button (center)
- Previous/Next exercise buttons
- Restart current exercise button
- "Skip to rest" button (if mid-exercise)

SETTINGS:
- Volume toggle (for audio cues)
- Speed control: 0.5x | 1x | 1.5x
- Auto-advance toggle
- Show/hide instructions

SAFETY PANEL:

Red alert card:
- "Stop Immediately If:"
- • You feel dizzy or lightheaded
- • Experience pain (not muscle fatigue)
- • Have difficulty breathing
- Emergency: 911 button

MODIFICATIONS:
Expandable section:
- "Make it easier: Use chair for support"
- "Make it harder: Add 2-lb weights"

PROGRESS STATS (bottom):
- Exercises completed: 3/8
- Time elapsed: 5:45 / 15:00
- Calories burned: ~35 (estimated)
- Progress bar

POST-WORKOUT SCREEN:
After all exercises complete:
- Celebration animation (confetti)
- "Great Work! Workout Complete 🎉"
- Summary stats
- "How do you feel?" rating (1-5 stars)
- "Save to History" button
- "Share Achievement" button
- "Repeat Workout" | "Browse More" buttons

MOBILE RESPONSIVE:
- Stack layout vertically
- Exercise list becomes bottom sheet
- Full-screen animation view
- Swipe gestures for next/previous

DESIGN STYLE:
- Modern fitness app aesthetic
- Primary: Blue (#3B82F6)
- Success: Green (#10B981)
- Warning: Yellow (#F59E0B)
- Use smooth transitions and animations
- Glassmorphism for overlay cards
- Large, touch-friendly buttons
```

---

### Prompt 4: Condition Selection & Personalization Page

```
Design a comprehensive health condition selector and personalization interface:

HEADER:
- Title: "Tell Us About Your Health"
- Subtitle: "We'll create a personalized exercise and nutrition plan"
- Progress steps: 1. Conditions → 2. Goals → 3. Preferences → 4. Review

STEP 1 - SELECT CONDITIONS:

MAIN CONDITIONS (card grid, 3 columns):
Each card shows:
- Large icon (relevant to condition)
- Condition name
- Brief description
- "Select" checkbox
- Hover: Blue border glow

Categories:

PREGNANCY:
- First Trimester (Weeks 1-12)
- Second Trimester (Weeks 13-26)
- Third Trimester (Weeks 27-40)

METABOLIC:
- Type 1 Diabetes
- Type 2 Diabetes
- Gestational Diabetes
- Thyroid Disorders

CARDIOVASCULAR:
- Hypertension (High BP)
- Post-Cardiac Surgery
- Heart Disease

RESPIRATORY:
- Asthma
- COPD

MUSCULOSKELETAL:
- Arthritis (Osteo/Rheumatoid)
- Chronic Back Pain
- Osteoporosis

NEUROLOGICAL:
- Parkinson's Disease
- Stroke Recovery

OTHER:
- Cancer Recovery
- Liver Disease
- Mental Health (Anxiety/Depression)
- "My condition isn't listed" (text input appears)

STEP 2 - SET GOALS:

Multi-select chips:
- Improve Fitness
- Lose Weight
- Manage Condition
- Prepare for Surgery/Birth
- Reduce Pain
- Increase Energy
- Better Sleep
- Stress Relief

STEP 3 - PREFERENCES:

FITNESS LEVEL:
Radio buttons with descriptions:
○ Beginner - "New to exercise"
○ Intermediate - "Exercise 1-2x per week"
○ Advanced - "Regular exerciser"

TIME COMMITMENT:
Slider: 10 min — 60 min per session
Days per week: Buttons 1-7

EXERCISE PREFERENCES (multi-select):
Checkboxes:
□ Low Impact
□ At Home (No Equipment)
□ Water Exercises
□ Yoga/Stretching
□ Strength Training
□ Cardio
□ Group Classes

DIETARY RESTRICTIONS:
Chips (can add custom):
- Vegetarian
- Vegan
- Gluten-Free
- Dairy-Free
- Nut Allergy
- Diabetic-Friendly
+ Add Custom

STEP 4 - REVIEW & GENERATE:

SUMMARY CARD:
Shows all selections in organized sections
- Conditions (with icons)
- Goals (with icons)
- Fitness level & time commitment
- Exercise preferences
- Dietary restrictions
"Edit" buttons for each section

GENERATE PLAN BUTTON:
- Large, prominent, gradient
- "Generate My Personalized Plan"
- Loading state: "Creating your custom plan..."

RESULTS PREVIEW:
After generation:
- "Your plan is ready! ✨"
- Preview cards:
  1. "12 Exercises Selected for You"
  2. "Customized Meal Plan"
  3. "Weekly Schedule"
- "View Full Plan" button

SAVE OPTIONS:
- Save to Profile
- Email Me the Plan
- Download PDF

DESIGN:
- Clean, step-by-step flow
- Use card-based layouts
- Smooth transitions between steps
- Progress indicator always visible
- Back button on each step
- Auto-save progress
- Mobile-friendly (stack vertically)
- Use encouraging copy and emojis
- Accessibility: High contrast, clear labels
```

---

### Prompt 5: Nutrition & Diet Plan Dashboard

```
Create a comprehensive nutrition dashboard showing personalized dietary recommendations:

TOP SECTION - DAILY OVERVIEW:

NUTRITION SCORE CARD (large, centered):
- Large circular gauge: 85/100 score
- Color gradient: Red → Yellow → Green based on score
- Text: "Great adherence today! 🎉"
- Breakdown: "8 of 10 recommendations followed"

QUICK STATS ROW (4 metrics):
1. Water Intake: 6/8 glasses (water drop icon, progress ring)
2. Meals Logged: 3/4 (plate icon)
3. Avoided Foods: 2 warnings (shield icon)
4. Calorie Target: 1,450/1,800 (flame icon)

MAIN CONTENT (2-column layout):

LEFT COLUMN (60%):

TODAY'S MEAL PLAN:
Accordion sections for each meal:

BREAKFAST (expandable):
Time: 7:00 - 9:00 AM
Recommended:
- Card 1: "Oatmeal with Berries"
  - Image placeholder
  - Portion: 1 cup oatmeal + 1/2 cup berries
  - Benefits: "Fiber for blood sugar control"
  - Calories: 280
  - "I ate this" button
- Card 2: "Greek Yogurt Parfait"
  - Similar format
  - Multiple options per meal

LUNCH (11:30 AM - 1:30 PM):
- 3 meal option cards with similar format

SNACK (3:00 - 4:00 PM):
- Healthy snack suggestions

DINNER (6:00 - 8:00 PM):
- 3 dinner option cards

EVENING SNACK (Optional):
- Light options if needed

Each meal section shows:
- Checkmark when logged
- Timer until next meal
- Swap button to see alternatives

MEAL LOGGER:
"What did you eat?" quick add:
- Search bar for foods
- Recent foods chips
- Custom entry option
- Camera icon: "Scan meal" (future feature)

FOODS TO FOCUS ON TODAY:
Grid of recommended foods (6 cards):
- 🥦 Leafy Greens - "3 servings" - Benefits: Iron, folate
- 🥜 Nuts & Seeds - "1 handful" - Benefits: Healthy fats
- 🐟 Fatty Fish - "1 serving" - Benefits: Omega-3
(continue pattern...)
Each card:
- Emoji/icon
- Food name
- Recommended serving
- Key benefit
- "Why this?" info icon tooltip

RIGHT COLUMN (40%):

WARNINGS & ALERTS:
Red alert card:
"⚠️ Foods to Avoid Today"
- 🍭 Added Sugars - "Risk: Blood sugar spike"
- 🧂 High Sodium Foods - "Risk: Elevated blood pressure"
- 🥤 Sugary Beverages - "Risk: Empty calories"
Each with explanation tooltip

NUTRIENTS TO TRACK:
Progress bars for key nutrients:
- Protein: 45g / 75g (60%) - Green
- Fiber: 18g / 30g (60%) - Green
- Iron: 12mg / 27mg (44%) - Yellow
- Calcium: 600mg / 1000mg (60%) - Green
Color coding:
- Green: On track
- Yellow: Needs attention
- Red: Deficient

HYDRATION TRACKER:
8 water glass icons
- Filled glasses (blue)
- Empty glasses (gray outline)
- "Add glass" button
- Target: 8 glasses (64 oz)
- Reminders: Every 2 hours

WEEKLY MEAL PREP GUIDE:
Card with:
- "Prep These This Weekend"
- Checklist of batch-cook items
- "View Full Prep Guide" button

SHOPPING LIST (collapsible):
Generated from meal plan:
- Grouped by category (Produce, Protein, Grains, etc.)
- Checkboxes
- "Share List" button
- "Export to App" options

BOTTOM SECTION:

WEEKLY ADHERENCE CHART:
Line graph showing:
- Days of week on X-axis
- Adherence score (0-100) on Y-axis
- Color-coded: Green zone (80-100), Yellow (60-79), Red (<60)
- Hover: Shows that day's details

INSIGHTS & TIPS:
Cards with personalized insights:
- "💡 You eat better on weekdays vs weekends"
- "🎯 Morning workouts → higher adherence"
- "⚠️ You're low on vitamin D - consider supplements"

QUICK ACTIONS (floating buttons):
- Log Meal (plus icon)
- Water Tracker (water drop)
- View Recipes
- Ask Nutritionist (chat icon)

DESIGN STYLE:
- Food photography style images
- Warm, appetizing color palette
- Green for healthy choices
- Red for warnings (not harsh)
- Cards with subtle shadows
- Smooth animations on interactions
- Mobile: Bottom nav for quick logging
- Use emoji for food items (friendly, universal)
```

---

### Prompt 6: Progress Tracking & Analytics Dashboard

```
Design a comprehensive progress tracking dashboard showing health journey analytics:

HEADER SECTION:
Welcome message: "Welcome back, Sarah! 💪"
Streak badge: "🔥 7-day workout streak!"
Last updated: "Updated 2 hours ago"

TOP METRICS (4 large cards):

1. TOTAL WORKOUTS:
- Large number: "24"
- Comparison: "+8 from last month" (green arrow up)
- Mini chart showing monthly trend
- Icon: Dumbbell

2. EXERCISE TIME:
- "8.5 hours"
- Average per session: "21 minutes"
- Target progress: 85%
- Icon: Clock

3. ADHERENCE RATE:
- "92%"
- "Excellent consistency!"
- 7-day moving average
- Icon: Target

4. HEALTH SCORE:
- "88/100"
- Color gauge (green)
- "+5 points this week"
- Icon: Heart with pulse

MAIN DASHBOARD (tabbed sections):

TAB 1 - OVERVIEW:

ACTIVITY CALENDAR:
- Month view calendar (heatmap style)
- Green intensity based on activity
- Darker green = more active
- Hover: Shows that day's details
- Click: Opens day detail modal
- Legend: 0, 1-2, 3-4, 5+ exercises

THIS WEEK'S PROGRESS:
Timeline view (vertical):
Monday:
- ✅ Morning Walk - 30 min
- ✅ Pregnancy Yoga - 15 min
- 💧 Water goal: 7/8 glasses
Tuesday:
- ✅ Strength Training - 20 min
- ⚠️ Skipped evening stretch
- 💧 Water goal: 8/8 glasses
(Continue for each day)

GOALS PROGRESS:
Cards for each goal with progress bars:
- "Walk 150 minutes per week"
  - Progress: 120/150 min (80%)
  - 3 more sessions needed
- "Complete 5 strength workouts"
  - Progress: 3/5 (60%)
  - 2 to go!

TAB 2 - EXERCISE ANALYTICS:

WORKOUT BREAKDOWN (donut chart):
- Cardio: 45%
- Strength: 30%
- Flexibility: 20%
- Balance: 5%
Legend with click to filter

MOST FREQUENT EXERCISES (ranked list):
1. Walking - 18 sessions, 9 hours total
2. Pregnancy Squats - 15 sessions
3. Cat-Cow Stretch - 12 sessions
(Show top 10)

EXERCISE INTENSITY DISTRIBUTION (bar chart):
- Low: 40% (green)
- Moderate: 50% (blue)
- High: 10% (orange)

TIME OF DAY PREFERENCE (radial chart):
- Morning: 60%
- Afternoon: 25%
- Evening: 15%
Insight: "You're a morning person! 🌅"

AVERAGE SESSION DURATION:
Line graph over time (last 30 days)
- Shows trend
- Markers for rest days

TAB 3 - NUTRITION ANALYTICS:

DIETARY ADHERENCE (gauge):
- 85% overall compliance
- Breakdown:
  - Foods to include: 90% ✓
  - Foods to avoid: 80% ✓

MACRO DISTRIBUTION (stacked bar chart by week):
- Protein
- Carbs
- Fats
Shows if within recommended ranges

MEAL TIMING CONSISTENCY:
Clock-style visual showing when meals are typically eaten
- Breakfast window
- Lunch window
- Dinner window

TOP CONSUMED FOODS (word cloud):
Bigger = more frequent
Oatmeal, Salmon, Broccoli, Almonds, etc.

HYDRATION TRENDS (area chart):
Daily water intake over 30 days
- Average line
- Target line
- Days below target highlighted

TAB 4 - HEALTH METRICS:

VITALS TRACKING (if logged):
Multiple line charts:
- Blood Pressure (if hypertension)
- Blood Sugar (if diabetes)
- Weight
- Resting Heart Rate
Each chart shows:
- Current value
- Trend (up/down/stable)
- Normal range zone (shaded)
- Doctor's target (dotted line)

SYMPTOM LOG:
Table showing:
- Date
- Symptom
- Severity (1-5)
- Notes
- Correlation with exercise/diet

MEDICATION ADHERENCE:
If tracking medications:
- Percentage taken on time
- Missed doses
- Refill reminders

TAB 5 - ACHIEVEMENTS:

BADGES EARNED:
Grid of achievement badges:
- 🥉 First Workout
- 🔥 7-Day Streak
- 💪 50 Exercises Completed
- 📈 Blood Sugar Improved
- 🎯 Monthly Goal Achieved
Each badge:
- Icon
- Name
- Date earned
- Description

MILESTONES (timeline):
- "First workout completed - Jan 5"
- "Completed 10 workouts - Jan 18"
- "30-day streak - Feb 4"
- "50 workouts milestone - Today!"

LEADERBOARD (optional, if enabled):
- Your rank
- Top 10 users (anonymous)
- Friendly competition mode

BOTTOM SECTION:

WEEKLY REPORT CARD:
Automated summary:
"This Week's Highlights:
✅ Completed 5/5 planned workouts
✅ Maintained 7-day streak
⚠️ Hydration below target 2 days
💪 New personal record: 25-min session
Focus Areas for Next Week:
- Drink more water
- Add one flexibility session
- Try prenatal yoga class"

EXPORT OPTIONS:
- Download PDF Report
- Share with Doctor
- Email Weekly Summary

INSIGHTS PANEL:
AI-generated observations:
- "Your morning workouts correlate with better adherence"
- "Rest days help you maintain consistency"
- "Consider adding more flexibility work"

DESIGN:
- Data visualization heavy
- Use charts library (Recharts)
- Color coding consistent throughout
- Interactive charts (hover, click, zoom)
- Date range selector (Last week, month, 3 months, year, all time)
- Export/share functionality
- Printable version
- Mobile: Swipeable cards for metrics
```

---

### Prompt 7: Mobile-First Exercise Quick Start Screen

```
Design a mobile-optimized quick start exercise screen for on-the-go workouts:

TOP BAR (fixed):
- Back button (left)
- "Quick Start" title (center)
- Profile icon (right)
- Thin colored line indicating condition (pregnancy: pink, diabetes: blue, etc.)

CONDITION CHIP (below header):
- Small badge: "Pregnancy - Trimester 2" with icon
- Swipeable to change condition quickly

QUICK START OPTIONS (large cards):

CARD 1 - START YOUR DAILY ROUTINE:
- Large gradient card (blue to purple)
- "15-Minute Morning Flow"
- Subtitle: "Energize your day"
- Preview: 3 small exercise thumbnails
- "Start Now" button (white)
- Time estimate: 15 min
- Difficulty: ⭐⭐☆☆☆

CARD 2 - CONTINUE WHERE YOU LEFT OFF:
- "You stopped at: Cat-Cow Stretch"
- Progress bar: 60% complete
- "Resume Workout" button
- Remaining time: 6 minutes left

CARD 3 - TODAY'S CHALLENGE:
- "✨ Daily Challenge: 5-Min Stretch"
- Streak indicator: "🔥 Keep your 7-day streak!"
- "Accept Challenge" button

RECENT WORKOUTS (horizontal scroll):
- Small cards showing recent routines
- "Yesterday: ✅ Morning Walk"
- "2 days ago: ✅ Strength Training"
- Tap to repeat

BROWSE BY TIME:
Chip buttons (horizontal scroll):
- 5 min
- 10 min
- 15 min
- 20 min
- 30 min
- 45 min+
Selected time shows filtered exercises below

BROWSE BY FOCUS:
Chip buttons:
- Full Body
- Upper Body
- Lower Body
- Core
- Flexibility
- Balance
- Breathing

SUGGESTED FOR YOU (scroll list):
Based on condition + history:
Each exercise card shows:
- Thumbnail/animation preview
- Exercise name: "Pelvic Floor Exercises"
- Duration: 10 min
- Difficulty: Beginner
- Benefits: "Prepares for labor"
- Favorite heart icon
- "Start" button (primary)
- "Info" button (i icon)

BOTTOM NAVIGATION (fixed):
- Home icon
- Exercises icon (active)
- Progress icon
- Profile icon

FLOATING ACTION BUTTON:
- Large "+" button (bottom right)
- Quick actions menu:
  - Log completed exercise
  - Add water
  - Quick note
  - Emergency contacts

SWIPE GESTURES:
- Swipe right: Go back
- Swipe left on card: Save for later
- Long press: Preview exercise

OFFLINE MODE INDICATOR:
If no internet: "📶 Offline - Showing saved workouts"

MOTIVATIONAL HEADER:
Rotating messages:
- "You're doing great! 💪"
- "Day 7 of your streak! 🔥"
- "Almost to your weekly goal!"

DESIGN:
- Large touch targets (min 44x44 pt)
- High contrast for readability
- Bottom navigation for thumb reach
- Card-based for easy scrolling
- Animations: Smooth slide transitions
- Pull to refresh
- Haptic feedback on actions
- Dark mode support
- Accessibility: VoiceOver labels
```

---

## Complete Disease-Specific Exercise Catalog

### Overview
This catalog contains 15 major health conditions with unique exercise requirements, totaling 120+ specific exercises.

---

### 1. Pregnancy (Trimester-Specific)

**First Trimester (Weeks 1-12)**
Focus: Energy conservation, nausea management, gentle movement
Exercises (8): Gentle Walking; Pelvic Tilts; Shoulder Rolls; Ankle Circles; Deep Breathing; Cat-Cow Stretch; Seated Leg Lifts; Wall Push-ups
Avoid: High-impact, lying flat on back after week 12, overheating

**Second Trimester (Weeks 13-26)**
Focus: Strength building, energy boost, balance
Exercises (10): Pregnancy Squats; Side Leg Raises; Modified Plank; Prenatal Yoga Flow; Swimming/Water Aerobics; Stationary Bike; Arm Circles with Light Weights; Kegel Exercises; Butterfly Stretch; Standing Hip Flexor Stretch
Avoid: Contact sports, risk of falling, exercises on back

**Third Trimester (Weeks 27-40)**
Focus: Labor preparation, comfort, stamina
Exercises (8): Pelvic Floor Exercises; Birth Ball Bouncing; Slow Walking; Wall Squats; Child's Pose; Tailor Sitting; Perineal Massage (guided); Breathing Techniques
Avoid: Lying on back, deep squats without support, overexertion

---

### 2. Diabetes (Type 1 & Type 2)

Focus: Blood sugar regulation, insulin sensitivity, weight management
Exercises (12): Brisk Walking; Resistance Band Training; Chair Squats; Wall Push-ups; Seated Marching; Bicep Curls; Leg Extensions; Step-Ups; Tai Chi; Swimming Laps; Cycling; Yoga for Diabetes
Timing: 30-60 min after meals
Avoid: Exercising with blood sugar <100 mg/dL or >250 mg/dL

---

### 3. Hypertension (High Blood Pressure)

Focus: Gradual cardio, stress reduction, no straining
Exercises (10): Moderate Walking; Light Jogging; Stationary Cycling; Water Aerobics; Dancing; Stretching Routine; Breathing Exercises; Gentle Yoga; Elliptical Training; Gardening
Avoid: Heavy weightlifting, holding breath, sudden intense exercise

---

### 4. Asthma

Focus: Controlled breathing, gradual intensity, warm-ups
Exercises (8): Swimming; Walking; Yoga; Cycling (Indoor); Volleyball; Diaphragmatic Breathing; Pursed-Lip Breathing; Pilates
Protocol: Warm up 10-15 min, inhaler nearby
Avoid: Cold dry air, high pollen areas, continuous high intensity

---

### 5. Arthritis (Osteoarthritis & Rheumatoid)

Focus: Joint mobility, reduce stiffness, low impact
Exercises (10): Water Walking; Gentle Range-of-Motion; Finger Exercises; Ankle Pumps; Shoulder Pendulum; Seated Knee Extensions; Tai Chi; Chair Yoga; Wrist Circles; Hip Marching (Seated)
Best Time: After morning stiffness subsides or warm bath
Avoid: High-impact activities, exercises during flare-ups

---

### 6. Parkinson's Disease

Focus: Balance, coordination, flexibility, freezing prevention
Exercises (10): Big Movements Walking; Boxing Training; Tango Dancing; Rock Steady Boxing; Balance Board Exercises; Vocal Exercises; Stretching Routine; Recumbent Bike; Yoga for Parkinson's; Face Exercises
Key: Large, deliberate movements; multitasking exercises
Avoid: Exercises with fall risk without support

---

### 7. Cardiac Rehabilitation (Post-Heart Attack/Surgery)

Focus: Gradual intensity increase, monitored progression
Phase 1 - Hospital: Bed Exercises; Sitting to Standing; Short Walks
Phase 2 - Outpatient: Monitored Treadmill; Stationary Bike; Light Arm Exercises; Breathing Exercises
Phase 3 - Maintenance: Moderate Walking; Light Strength Training; Swimming; Stretching
Critical: Monitor heart rate, stop if chest pain/dizziness

---

### 8. Chronic Back Pain (Lower Back)

Focus: Core strengthening, flexibility, posture
Exercises (10): Pelvic Tilts; Knee-to-Chest Stretch; Cat-Cow Stretch; Bird Dog; Bridge Exercise; Child's Pose; Wall Sits; Dead Bug; Swimming; McKenzie Extensions
Avoid: Toe touches, sit-ups, straight-leg lifts

---

### 9. Osteoporosis (Bone Density Loss)

Focus: Weight-bearing, balance, bone strengthening
Exercises (10): Walking; Stair Climbing; Wall Push-ups; Standing Leg Lifts; Heel Raises; Dancing; Light Weight Training; Balance Exercises; Resistance Band Rows; Tai Chi
Avoid: Forward bending, twisting, high-impact if severe

---

### 10. COPD (Chronic Obstructive Pulmonary Disease)

Focus: Breathing efficiency, endurance, oxygen use
Exercises (8): Pursed-Lip Breathing; Diaphragmatic Breathing; Arm Raises; Leg Marching (Seated); Wall Push-ups; Shoulder Blade Squeezes; Walking; Stationary Bike
Protocol: Use oxygen if prescribed, rest when needed
Avoid: Overexertion, holding breath, cold air exercise

---

### 11. Stroke Recovery

Focus: Regain mobility, balance, coordination
Early Stage: Passive Range of Motion; Sitting Balance; Ankle/Wrist Movements; Facial Exercises
Middle Stage: Sit-to-Stand Transitions; Assisted Walking; Arm Reach Exercises; Mirror Therapy; Weight Shifting
Late Stage: Treadmill with Support; Constraint-Induced Therapy; Fine Motor Practice; Balance Board

---

### 12. Thyroid Disorders

**Hypothyroidism (Underactive)**: Moderate Walking; Yoga; Swimming; Light Strength Training; Cycling; Pilates
**Hyperthyroidism (Overactive)**: Gentle Yoga; Slow Walking; Stretching; Tai Chi; Water Exercise

---

### 13. Anxiety & Depression

Focus: Mood improvement, stress reduction, endorphins
Exercises (10): Aerobic Walking; Jogging; Yoga; Dance; Boxing/Kickboxing; Swimming; Hiking in Nature; Group Fitness Classes; Martial Arts; Breathwork
Science: Exercise releases endorphins and serotonin

---

### 14. Liver Disease (Fatty Liver, Cirrhosis)

Focus: Weight loss (if overweight), low-intensity cardio
Exercises (8): Daily Walking; Cycling; Swimming; Yoga; Light Resistance Bands; Stretching; Water Aerobics; Tai Chi
Avoid: Contact sports (if cirrhosis), overexertion

---

### 15. Cancer Survivors (During & Post-Treatment)

Focus: Fatigue management, strength rebuilding, immunity
During Treatment: Short Walks; Gentle Stretching; Breathing Exercises; Light Yoga
Post-Treatment: Progressive Walking; Resistance Training; Swimming; Yoga; Cycling; Balance Exercises; Core Strengthening; Range of Motion
Special: Breast cancer survivors - avoid lymphedema triggers

---

### Summary Table

| Condition | # Exercises | Primary Focus | Intensity Level |
|-----------|-------------|---------------|-----------------|
| Pregnancy (T1) | 8 | Gentle, energy conservation | Low |
| Pregnancy (T2) | 10 | Strength, energy | Low-Moderate |
| Pregnancy (T3) | 8 | Labor prep, comfort | Low |
| Diabetes | 12 | Blood sugar control | Moderate |
| Hypertension | 10 | Gradual cardio | Low-Moderate |
| Asthma | 8 | Controlled breathing | Low-Moderate |
| Arthritis | 10 | Joint mobility | Low |
| Parkinson's | 10 | Balance, coordination | Moderate |
| Cardiac Rehab | 10 | Gradual progression | Low → Moderate |
| Back Pain | 10 | Core strength | Low-Moderate |
| Osteoporosis | 10 | Weight-bearing | Moderate |
| COPD | 8 | Breathing efficiency | Low |
| Stroke Recovery | 12 | Mobility restoration | Low → Moderate |
| Thyroid (Hypo) | 6 | Energy-appropriate | Moderate |
| Thyroid (Hyper) | 5 | Calming, gentle | Low |
| Mental Health | 10 | Mood improvement | Moderate-High |
| Liver Disease | 8 | Weight management | Low-Moderate |
| Cancer Recovery | 12 | Strength rebuilding | Low → Moderate |

Total: 15 conditions, 151 exercises

---

## HealthWise AI - Complete MVP Blueprint

### Problem Statement
Patients struggle to understand reports and lack personalized guidance on diet and exercise, leading to poor outcomes.

### Solution Overview
HealthWise AI analyzes reports with Gemini AI and provides personalized recommendations, diets, and exercises tailored to each condition.

### Tech Stack
- Frontend: React + Tailwind
- AI: Google Gemini API
- Animations: Lottie/React Spring
- Storage: localStorage (MVP) / Firebase (prod)
- File processing: pdf.js
- Timer: Custom React component

### System Architecture
User Interface Layer (Uploader, Analysis Dashboard, Recommendations, Exercise Library, Progress Tracker)
AI Processing Layer (Gemini integration, analysis, recommendation generator)
Data Layer (Profiles, History, Exercise Library, Nutrition DB)

### Core Features (MVP)
- Intelligent Report Analyzer (upload → parse → Gemini → structured output)
- Personalized Recommendations Engine (DOs, DON'Ts, diet, lifestyle)
- Visual Exercise Library with animations and safety notes
- Interactive Exercise Player (timers, controls, overlays)
- Personalized Dashboard (summary, today’s recs, progress, quick actions)

### Key Functions
- `reportAnalyzer(file)`: validate, extract text, detect type, send to Gemini, parse structured findings; handle errors/retries.
- `generateRecommendations({reportAnalysis, userProfile})`: produce DOs, DON'Ts, diet (include/avoid), lifestyle; consider allergies and meds.
- `getExerciseRoutine({condition, fitnessLevel, duration})`: select warm-up/main/cool-down, rest periods, safety flags.
- `exerciseTimer(state)`: play/pause/skip/complete sets, rest handling, audio/vibration cues, auto-advance.
- `nutritionTracker`: meal logging vs plan, adherence scoring, alternatives.
- `progressMonitor`: track exercise/diet adherence, symptoms, vitals trends, badges, streaks.

### Database Sketch (MVP)
Users: profile (conditions, allergies, meds), reports (analysis, recommendations, fileUrl), exerciseHistory, nutritionLogs.

### UI/UX Principles
- Color coding: Red=warning, Green=safe, Yellow=caution, Blue=info
- Accessibility: high contrast, large fonts, voice-over labels, emergency button
- Mobile-first: responsive, touch-friendly, offline for exercises, notifications

### Implementation Roadmap (4 weeks)
1) Foundation: React setup, Gemini API, uploader, layout
2) Core: analyzer, recommendations, exercise library (10+), timer
3) Polish: animations, dashboard, testing
4) Demo: mock data, deploy, record demo

### Safety & Compliance
- Disclaimers: not medical advice; consult doctor; emergency call instructions
- Data privacy: local processing for MVP; consent; deletion options

### Bonus Ideas (if time)
Chatbot Q&A, medication reminders, community, telemedicine, wearables, family sharing, multilingual.

### Sample Gemini Prompts
- Report analysis JSON output with findings, risk, actions, foods, doctor triggers.
- Exercise routine generation by condition/trimester with warm-up/main/cool-down, safety tips.

### Demo Script Outline
Upload sample → AI analysis → show personalized recs → start exercise with timer → show progress → switch condition → recap.

### Pre-Hackathon Checklist
- Gemini key tested
- React deps installed
- 10 animations sourced
- Sample reports ready
- Mockups prepared
- Backup mock responses
- Pitch deck outline
- Demo env tested

