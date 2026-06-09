# 7 SMART QUESTIONS TO ASK THE INTERVIEWER

## Why Ask Questions?
- **Shows genuine interest**: You're interviewing them too, not just selling yourself
- **Signals strategic thinking**: You ask about architecture, challenges, team dynamics (not just perks)
- **Gathers real info**: Helps you decide if this is actually a good fit
- **Impresses them**: Most candidates ask 0-2 questions. Asking 4-5 smart ones stands out
- **Prevents regret**: You learn what you're actually signing up for

---

## THE 7 QUESTIONS

### 1. **"Tell me about the current state of Visa's data infrastructure in AP. What's working well, and where are the biggest pain points your team is tackling right now?"**

**Why this is smart**:
- Shows you're thinking about real problems, not just job title
- "Pain points" reveals what's urgent (high signal for what you'd work on)
- Their answer tells you if this is maintenance work or building new things
- Demonstrates you understand you'd be joining a specific team context

**What good answers sound like**:
- ✅ "We're migrating from on-prem Hadoop to cloud, and the tricky part is managing dual systems during the transition"
- ✅ "Data quality issues from partner integrations—coordinating with 20 different data sources is a mess"
- ✅ "We're great at batch pipelines but real-time is underdeveloped. ML models need sub-5-minute latency"

**What red flags sound like**:
- ❌ "Everything is great, no real pain points" (sounds like they don't care about improving)
- ❌ "I don't know" (bad sign for a hiring manager)
- ❌ Complaints about the team (blame culture vs. problem-solving)

**Follow-up if needed**: "Which of these pain points would the new engineer be helping solve?"

---

### 2. **"What does the ideal trajectory look like for this role? Are you seeing this as someone staying for 3-5 years and growing into a team lead or architect role, or more of a steady-state IC (individual contributor) position?"**

**Why this is smart**:
- Signals you're thinking long-term, not job-hopping
- Helps you understand promotion paths and growth at Visa
- Shows maturity: some people want stability, others want rapid advancement
- Their answer reveals company investment in talent development

**What good answers sound like**:
- ✅ "This role typically grows into tech lead within 2-3 years, then principal engineer or architect"
- ✅ "We have strong IC track record. You can go deep in infrastructure and grow without managing people"
- ✅ "We invest in people—expect training budget, certifications, conference attendance"

**What red flags sound like**:
- ❌ "We'll see how it goes" (no clear career path)
- ❌ "You'll be on-call forever, no real progression" (burnout signal)
- ❌ "Promotion depends entirely on politics" (bad culture)

---

### 3. **"What's your team's approach to technical debt and infrastructure upgrades? How do you balance new feature work with platform improvements?"**

**Why this is smart**:
- **Data engineers live in this tension**: Building new pipelines vs. maintaining/optimizing old ones
- Shows you understand that software requires maintenance
- Reveals team's engineering maturity (do they care about code quality?)
- Helps you know if you'd spend 50% on boring infrastructure or have time for innovation

**What good answers sound like**:
- ✅ "We allocate 20% of our sprint to tech debt. Quarterly platform upgrade sprints"
- ✅ "We measure technical debt in terms of maintenance cost and pay it down systematically"
- ✅ "New features are blocked if they don't meet performance standards. We have a review process"

**What red flags sound like**:
- ❌ "We don't have time for tech debt—too many feature requests" (burnout incoming)
- ❌ "Tech debt is someone else's problem" (toxic culture)
- ❌ No metrics or processes for tracking it (chaotic)

**Follow-up**: "If I were to join, what would be the first infrastructure problem you'd want me to tackle?"

---

### 4. **"How does your team approach collaboration with data scientists? How do you handle requests for new tools, frameworks, or architectural changes?"**

**Why this is smart**:
- JD mentions "Support platform upgrades" and "Collaborate with data scientists"
- Reveals team dynamics and how much you'd be in meetings (or autonomous)
- Shows if they listen to technical input or just execute orders
- Visa's team is distributed (AP region): you need to understand async collaboration patterns

**What good answers sound like**:
- ✅ "Weekly sync with the data science team. We prioritize infrastructure work based on their roadmap, but also push back on unrealistic asks with data"
- ✅ "We have a technical steering committee that reviews new tool adoption. Anyone can propose, we evaluate together"
- ✅ "Data scientists own their use cases; we own the platform. We design APIs together"

**What red flags sound like**:
- ❌ "Data scientists request, we build. No pushback" (you become a build monkey)
- ❌ "Data scientists don't understand infrastructure; they just complain" (disrespect, silos)
- ❌ "We make all decisions top-down" (no team input)

---

### 5. **"What does the onboarding process look like for a new engineer? How long before I'm expected to be productive? What's the mentorship structure like?"**

**Why this is smart**:
- Shows you care about setting up for success (not just "I'll figure it out")
- Reveals team maturity (do they invest in onboarding or throw you in?)
- Signals you're thinking long-term: good onboarding = more likely to stay
- At global company (AP region), you want to know about time zone collaboration and support

**What good answers sound like**:
- ✅ "Week 1: environment setup, system architecture overview. Week 2-3: first small contribution. Month 1-2: main project. We assign a mentor from the team"
- ✅ "We have documented onboarding guides, Slack channel for new hires, and async-friendly communication since we're distributed"
- ✅ "We expect 3 months to full productivity. Ramping engineers pair with experienced ones"

**What red flags sound like**:
- ❌ "Figure it out yourself" (chaotic, no support)
- ❌ "You should be productive in week 1" (unrealistic expectations)
- ❌ No documentation or mentorship (learning on your own)

---

### 6. **"How do you measure success for this role? What metrics or outcomes would indicate that someone is excelling in this position after their first year?"**

**Why this is smart**:
- Shows you're goal-oriented and want clear success criteria
- Helps you understand if they care about: code quality, velocity, innovation, reliability, or just shipping features
- Reveals their values: "number of pipelines deployed" vs. "reduced query latency by 50%"
- Prevents you from working toward the wrong things

**What good answers sound like**:
- ✅ "First 6 months: deliver a working cloud migration of System X. Year 1: Platform reliability hits 99.95% SLA, query latency improved 40%"
- ✅ "Success is: mentoring junior engineers, reducing on-call load by 30%, establishing monitoring for all pipelines"
- ✅ "OKRs are collaborative. We define quarterly goals together based on business needs"

**What red flags sound like**:
- ❌ "I don't know" (disorganized management)
- ❌ "Just maintain the status quo" (no growth opportunity)
- ❌ "Whatever your manager decides" (no agency)

---

### 7. **"What's the biggest challenge your team faced in the last year, and what did you learn from it? How has that shaped your approach to building the team now?"**

**Why this is smart**:
- Shows vulnerability and reflection (mature leader = better team)
- Tells you about real challenges you might face
- Signals if they learn from mistakes or repeat them
- Gives insight into their leadership philosophy
- Personal touch: makes the interview feel like a conversation, not an interrogation

**What good answers sound like**:
- ✅ "We had a major data corruption issue from a migration. Taught us to invest heavily in validation and testing. Now we have a QA environment that mirrors production"
- ✅ "We were siloed between infrastructure and data science. Had to establish communication patterns and shared goals. Now we're much better at collaborating"
- ✅ "We burned out an engineer trying to do everything. Learned to distribute load and hire more specialists. Now we're intentional about workload"

**What red flags sound like**:
- ❌ "No major challenges" (either lying or nothing interesting happens)
- ❌ "It was all someone else's fault" (no ownership)
- ❌ "We just moved on" (no learning culture)

---

## HOW TO DELIVER THESE QUESTIONS

### Timing
- **Usually at the end**: "Do you have any questions for me?" ← That's your cue
- **Time limit**: You probably have 10-15 minutes. Ask 3-4 questions max (1 follow-up each)
- **If you have multiple interviews**: Save the deeper questions for the hiring manager or team lead (not the recruiter screening call)

### Delivery (Tone & Style)
- **Conversational**: "I'm curious about [topic]..." NOT "Interrogate me about..."
- **Genuine curiosity**: You actually want to know, not just checking a box
- **Listen actively**: Take notes, respond to their answer, ask follow-ups
- **Collaborative**: "If I were on your team, how would I..." NOT "Why don't you..."

### What to Do with Answers
- **Write them down**: You're doing research on whether this is a good fit
- **Evaluate fit**: Does this align with what you want in a job?
- **At next round**: "Based on what [person] said about [topic], I have a follow-up question..."
- **If red flags**: It's okay to walk away. Bad team fit = bad experience, no matter the title

---

## BONUS: QUESTIONS TO AVOID

❌ **"What's the salary?" or "How much PTO do I get?"** — Recruiters handle this, not interviewers. Comes across as mercenary.

❌ **"Do you like working here?" or "How do you like your boss?"** — Puts them on the spot. Boring answer incoming.

❌ **"Why did the last person leave?"** — Could be personal, not professional. Skip it.

❌ **"What's your biggest competitor?"** — Generic, not about your team/role.

❌ **"Do you have any concerns about my background?"** — Defensive. If they do, they'll tell you during hiring decision. Don't force it early.

---

## SAMPLE CONVERSATION FLOW

**Interviewer**: "Great questions so far. Do you have anything for me?"

**You** (pause, reference notes): "Actually, a couple. I was curious about something you mentioned earlier about the cloud migration. How is that impacting your team's day-to-day? Are you running both systems in parallel, or phasing it out?"

**Interviewer** (explains): "We're dual-running for the next 6 months..."

**You** (follow-up): "That sounds complex. How are you handling data consistency between systems? That's something I'd want to understand better if I joined."

**Interviewer** (details): "Good question. We have reconciliation jobs that..."

**You** (next question): "Thanks for walking me through that. One more: what would you say is the biggest bottleneck for the team right now?"

**Interviewer** (answers)...

**You** (closing): "Thanks, this gives me a much better sense of what I'd be working on. Really appreciate your time."

---

## FINAL TIPS

1. **Personalize**: Use details from the JD, conversation, or Visa's recent news
2. **Listen more than you talk**: Interview is 60/40 them/you
3. **Take notes**: Shows you care, helps you remember
4. **No "gotcha" questions**: You're collaborating, not testing them
5. **Save the best for last**: Most important question should be second-to-last so you end on a high note

**Goal**: They should feel like you're genuinely interested in solving the right problems at the right place, not just collecting offer letters.
