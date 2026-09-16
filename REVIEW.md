# Repository Review and Improvement Record

## Main strengths of the original repository

- The original interface was clean, responsive, and easy to navigate.
- It already randomized both questions and answer positions.
- It supported saved sessions, flags, keyboard navigation, progress tracking, and a results screen.
- The original 200-question bank covered the main Introduction to Law themes reasonably broadly.

## Main issues found

1. **The question bank was embedded inside the HTML.**  
   This made the file difficult to review, maintain, proofread, or expand.

2. **Two almost identical HTML files were present.**  
   `index.html` and `main.html` created uncertainty about which file classmates should open and increased the risk of inconsistent updates.

3. **The full-bank size was hard-coded in several places.**  
   Text, buttons, assertions, and event handlers referred specifically to 200 questions, so expanding the bank required multiple manual changes.

4. **Incorrect-answer feedback was not explicit enough.**  
   The original review showed the correct answer and one general explanation, but it did not clearly tell the student why the selected option failed.

5. **Questions did not identify their workshop source.**  
   Students could not easily return to the relevant slides after making a mistake.

6. **A few questions needed correction or qualification.**
   - The paragraph-structure item incorrectly placed the main point at the end; Workshop 8 recommends a topic sentence at the beginning.
   - The hierarchy item presented one fixed ranking for treaties and case law; the materials say treaty rank varies by jurisdiction.
   - The OSCOLA items were updated to reflect the fifth edition and the course rule that each footnote ends with a full stop.

7. **The README contained only the project title.**  
   It did not explain how to run, share, edit, or validate the application.

## Changes made

- Expanded the bank from **200 to 312 questions**.
- Added questions drawn from the uploaded materials for Workshops 1–9.
- Added more scenario-based questions on:
  - the grudge informer and Fuller’s principles;
  - Harvey v Facey, R v Coney, and Herd v Weardale;
  - false imprisonment and Biff’s Bus;
  - civil-law/common-law distinctions and precedent;
  - sources, hierarchy, and conflicts of norms;
  - legal research, citation, and OSCOLA;
  - signposting and legal argument;
  - legal writing, revision, active voice, and responsible AI use;
  - study methods, academic integrity, and exam technique.
- Moved the bank to `questions.js`.
- Added `questions.csv` for easy proofreading.
- Made the interface derive the bank size dynamically.
- Added workshop/source labels.
- Added explicit end-of-session wrong-answer feedback.
- Removed the duplicate `main.html`.
- Added practical sharing and editing instructions.

## Recommended future review process

Before each exam period:

1. Compare each workshop label with the newest official slide deck.
2. Ask the lecturer whether any topic has been removed, added, or changed.
3. Have at least two classmates independently check every new question.
4. Confirm that exactly one option is defensibly best.
5. Avoid distractors that are wrong only because of obscure wording.
6. Prefer short scenarios that test application over pure memorization.
7. Update OSCOLA and exam-procedure questions whenever the official guidance changes.
8. Record disputed questions in an issue list instead of silently changing them.

## Limitations

Some legal propositions are deliberately simplified because the course itself introduces broad legal concepts across different jurisdictions. The app should therefore be treated as a course-practice tool, not as jurisdiction-specific legal advice or an official mock exam.
