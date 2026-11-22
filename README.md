This website is awesome!!! -SH

# Try a Day: open items to review and revise

Try a Day is a career exploration app for students, with a separate section for parents and guardians. This file lists what still needs checking, what we parked for later, and what the school's tech team needs to know.

- **Live version:** https://claude.ai/artifact/FFDKy5hgW3WWyrb696hpag (updates whenever changes are published)
- **School copy:** `try-a-day.html`, one self-contained file. It is a snapshot, so request a new copy after any change.

---

## 1. Review with the counselor's office

I wrote these from general knowledge, not official sources. Each needs a check before students and families rely on it.

### Student content
- [ ] **Training steps for all 51 careers.** Each career has three steps: junior year, senior year and after graduation. The labels change with the student's grade.
- [ ] **"Good to know" application tips**, one per career.
- [ ] **Classes, clubs and high school types by career group** (8 groups), shown to middle school, 9th and 10th grade students. The counselor may want to swap in programs your district actually offers.
- [ ] **Program descriptions** in "Explore the world and your interests" (12 programs) and "Pay for college and get ready" (8 programs). Check eligibility wording, especially SEO Scholars (which areas it serves) and QuestBridge (income and academic requirements).
- [ ] **The 21 careers marked "New to me."** I chose which careers count as lesser-known.
- [ ] **Which career group each career belongs to.** This drives browsing and the class and program suggestions.

### Parent and guardian content
- [ ] **Adult next steps.** These are written by training type (apprenticeship, short program, college, graduate school), not job by job.
- [ ] **"How you can help" tips for parents**, also written by training type.
- [ ] **Typical tasks for 32 common jobs** that aren't career pages, such as cashier, CNA, office manager and stay-at-home parent.
- [ ] **Task guesses from 17 job-title keywords**, such as "manager," "driver" or "technician."
- [ ] **The 18 everyday activities** in the parent "narrow it down" path, and the skills each one maps to.
- [ ] **"Similar jobs" suggestions** for jobs the app doesn't have (104 search terms). For example, "lawyer" suggests interpreter, social worker and HR specialist.

---

## 2. Data to verify and update every year

- [ ] **Pay figures.** All 51 use U.S. Bureau of Labor Statistics median pay for May 2025, rounded. Update them each year when BLS releases new figures.
  - Five figures came from sites republishing BLS data, not bls.gov itself. Check these first: **software developer, power line worker, logistics coordinator, farm or ranch manager, animal trainer.**
  - Several figures cover a wider BLS group, and the cards say so: police (includes detectives), paramedic (includes EMTs), ship's officer (all water transportation workers), occupational therapy assistant (includes aides).
- [ ] **The budget screen** (second opening screen):
  - Rent and utilities, $1,500: Census Bureau median gross rent, 2024 ($1,487). Consider using local rent instead.
  - Groceries, $350: USDA low-cost food plan, 2026, taken from a secondary source. Confirm against USDA's own table.
  - Car, $500 a month: my estimate for a used car.
  - Take-home pay: my estimate, counting federal taxes only.
- [ ] **Adult fact screens:** World Economic Forum Future of Jobs Report 2025 (39%), Department of Labor apprenticeship data for fiscal 2021 (3 in 5 apprentices 25 or older; average age about 30), and LinkedIn surveys (62% have taken a career break).
- [ ] **Program links and deadlines.** Check the links for all 20 programs once a year. Deadlines move; NSLI-Y and YoungArts both changed dates between years.
- [ ] **Gallup report statistics** are paraphrased with credit, because the report's copyright notice restricts quoting. Ask Gallup for permission before quoting it directly.

---

## 3. Features parked for later

1. **Credentials and expertise for adults.** "Plan for me" treats a job as everyday tasks, so it undersells people with degrees and licenses, such as a speech-language pathologist.
   - Ideas: (a) ask about highest education or license and its field, and count that schooling as done; (b) ask what they know deeply, such as health, language, children or law; (c) for licensed professionals, explain that upskilling usually means a specialty certification, supervising or private practice, and point to their professional association; (d) add professional jobs to the built-in list.
   - Recommended: (a) and (c) together.
2. **Link programs to the jobs a student saves.** Each explore program is already tagged with the career groups it fits (study abroad with travel and the world, art programs with design and creativity, and so on). Next step: show "Fits jobs you saved" and put those programs first.
3. **Grade level for parents planning for a child.** Parent pages say "Junior year" instead of assuming 11th grade. With several children, each child could have a grade.
4. **More careers.** Requested or likely popular: lawyer, mechanical engineer, chef, hairstylist, pharmacist, speech-language pathologist.
5. **Real artwork.** The workday scenes are simple placeholder illustrations drawn in code.
6. **Local information.** Local rent on the budget screen, and the district's own high schools, CTE programs and dual enrollment.

### Ideas not yet discussed
- An accessibility review with students who use screen readers.
- A Spanish version for families.
- A live job lookup that asks Claude. This would need each viewer to sign in and approve it, and wouldn't work in the school's file, so the built-in lists are the default.

---

## 4. Notes for the tech team

- **One self-contained file.** The only outside request is for two Google Fonts; if it's blocked, the app falls back to standard fonts.
- **Nothing is stored or sent.** No accounts, no tracking. Students copy or email their report before closing the page. If accounts are ever added, student privacy laws (COPPA, FERPA) and district rules apply.
- **Link back in emailed reports.** It points to the live claude.ai link. On the school's own website, it automatically links to that page instead. To set it by hand, edit the `SITE_URL` line in the code.
- **Email buttons** open Gmail, Outlook or the computer's email app with everything filled in. Nothing is sent until the student presses Send. "Copy the email instead" is the backup.
- **External links** to programs, Google searches and email open in a new tab.
- **Where content lives in the code**, for anyone editing directly:

| What | Name in the code |
|---|---|
| Careers (pay, day, steps, skills) | `CAREERS` |
| Opening screens | `INTRO` |
| Career groups | `CATS` |
| Classes, clubs, school types | `PREP` |
| Explore programs | `EXPLORE` |
| College prep and financing | `COLLEGE` |
| Common adult jobs and tasks | `COMMON` |
| Job-title keywords | `KEYWORDS` |
| Search terms and similar jobs | `ALIAS` |
| Parent activity list | `ACTS` |
| Adult fact screens | `MFACTS` |
| "New to me" careers | `RARE` |
