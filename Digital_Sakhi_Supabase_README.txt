DIGITAL SAKHI — SUPABASE SAVE SETUP

What is included
- index.html (GitHub Pages home page) and Digital_Sakhi_Home.html (same updated home page, retained so existing learning-page links continue to work)
- Six separate learning pages (updated to save skill completion to Supabase)
- Digital_Sakhi_Supabase_Setup.sql (creates the required tables and insert-only policies)

IMPORTANT: The HTML still stores a local progress copy in the browser so the learner dashboard can display progress. The new code also sends records to Supabase. Anonymous website visitors can INSERT records but cannot SELECT, UPDATE or DELETE learner rows via the public API. This is a starter setup for a college project, not a complete identity-verification system; anyone can submit fake records to a public form. For real sensitive data or verified learner identities, add Supabase Auth and stricter policies or use a server-side Edge Function.

SETUP STEPS
1. Open https://supabase.com/dashboard and select your Digital Sakhi project.
2. Open SQL Editor → New query.
3. Open Digital_Sakhi_Supabase_Setup.sql from this package, copy all its contents, paste into SQL Editor, and click Run.
4. Check that the tables learner_profiles, baseline_assessments, skill_completions, quiz_attempts and program_completions exist in Table Editor.
5. Upload all seven HTML files to the root of your GitHub Pages repository. Use index.html as the home page filename (rename Digital_Sakhi_Home.html to index.html, and update the learning pages' back links from Digital_Sakhi_Home.html to index.html if you do this).
6. Test the website over its published HTTPS URL. Create a profile, submit an assessment, mark a skill complete, and submit the quiz.
7. In Supabase → Table Editor, open each table and confirm a new row appears.

The existing public survey connection is retained. Do not add a Supabase service_role key to any HTML or public GitHub repository.
