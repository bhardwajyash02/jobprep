# 2-WEEK INTERVIEW PREP PLAN

## OVERVIEW
Goal: Go from "decent candidate" to "standout candidate" in 14 days.

**Assumption**: You have 5+ years data engineering experience and are reasonably solid. This plan helps you:
- ✅ Master Visa-specific pain points
- ✅ Prepare compelling stories and answers
- ✅ Learn any specific gaps
- ✅ Build confidence for the interview

**Time commitment**: 10-12 hours/week (1.5 hours/day)

---

## WEEK 1: RESEARCH, STORIES, FUNDAMENTALS

### Day 1-2: Deep Dive into Visa & Payments (2 hours)
**Goal**: Sound knowledgeable about the domain.

**Research**:
- [ ] Read: Visa's official blog on payment processing (5 min)
  - Link: https://www.visa.co.in/about-visa/latest-press-releases.html
  - Focus: Recent innovations, tech challenges, scale
- [ ] Read: "How Visa Handles Billions of Transactions" (Medium/LinkedIn posts) (15 min)
  - Search: "Visa data infrastructure" OR "Visa Consulting Analytics"
- [ ] Watch: "Modern Payment Systems Architecture" (YouTube, 15 min)
  - Links: 
    - https://www.youtube.com/watch?v=FPp_ZKx3pHY (Payment Systems)
    - https://www.youtube.com/watch?v=Hqqq0kxE2RA (Fintech Infrastructure)
- [ ] Read: Articles on PSD2, open banking, real-time payments (10 min)
  - Understand the landscape Visa operates in

**Takeaway doc**:
- Create a 1-page summary: "Visa's Business Challenges & Opportunities"
  - List 3-5 technical problems Visa likely faces
  - Link each to data engineering

**Example output**:
```
Visa's Challenge #1: Real-time Fraud Detection
- Problem: Prevent fraudulent transactions in <100ms
- Data Engineering: Build real-time pipeline ingesting from global merchants
- Technologies: Kafka, ML model serving, <50ms latency requirement

Visa's Challenge #2: Global Scale with Local Compliance
- Problem: 200+ countries, different regulations (PSD2, RBI)
- Data Engineering: Data residency, compliance, audit trails
- Technologies: Multi-region data lakes, governance framework
```

---

### Day 3-4: Identify Your Best Stories (2 hours)
**Goal**: Have 5-6 strong project examples you can adapt to different questions.

**Exercise**: List 8-10 projects you've worked on. For each, fill in:
| Project | Scale (data size) | Key Challenge | Technology | Business Impact |
| --- | --- | --- | --- | --- |
| ETL Migration | 100GB | Query latency | Spark, Airflow | 50% faster reporting |
| ML Pipeline | 50GB | Model serving | Python, Kafka | 2M customers reached |

**Then narrow to top 5**:
- **Story #1: Scale** (biggest data project)
- **Story #2: Production** (worst production incident)
- **Story #3: Optimization** (performance improvement with numbers)
- **Story #4: Collaboration** (working across teams)
- **Story #5: Learning** (learning a new tool/framework)

**For each story, write STAR bullets** (30 sec to 2 min each):
- **S**: Situation (what was the problem?)
- **T**: Task (what was your role?)
- **A**: Action (what did you do? specific decisions, not just "I worked hard")
- **R**: Result (what changed? numbers!)

**Example**:
```
STORY: Scale
S: Company had 10M daily transactions, but reporting took 24 hours (needed <1 hour)
T: Lead data engineer, owned the pipeline redesign
A: Profiled existing Spark job, found 85% time on one shuffle. Repartitioned data, 
   added caching, tuned Spark config (memory, partitions)
R: Latency improved from 24h to 2h. Now 50+ teams use real-time dashboards daily.
```

**Video resource**: How to craft STAR stories
- https://www.youtube.com/watch?v=fGdC7Ae1ICQ (2:30 min)

---

### Day 5-6: Study Technical Concepts (2 hours)
**Goal**: Fill gaps in distributed systems, performance tuning, architecture.

**Pick 2 of these based on your weaknesses**:

#### Option A: Distributed Systems Fundamentals (1 hour)
- **Read**: "Designing Data-Intensive Applications" Ch. 1-2 (45 min read)
  - Free summary: https://blog.bytebytego.com/p/designing-data-intensive-applications
  - Focus: CAP theorem, consistency models, replication
- **Watch**: "Distributed Systems Crash Course" (15 min)
  - https://www.youtube.com/watch?v=p7-gST0Xczg

#### Option B: Performance Tuning (1 hour)
- **Read**: "Spark Tuning Guide" (official docs, 30 min)
  - https://spark.apache.org/docs/latest/tuning.html
  - Focus: memory tuning, shuffle operations, partitioning
- **Watch**: "Optimizing Spark Jobs" (30 min)
  - https://www.youtube.com/watch?v=9Kcs3vZxLAM

#### Option C: Cloud Architecture (1 hour)
- **Read**: Cloud migration case study (AWS, GCP, or Azure)
  - AWS example: https://aws.amazon.com/solutions/case-studies/
  - Pick one similar to your background
- **Watch**: "On-Prem to Cloud Migration Strategy" (30 min)
  - https://www.youtube.com/watch?v=_R6gwZt36Q8

#### Option D: Data Quality & Governance (1 hour)
- **Read**: "Great Expectations" intro (30 min)
  - https://docs.greatexpectations.io/docs/
- **Watch**: "Data Quality Frameworks" (30 min)
  - https://www.youtube.com/watch?v=7s8j8h5p3Bc

---

### Day 7: Practice Interview Answers (2 hours)
**Goal**: Deliver answers smoothly without sounding scripted.

**Exercise**:
- [ ] Pick 5 hardest questions from `02_20_INTERVIEW_QUESTIONS.md`
- [ ] Write out answers (using STAR format for behavioral questions)
- [ ] Record yourself (phone, camera, or Zoom) answering each (2 min max each)
- [ ] Watch playback, critique:
  - Do you speak clearly or mumble?
  - Do you use "umm" or "uh"? (Try to minimize)
  - Do you sound confident or apologetic?
  - Are your examples specific with numbers?

**Resources**:
- https://www.youtube.com/watch?v=S4w3V7vf_3Q (Interviewing tips, 7 min)

**Deliverable**: 5 videos of yourself answering questions (for your own review)

---

## WEEK 2: DEEP DIVES & FINAL PREP

### Day 8-9: Technical Deep Dive (2 hours)
**Goal**: Master 3 specific technologies Visa uses.

**Pick based on JD** (likely priorities):
1. **Spark/PySpark** - Non-negotiable (1 hour)
   - [ ] Review Spark architecture (DAGs, RDDs, lazy evaluation)
   - [ ] Write 2-3 small PySpark scripts (join, aggregation, window function)
   - [ ] Understand common optimizations: partitioning, caching, broadcast joins
   - [ ] Practice: Build a simple ETL script that handles 1M+ records
   - **Video**: https://www.youtube.com/watch?v=5d23i9QYbTc (1 hour Spark fundamentals)

2. **Cloud Platform** (AWS / GCP / Azure) - 30 min
   - [ ] Review data services (S3, Snowflake, BigQuery, etc.)
   - [ ] Understand cost models and trade-offs
   - [ ] Know at least 1 migration strategy
   - **Video**: https://www.youtube.com/watch?v=G5_GX9L4WKo (AWS for Data, 30 min)

3. **Data Pipeline Orchestration** (Airflow / dbt) - 30 min
   - [ ] Understand DAG concepts
   - [ ] Know how to handle failures, retries, dependencies
   - [ ] Review one case study of a production pipeline
   - **Video**: https://www.youtube.com/watch?v=cHLV0kK5D_s (Airflow fundamentals, 30 min)

---

### Day 10-11: Tough Questions Practice (2 hours)
**Goal**: Handle the hardest, most likely questions with confidence.

**Session 1: Tech Questions** (1 hour)
- [ ] Answer questions 1-4 from Section A (Technical)
- [ ] Write detailed answers, covering:
  - Specific architecture decisions
  - Trade-offs considered
  - Metrics/numbers
- [ ] Identify weaknesses in your answer
- [ ] Revise

**Sample Question**: "Design a data pipeline to handle 10 billion transactions per day"
- Your answer should cover:
  - Data sources (APIs, databases)
  - Ingestion strategy (batch vs. stream)
  - Storage (data lake architecture, partitioning)
  - Processing (Spark, batch/real-time)
  - Serving (who uses the data? How?)
  - Monitoring and SLAs

**Session 2: Behavioral + Situational** (1 hour)
- [ ] Answer questions 9-13 (behavioral)
- [ ] Answer questions 14-17 (situational)
- [ ] Practice explaining your thinking aloud
- [ ] Record one STAR answer (2 min)

**Resource**: 
- https://www.youtube.com/watch?v=SO3-L5LCgMY (STAR method deep dive, 5 min)

---

### Day 12-13: Research Company Culture & Final Q&A (1.5 hours)
**Goal**: Show genuine interest and ask thoughtful questions.

**Company Research**:
- [ ] Read Visa's recent press releases (5 min)
- [ ] Check Visa's tech blog / engineering posts (10 min)
- [ ] Look at Glassdoor reviews (focus on engineering culture, 10 min)
- [ ] Search LinkedIn for current/former Visa engineers (see career progression)
- [ ] Find Visa's tech stack mentions on StackShare or similar (5 min)

**Questions Prep**:
- [ ] Review `05_QUESTIONS_FOR_INTERVIEWER.md`
- [ ] Pick 3-4 questions that resonate most
- [ ] Customize with company research (mention specific initiatives, challenges)
- [ ] Practice asking them naturally (not robotic)

**Example customization**:
Instead of: "What are pain points in your infrastructure?"
Better: "I saw Visa recently announced [initiative]. How is your team enabling that? What infrastructure challenges come with [initiative]?"

---

### Day 14: Final Review & Confidence Building (2 hours)
**Goal**: Feel ready, not panicked.

**Checklist**:
- [ ] Review your 5 best stories (STAR format)
- [ ] Answer 5 random questions from Section A (technical)
- [ ] Answer 5 random questions from Section B-D (behavioral/situational)
- [ ] Review 3 questions you'd ask the interviewer
- [ ] Mock interview with friend (30 min)
- [ ] Get feedback, adjust

**Final preparation**:
- [ ] Get good sleep (last 3 days before interview)
- [ ] Prepare what to wear (professional, not overly formal for tech)
- [ ] Prepare logistics (check time zone if remote, test camera/audio if video)
- [ ] Prepare talking points (Visa's scale, your enthusiasm, specific examples)

**Day before**:
- [ ] Don't cram new information
- [ ] Review your stories (just skim, not deep study)
- [ ] Prepare 3 wins you want to mention
- [ ] Get 8 hours sleep
- [ ] Eat well, exercise if you can

**Day of**:
- [ ] Arrive 15 min early (if in-person)
- [ ] Calm breath exercises (2 min before interview)
- [ ] Smile when you meet them (changes your tone)
- [ ] Listen more than you talk
- [ ] Ask for clarification if confused
- [ ] Show enthusiasm for the problems they're solving

---

## LEARNING RESOURCES SUMMARY

### Free Resources
- **YouTube Channels**:
  - [Databricks Academy](https://www.youtube.com/@databricks-academy) - Spark tuning, MLOps
  - [Data Engineering Simplified](https://www.youtube.com/@learndataeng) - Data pipeline design
  - [Seattle Data Guy](https://www.youtube.com/@SeattleDataGuy) - Architecture, interviews
  - [ByteByteGo](https://www.youtube.com/@ByteByteGo) - System design fundamentals

- **Blogs & Articles**:
  - [Engineering at Uber](https://eng.uber.com/data/) - Real-world data challenges
  - [Stripe Engineering](https://stripe.com/blog/engineering) - Payment systems
  - [LinkedIn Engineering Blog](https://engineering.linkedin.com/blog) - Large-scale systems
  - [Databricks Blog](https://www.databricks.com/blog) - Spark optimization

- **Documentation**:
  - Apache Spark official docs: https://spark.apache.org/docs/latest/
  - AWS Data Architecture: https://aws.amazon.com/solutions/
  - Great Expectations: https://docs.greatexpectations.io/

### Paid Resources (if you want to level up fast)
- **Courses** (~$50-200):
  - [Coursera: Data Engineering with Python](https://www.coursera.org/learn/data-pipelines-systems)
  - [Udacity: Data Engineer Nanodegree](https://www.udacity.com/course/data-engineer-nanodegree--nd027)
  - [DataCamp: Data Engineering Tracks](https://www.datacamp.com/tracks/data-engineer)

- **Books**:
  - "Designing Data-Intensive Applications" by Martin Kleppmann
  - "The Art of Scalability" by Martin Abbott & Michael T. Fisher
  - "Machine Learning Systems Design" by Chip Huyen

---

## WEEKLY SCHEDULE (Quick Reference)

### Week 1
| Day | Topic | Time | Deliverable |
| --- | --- | --- | --- |
| 1-2 | Visa Research | 2h | 1-page summary |
| 3-4 | Story Mining | 2h | 5 STAR stories |
| 5-6 | Tech Concepts | 2h | Notes on chosen topic |
| 7 | Practice Answers | 2h | 5 recorded videos |
| **Week 1 Total** | | **10h** | |

### Week 2
| Day | Topic | Time | Deliverable |
| --- | --- | --- | --- |
| 8-9 | Technical Deep Dive | 2h | PySpark scripts, architecture notes |
| 10-11 | Tough Questions | 2h | Written answers + 1 recorded video |
| 12-13 | Company Research & Q&A | 1.5h | 3-4 customized questions |
| 14 | Final Review & Mock | 2h | Feeling confident, zero anxiety |
| **Week 2 Total** | | **7.5h** | |

**Grand Total: 17.5 hours over 2 weeks (1.25 hours/day)**

---

## SUCCESS METRICS

By the end of Week 2, you should:
- ✅ Deliver 5 compelling stories with specific numbers and impact
- ✅ Answer any technical question with a well-reasoned architecture or approach
- ✅ Explain your gap areas honestly without sounding unprepared
- ✅ Ask 3-4 thoughtful questions about the role/team/company
- ✅ Show enthusiasm for Visa's mission and technical challenges
- ✅ Speak clearly and confidently, minimal "umms" and "uhs"

**Red flag if you're NOT ready**: You can't recall one specific story with numbers, or you sound unsure about Spark/cloud concepts. If so, extend prep another week.

---

## DAY-OF INTERVIEW TIPS

1. **Arrive early** (15 min buffer)
2. **Smile** before they see you (changes your tone)
3. **Listen to the full question** before answering
4. **Pause to think** (2 seconds is okay, better than rambling)
5. **Give SPECIFIC examples** with numbers ("50% improvement" > "much better")
6. **Turn the conversation back**: "That's why I'm excited about this role..."
7. **Ask clarifying questions** if confused ("Am I understanding correctly...?")
8. **Tell stories, don't recite facts** (people remember stories, not bullet points)
9. **Avoid negating former employers** (professional, always)
10. **At the end**: "When would I hear back? Is there anything else you'd like to know?"

---

## IF YOU'RE NERVOUS

**Remember**:
- They WANT you to succeed (hiring is hard, they'd rather not repeat this)
- You have 5+ years experience (you belong in the room)
- Admitting gaps > pretending to know everything
- Most candidates are less prepared than you will be after this plan

**Breathe** (4 count in, 6 count out, 3 times before starting)

You've got this. 🚀
