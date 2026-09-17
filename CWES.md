# CWES Review

Hey there, how's it going? I'm huupwn — that's my hacker handle, but my real name is Hữu. I'm still in high school, and CWES is actually the very first certification I've ever earned.

Next year I'm aiming to compete in a CTF, and I decided the best way to get ready was to study for and pass the **CWES (Web Exploitation Specialist)** certification from Hack The Box (HTB). It's a relatively new credential that's been gaining traction, and people often compare it to eWPTX or BSCP. Below is my full experience: the course, the exam, the report.

## Introduction

I got into security almost by accident — messing around with HTB Academy's free modules out of curiosity, then getting hooked on the "aha" moment of finding a working exploit. I don't have any prior certifications, any professional experience, or a network in the industry. What I do have is a lot of free time as a student and a genuine interest in web exploitation.

I like certifications because they're tangible proof of knowledge — a way to prove to myself (and eventually to others) that the skills are real, even without a resume full of work history.

After some research, I narrowed it down to two options: HTB's **Certified Web Exploitation Specialist (CWES)** and PortSwigger's **Burp Suite Certified Practitioner (BSCP)**. I'd already tried a few free HTB Academy modules just for fun and liked the teaching style, so CWES felt like the natural next step — and a solid checkpoint on the way to next year's CTF.

To earn the certification, you need to:

1. Complete all training material in the **Web Penetration Tester** path.
2. Pass the exam with a score of at least 80/100.
3. Submit a professional report.

## The Preparation Course

You have to complete 100% of the course material and pass the skills assessment at the end of every module before the exam even unlocks.

The path has about 20 modules, ranging from easy to medium difficulty. Everything is text-based — no videos, no slides. I got stuck on a few tasks, but the community hints (online and in HTB's Discord) saved me more than once.

No complaints about the content itself — it's clear, concise, and to the point. You can tell some modules were written by people with real pentesting experience; they occasionally drop in real-world anecdotes, which is a nice touch.

The full module list is on the HTB Academy site under the Web Penetration Tester path.

### Preparation: The Downside

The biggest gap is *practice*. Sure, each module ends with tasks, but you already know exactly which vulnerability class you're hunting for going in — that makes things much easier than they should be.

The real exam hands you an application and nothing else; figuring out what to test for is on you. A large integrated lab combining several applications — something that actually simulates exam conditions — would go a long way. A standalone list of extra practice machines wouldn't hurt either. Overall, I felt the course under-prepares you on the practical side.

## The Exam

One big plus: no scheduling required. You just log in and hit start whenever you're ready. You get **7 days total**, covering both lab access and report writing — no extra time is granted for the report, so plan accordingly.

You'll face multiple applications, each requiring a user flag and a root flag. Usually that means exploiting one vulnerability, or chaining two. Often there's some extra trick you have to work out on your own, though a few flags were straightforward — comparable to the skills assessments.

Honestly, some parts of the exam were *much* harder than anything in the modules — a few challenges pushed me well beyond what the skills assessments prepared me for. Other flags were closer to module difficulty, but I wouldn't call the exam "on par" across the board; expect real difficulty spikes. I had all flags by day 4 and spent the rest of the time on the report.

### The Exam's Downside

Seven days is a long stretch. I ended up scheduling mine over the New Year holidays to avoid taking time off work — not exactly a restful way to spend the break, and mentally draining while everyone else is off relaxing. I'd argue the timeline (and possibly the task count) could be trimmed.

It's also worth being upfront: without experience on machines outside the official modules, the exam is genuinely tough. The course theory alone isn't quite enough.

### The Exam's Upside

The environment itself was rock solid — no lag, no crashes, which matters a lot over a week-long exam. I also genuinely enjoyed the design of several of the challenges.

## Is the Course Enough to Pass?

Short answer: partially. The exploitation techniques are taught well, but as mentioned, the exam leans on "tricks" that aren't explicitly covered in the modules. Expect to figure some of it out on your own — which, honestly, is good practice for a CTF environment where you rarely get hand-holding either.

## Writing the Report

Capturing flags isn't enough on its own — a professional report is mandatory, and people do fail for turning in a weak one. It's not a walkthrough; it needs a full vulnerability breakdown per finding: impact, CWE/CVSS scoring, mitigations, and a step-by-step reproduction. HTB provides a template that spells out exactly what they expect.

I used **Sysreptor** to write mine, and it made the process much easier. It auto-formats everything in HTB's house style, builds a table of contents, and gives you a pre-structured section per finding. Find a SQL injection? Click "add new finding," select SQLi from the list, and it generates a chapter with pre-filled description and mitigation sections — you just plug in your specific steps.

**Tip:** the cloud version of Sysreptor is paid, but you can self-host it for free on your own VM and access it through a web panel from Kali or your host machine. I'd strongly recommend setting this up *before* the exam starts. It refused to run on my Kali box, so I had to spin up Ubuntu instead — about 90 minutes I didn't want to lose mid-exam.

Writing the report took me 5–6 hours. I slept on it and reviewed everything with fresh eyes the next morning. HTB's grading SLA is up to 20 business days.

**Update:** I submitted my report at noon on January 7th and got the passing result the evening of January 9th — just over two days for the review.

## Cost

As of early 2026, there are two main ways to pay:

- **Silver Annual Subscription — $490.** Full access to the Web Penetration Tester path plus one exam voucher. The simplest, set-it-and-forget-it option.
- **Cubes (HTB's internal currency).** The full Web Penetration Tester path costs 1,410 cubes (~$150 at ~$100 per 1,000 cubes), plus a separate $210 exam voucher — roughly **$360 total**. More budget-friendly if CWES is your only goal on the platform.

Check HTB's billing page for current pricing.

## My Tips

1. **Take detailed notes.** Non-negotiable. Modules often bury small details or code snippets that become direct hints during the exam — document everything so it's searchable later.
2. **Redo the skills assessments before the exam.** Go back and re-solve the final module tasks, and skim the learning material again so you can navigate it quickly under time pressure. You *will* be flipping back to course text during the exam looking for ideas.
3. **Get outside practice.** The modules alone aren't enough — time spent on machines on the main HTB platform is invaluable. I haven't finished the Bug Bounty Hunter track myself, but it looks like solid manual-exploitation practice, and manual exploitation is exactly the muscle a CTF will test.
4. **Be selective about extra resources.** I worked through parts of IppSec's CPTS path, and while good, it wasn't very relevant here. Look for machines that demand manual web exploitation, not public exploits for outdated software — that's the skill set both CWES and next year's CTF actually reward.


***Note about AI usage:*** *I wrote this article myself. I used Claude (Anthropic) to significantly refine the grammar, wording, and sentence structure; the technical content and all claims are my own.*

***Note:*** *If you want some of my CWES write-up, pls contact me [here](https://www.facebook.com/profile.php?id=61553341873402)*