# SOES Student app

The Student portal of the Secure Offline Examination System (LCUP Senior High School) as an installable mobile app.
Students install it from Chrome on their Android phone. After the first open it works without internet.

## Put it online with GitHub Pages (one time, about 10 minutes)

1. Sign in at https://github.com (create a free account if needed).
2. Select **New repository**. Name it `soes-student`, choose **Public** (GitHub Pages on a free account needs a public repository; the app holds no exam questions, answer keys, or student data), and select **Create repository**.
3. On the new repository page, select **uploading an existing file**. Drag in everything from this folder: `index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, `README.md`, and the `icons` folder. Select **Commit changes**.
   If your computer hides `.nojekyll`, skip it; the app still works.
4. Open **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, Branch to **main**, folder **/(root)**, and select **Save**.
5. After a minute or two the page shows the address, for example `https://your-username.github.io/soes-student/`. That is the app link to give students.

## How students install it

1. Open the app link in **Chrome** on the phone (with internet, the first time only).
2. Tap the **⋮** menu, then **Install app** or **Add to Home screen**.
3. Open **SOES Student** from the home screen. It opens full screen like any app.
4. Tap **Add my profile**: official student ID, full name, section, and a 4 to 6 digit PIN.

On iPhone: open the link in Safari, tap **Share**, then **Add to Home Screen**.

## Using it

- Save the quiz package your teacher shares (file or code) before exam day under **My quizzes > Add a quiz package**.
- At exam time, enter the exam password your teacher announces. No internet is needed while answering.
- Leaving the app or staying idle locks the exam. Only your teacher's reconnection code unlocks it.
- After submitting, send the submission file or code to your teacher. Add the results file your teacher releases under **My scores** to see your score and study recommendations.

## Updating the app

Upload the new `index.html` (and any changed files) to the same repository. Also change the `CACHE` name in `sw.js`
(for example `soes-student-v0.6`) so phones pick up the new version the next time they open the app online.

## Privacy and security notes

- Profiles, packages, answers, and results are stored only on the student's phone, protected by the PIN.
- Quiz packages stay encrypted until the exam password is entered. Answer keys never reach the phone.
- Clearing Chrome's site data or uninstalling the app deletes saved work. Students can make a backup under **Profile & backup**.
