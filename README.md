<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Module 26 - The Mompreneur Zone | The Creator Plug Academy</title>
  <style>
    :root {
      --ink: #24192f;
      --muted: #6f6178;
      --panel: #ffffff;
      --gold: #d9a441;
      --gold-soft: #fff2c9;
      --rose: #f05d8a;
      --teal: #18a6a7;
      --violet: #4d2770;
      --violet-deep: #241332;
      --line: #eadfce;
      --shadow: 0 18px 40px rgba(48, 31, 61, 0.14);
    }
    * { box-sizing: border-box; }
    html { scroll-behavior: smooth; }
    body {
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      color: var(--ink);
      background:
        radial-gradient(circle at 14% 8%, rgba(240, 93, 138, 0.15), transparent 28%),
        radial-gradient(circle at 88% 4%, rgba(24, 166, 167, 0.16), transparent 26%),
        linear-gradient(180deg, #fffaf1 0%, #f8f1e7 45%, #f4ebdd 100%);
      line-height: 1.6;
    }
    a { color: #2c6f91; font-weight: 800; }
    .page { width: min(1120px, calc(100% - 32px)); margin: 0 auto; padding: 28px 0 56px; }
    .hero { background: linear-gradient(135deg, rgba(36, 19, 50, 0.96), rgba(77, 39, 112, 0.92)); color: #fff; border-radius: 8px; padding: 34px; box-shadow: var(--shadow); position: relative; overflow: hidden; }
    .hero:after { content: ""; position: absolute; right: -78px; top: -82px; width: 260px; height: 260px; border: 2px solid rgba(217, 164, 65, 0.36); transform: rotate(20deg); }
    .eyebrow { display: inline-flex; background: rgba(217, 164, 65, 0.18); border: 1px solid rgba(217, 164, 65, 0.45); color: #ffe3a0; border-radius: 8px; padding: 7px 11px; font-size: 13px; font-weight: 800; letter-spacing: 0.08em; text-transform: uppercase; }
    h1, h2, h3 { line-height: 1.15; margin: 0; }
    h1 { max-width: 900px; margin-top: 18px; font-size: clamp(34px, 6vw, 70px); }
    .subtitle { max-width: 880px; margin: 18px 0 0; color: #f6e9d6; font-size: 18px; }
    .quick-links { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 24px; position: relative; z-index: 1; }
    .quick-links a, .copy-button { appearance: none; border: 0; border-radius: 8px; background: var(--gold); color: #241332; cursor: pointer; display: inline-flex; align-items: center; justify-content: center; font-family: inherit; font-size: 14px; font-weight: 900; line-height: 1; min-height: 42px; padding: 12px 14px; text-decoration: none; }
    .quick-links a:hover, .copy-button:hover { background: #f1c761; }
    .hero-grid, .three-col { display: grid; grid-template-columns: repeat(3, 1fr); gap: 14px; margin-top: 26px; }
    .hero-card { background: rgba(255, 255, 255, 0.1); border: 1px solid rgba(255, 255, 255, 0.18); border-radius: 8px; padding: 18px; min-height: 126px; }
    .hero-card strong { color: #ffe1a1; display: block; font-size: 15px; text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 8px; }
    .section { margin-top: 24px; background: rgba(255, 255, 255, 0.88); border: 1px solid var(--line); border-radius: 8px; padding: 28px; box-shadow: 0 10px 24px rgba(48, 31, 61, 0.08); }
    .section h2 { color: var(--violet-deep); font-size: clamp(25px, 3vw, 38px); margin-bottom: 12px; }
    .section-intro { max-width: 900px; color: var(--muted); margin: 0 0 20px; }
    .two-col { display: grid; grid-template-columns: repeat(2, 1fr); gap: 16px; }
    .card { background: var(--panel); border: 1px solid var(--line); border-radius: 8px; padding: 20px; }
    .card h3 { color: var(--violet); font-size: 20px; margin-bottom: 8px; }
    .tag { display: inline-block; border-radius: 8px; padding: 5px 9px; margin-bottom: 12px; background: var(--gold-soft); color: #765210; font-weight: 800; font-size: 12px; text-transform: uppercase; letter-spacing: 0.06em; }
    ul, ol { margin: 10px 0 0 20px; padding: 0; }
    li { margin: 8px 0; }
    .link-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 12px; margin-bottom: 24px; }
    .lesson-link { background: #fff; border: 1px solid var(--line); border-radius: 8px; color: var(--violet-deep); display: block; font-weight: 800; padding: 14px; text-decoration: none; }
    .lesson-link:hover { border-color: var(--gold); box-shadow: 0 8px 20px rgba(48, 31, 61, 0.1); transform: translateY(-1px); }
    .lesson { display: grid; grid-template-columns: 84px 1fr; gap: 16px; border-top: 1px solid var(--line); padding: 20px 0; }
    .lesson:first-of-type { border-top: 0; padding-top: 0; }
    .lesson-number { width: 64px; height: 64px; border-radius: 8px; background: linear-gradient(135deg, var(--violet), var(--rose)); color: #fff; display: grid; place-items: center; font-size: 24px; font-weight: 900; box-shadow: 0 12px 22px rgba(77, 39, 112, 0.22); }
    .lesson-number a { color: #fff; display: grid; height: 100%; place-items: center; text-decoration: none; width: 100%; }
    .callout { border-left: 5px solid var(--gold); background: #fff7dc; padding: 16px 18px; border-radius: 8px; margin-top: 16px; }
    .warning { border-left-color: var(--rose); background: #fff0f5; }
    table { width: 100%; border-collapse: collapse; overflow: hidden; border-radius: 8px; background: #fff; border: 1px solid var(--line); margin-top: 14px; }
    th, td { text-align: left; vertical-align: top; border-bottom: 1px solid var(--line); padding: 14px; }
    th { background: var(--violet-deep); color: #fff; font-size: 13px; text-transform: uppercase; letter-spacing: 0.06em; }
    tr:last-child td { border-bottom: 0; }
    .script-box { background: #241332; color: #fdf5e8; border-radius: 8px; padding: 18px; font-family: "Courier New", Courier, monospace; font-size: 14px; line-height: 1.55; white-space: pre-wrap; }
    .copy-row { align-items: center; display: flex; flex-wrap: wrap; gap: 10px; justify-content: space-between; margin-bottom: 10px; }
    .checklist { list-style: none; margin-left: 0; }
    .checklist li { padding-left: 34px; position: relative; }
    .checklist li:before { content: ""; position: absolute; left: 0; top: 5px; width: 19px; height: 19px; border-radius: 5px; border: 2px solid var(--teal); background: #efffff; }
    .footer { margin-top: 24px; text-align: center; color: var(--muted); font-size: 14px; }
    @media (max-width: 820px) {
      .hero { padding: 24px; }
      .hero-grid, .two-col, .three-col, .link-grid { grid-template-columns: 1fr; }
      .lesson { grid-template-columns: 1fr; }
      table, thead, tbody, th, td, tr { display: block; }
      th { display: none; }
    }
  </style>
</head>
<body>
  <main class="page">
    <section class="hero">
      <span class="eyebrow">Module 26</span>
      <h1>The Mompreneur Zone</h1>
      <p class="subtitle">Build a business that works around your family, not against it. Strategy, systems, digital products, content, email, affiliate income, coaching, and realistic time blocks for real mom life.</p>
      <nav class="quick-links" aria-label="Quick links">
        <a href="#lessons">Lessons</a>
        <a href="#launch-plan">30-Day Plan</a>
        <a href="#copy-tools">Copy Tools</a>
        <a href="#resources">Resource Links</a>
      </nav>
      <div class="hero-grid">
        <div class="hero-card"><strong>Core Message</strong>This is not hustle culture. It is smart strategy for the time and energy you actually have.</div>
        <div class="hero-card"><strong>Best Models</strong>Digital products, affiliate marketing, content, VA work, social media management, coaching, and print on demand.</div>
        <div class="hero-card"><strong>Main Result</strong>A flexible business plan that fits school pickups, naps, sick days, and family life.</div>
      </div>
    </section>

    <section class="section" id="welcome">
      <h2>Welcome to Module 26</h2>
      <p class="section-intro">You are a mom. You love your kids. You also want more income, more purpose, more freedom, and more of yourself. The Mompreneur Zone is built for women managing real life while building something of their own.</p>
      <div class="callout">Whether you have 30 minutes a day or 3 hours, there is a business model and system that can work. The goal is not to copy someone else's schedule. The goal is to design a business around your actual life.</div>
    </section>

    <section class="section" id="lessons">
      <h2>Lessons</h2>
      <div class="link-grid">
        <a class="lesson-link" href="#lesson-1">1. Mindset shift</a>
        <a class="lesson-link" href="#lesson-2">2. Business models that work</a>
        <a class="lesson-link" href="#lesson-3">3. Finding your niche</a>
        <a class="lesson-link" href="#lesson-4">4. Digital product business</a>
        <a class="lesson-link" href="#lesson-5">5. Social media</a>
        <a class="lesson-link" href="#lesson-6">6. Time blocking</a>
        <a class="lesson-link" href="#lesson-7">7. Email list</a>
        <a class="lesson-link" href="#lesson-8">8. Affiliate marketing</a>
        <a class="lesson-link" href="#lesson-9">9. Coaching and consulting</a>
        <a class="lesson-link" href="#lesson-10">10. Protecting energy</a>
        <a class="lesson-link" href="#lesson-11">11. Real business transition</a>
        <a class="lesson-link" href="#lesson-12">12. Income stack</a>
        <a class="lesson-link" href="#lesson-13">13. Community and collaboration</a>
        <a class="lesson-link" href="#launch-plan">14. 30-Day launch plan</a>
      </div>

      <article class="lesson" id="lesson-1">
        <div class="lesson-number"><a href="#lesson-1">1</a></div>
        <div>
          <h3>The Mompreneur Mindset Shift</h3>
          <p>Before strategy, we have to address what is happening in your head. Many moms get stopped before they start, not by their children or schedule, but by thoughts like "I do not have enough time" or "I will wait until life is calmer."</p>
          <div class="two-col">
            <div class="card">
              <h3>The lies</h3>
              <ul>
                <li>I do not have enough time.</li>
                <li>My kids need me too much right now.</li>
                <li>I am not tech-savvy enough.</li>
                <li>I will wait until they are in school.</li>
                <li>Someone else is already doing this.</li>
                <li>I do not know where to start.</li>
              </ul>
            </div>
            <div class="card">
              <h3>The truth</h3>
              <p>You do not need 8 hours a day. You need a plan for the hours you do have. Moms are already operators, schedulers, researchers, negotiators, problem solvers, and emotional managers.</p>
            </div>
          </div>
          <h4>The Mompreneur Mindset</h4>
          <ul>
            <li>Done is better than perfect.</li>
            <li>Progress over perfection, every single day.</li>
            <li>Your business does not have to be big to be meaningful.</li>
            <li>Consistency in small pockets of time beats random big effort.</li>
            <li>You are teaching your children what it looks like to build something.</li>
          </ul>
          <div class="callout"><strong>Reframe:</strong> Instead of "I only have 30 minutes," say "I have 30 minutes. What is the highest-impact thing I can do right now?"</div>
        </div>
      </article>

      <article class="lesson" id="lesson-2">
        <div class="lesson-number"><a href="#lesson-2">2</a></div>
        <div>
          <h3>Business Models That Work for Moms</h3>
          <p>Not every business model is compatible with motherhood. The best mompreneur businesses are flexible, low-cost, digital-first, and scalable.</p>
          <table>
            <thead><tr><th>Business Model</th><th>Time Required</th><th>Startup Cost</th><th>Earning Potential</th></tr></thead>
            <tbody>
              <tr><td>Digital products</td><td>1-2 hrs/day to build</td><td>Low</td><td>$500-$5,000+/month</td></tr>
              <tr><td>Affiliate marketing</td><td>30-60 min/day</td><td>Free</td><td>$200-$3,000+/month</td></tr>
              <tr><td>Coaching or consulting</td><td>2-3 hrs/week plus prep</td><td>Low</td><td>$1,000-$10,000+/month</td></tr>
              <tr><td>Social media management</td><td>Flexible hours</td><td>Free</td><td>$500-$3,000+/month</td></tr>
              <tr><td>Virtual assistant</td><td>Flexible hours</td><td>Free</td><td>$800-$4,000+/month</td></tr>
              <tr><td>Print on demand</td><td>1-2 hrs setup blocks</td><td>Free to low</td><td>$200-$2,000+/month</td></tr>
              <tr><td>Blogging/content</td><td>30-60 min/day</td><td>Low</td><td>$300-$5,000+/month</td></tr>
              <tr><td>Online courses</td><td>Build once, sell repeatedly</td><td>Low-medium</td><td>$500-$10,000+/month</td></tr>
              <tr><td>Handmade/Etsy shop</td><td>Variable</td><td>Low-medium</td><td>$300-$3,000+/month</td></tr>
            </tbody>
          </table>
          <div class="callout"><strong>Best starter combo:</strong> digital products plus affiliate marketing. Low time investment, no client management, and strong passive income potential.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-3">
        <div class="lesson-number"><a href="#lesson-3">3</a></div>
        <div>
          <h3>Finding Your Niche as a Mompreneur</h3>
          <p>Your niche is the specific topic or community you serve. The most powerful move is to build in a niche you already live in.</p>
          <div class="two-col">
            <div class="card"><h3>Mom Life</h3><p>Pregnancy, newborns, toddlers, school-age kids, homeschooling, single motherhood, co-parenting, blended families, motherhood mental health.</p></div>
            <div class="card"><h3>Home and Lifestyle</h3><p>Meal planning, budgeting, organization, cleaning systems, intentional living, family routines, slow living.</p></div>
            <div class="card"><h3>Health and Wellness</h3><p>Postpartum fitness, mom nutrition, family-friendly recipes, sleep, natural parenting, mental health.</p></div>
            <div class="card"><h3>Education and Kids</h3><p>Homeschool curriculum, learning activities, crafts, screen-free play, Montessori at home, reading readiness.</p></div>
            <div class="card"><h3>Finance</h3><p>Family budgeting, debt-free journey, saving on one income, couponing, frugal living, side hustles.</p></div>
            <div class="card"><h3>Business for Moms</h3><p>Teaching other moms how to build a business, once you have results, process, or experience to share.</p></div>
          </div>
          <h4>How to pick your niche</h4>
          <ol>
            <li>What do other moms ask you about?</li>
            <li>What have you figured out that felt hard until it clicked?</li>
            <li>What would you talk about for free because you love it?</li>
            <li>What problem are you currently solving in your own life?</li>
          </ol>
        </div>
      </article>

      <article class="lesson" id="lesson-4">
        <div class="lesson-number"><a href="#lesson-4">4</a></div>
        <div>
          <h3>Building Your Digital Product Business</h3>
          <p>Digital products are one of the best business models for moms because once created, they can sell without your presence.</p>
          <div class="two-col">
            <div class="card">
              <h3>Printables and Templates</h3>
              <ul>
                <li>Meal planning templates.</li>
                <li>Family budget spreadsheets.</li>
                <li>Chore charts and reward systems.</li>
                <li>Homeschool planners.</li>
                <li>Pregnancy and baby milestone trackers.</li>
                <li>Self-care checklists.</li>
                <li>Back-to-school printables.</li>
              </ul>
            </div>
            <div class="card">
              <h3>Guides and Courses</h3>
              <ul>
                <li>The Busy Mom's Meal Prep Guide.</li>
                <li>30-Day Declutter Challenge for Moms.</li>
                <li>Starting Your Side Hustle With a Newborn.</li>
                <li>Homeschool curriculum bundles.</li>
                <li>Baby sign language course.</li>
                <li>Toddler activity library.</li>
              </ul>
            </div>
          </div>
          <table>
            <thead><tr><th>Product</th><th>Typical Price</th><th>Best Platform</th></tr></thead>
            <tbody>
              <tr><td>Single printable</td><td>$3-$7</td><td>Etsy, Payhip</td></tr>
              <tr><td>Template bundle</td><td>$10-$25</td><td>Etsy, Gumroad, Payhip</td></tr>
              <tr><td>eBook or guide</td><td>$7-$37</td><td>Gumroad, Payhip, Etsy</td></tr>
              <tr><td>Mini-course</td><td>$27-$97</td><td>Gumroad, Skool, Kajabi</td></tr>
              <tr><td>Full course or curriculum</td><td>$97-$297</td><td>Skool, Kajabi, Teachable</td></tr>
            </tbody>
          </table>
        </div>
      </article>

      <article class="lesson" id="lesson-5">
        <div class="lesson-number"><a href="#lesson-5">5</a></div>
        <div>
          <h3>Social Media for Mompreneurs</h3>
          <p>You do not need a massive following to make money. You need the right following: people who trust you, relate to your life, and believe you can help.</p>
          <table>
            <thead><tr><th>Platform</th><th>Best For</th><th>Content Ideas</th></tr></thead>
            <tbody>
              <tr><td>TikTok and Reels</td><td>Relatable short-form video, tips, humor, day-in-the-life.</td><td>Mom hacks, honest routines, side hustle updates, product demos.</td></tr>
              <tr><td>Pinterest</td><td>Search-based traffic without daily performance pressure.</td><td>Printables, blog posts, product pins, checklists, meal plans.</td></tr>
              <tr><td>Facebook Groups</td><td>Community and warm trust-building.</td><td>Helpful posts, prompts, live trainings, niche conversations.</td></tr>
              <tr><td>YouTube</td><td>Longer tutorials, homeschool, routines, how-to content.</td><td>Walkthroughs, routines, reviews, step-by-step lessons.</td></tr>
              <tr><td>Blog</td><td>Google and Pinterest traffic, affiliate income, evergreen content.</td><td>Lists, tutorials, reviews, family systems, product roundups.</td></tr>
            </tbody>
          </table>
          <h4>Content ideas, no perfection required</h4>
          <ul>
            <li>What I actually ate today as a mom of 3.</li>
            <li>How I made $300 while my baby napped.</li>
            <li>5 things I stopped buying that saved us money.</li>
            <li>Honest homeschool routine: what nobody tells you.</li>
            <li>How I organize our home with 4 kids and zero storage.</li>
            <li>A day in my life as a work-from-home mom.</li>
          </ul>
        </div>
      </article>

      <article class="lesson" id="lesson-6">
        <div class="lesson-number"><a href="#lesson-6">6</a></div>
        <div>
          <h3>Time Blocking for the Mompreneur</h3>
          <p>The biggest challenge is not motivation. It is time. The solution is not finding perfect balance. The solution is using small pockets with a clear plan.</p>
          <div class="two-col">
            <div class="card"><h3>Naptime CEO Method</h3><p>Baby napping equals one power hour. Choose one task only. Keep a priority list ready so you can start immediately when the nap starts.</p></div>
            <div class="card"><h3>Before-They-Wake System</h3><p>Wake up 30-60 minutes before the kids and work on one focused task before the day begins.</p></div>
            <div class="card"><h3>After-Bedtime Shift</h3><p>Use 8pm-10pm for creation, planning, or batching. Set an end time so you do not burn out.</p></div>
            <div class="card"><h3>The 3-Task Rule</h3><p>Each day, pick only 3 business tasks that actually move the business forward. Do those first.</p></div>
          </div>
          <table>
            <thead><tr><th>Day</th><th>Focus</th></tr></thead>
            <tbody>
              <tr><td>Monday</td><td>Content creation: write or film.</td></tr>
              <tr><td>Tuesday</td><td>Content creation: finish or edit.</td></tr>
              <tr><td>Wednesday</td><td>Business tasks: email, products, shop updates.</td></tr>
              <tr><td>Thursday</td><td>Marketing: schedule content, outreach, engagement.</td></tr>
              <tr><td>Friday</td><td>Review and plan next week.</td></tr>
              <tr><td>Weekend</td><td>Protected family time and rest when possible.</td></tr>
            </tbody>
          </table>
        </div>
      </article>

      <article class="lesson" id="lesson-7">
        <div class="lesson-number"><a href="#lesson-7">7</a></div>
        <div>
          <h3>Growing Your Email List as a Mompreneur</h3>
          <p>Your email list is your most valuable business asset, especially when you cannot post daily. Email lets you reach your audience on your schedule.</p>
          <h4>Lead magnet ideas</h4>
          <ul>
            <li>Free printable: meal plan, budget template, chore chart, self-care tracker.</li>
            <li>Free mini guide: 5 Things That Actually Helped My Toddler Sleep.</li>
            <li>Free challenge: 5-Day Declutter Challenge.</li>
            <li>Free recipe collection: 10 Freezer Meals for New Moms.</li>
            <li>Free checklist: Hospital Bag Checklist or Back-to-School Checklist.</li>
          </ul>
          <h4>3-email welcome sequence</h4>
          <table>
            <thead><tr><th>Email</th><th>Timing</th><th>Purpose</th></tr></thead>
            <tbody>
              <tr><td>Email 1</td><td>Day 0</td><td>Deliver the freebie and welcome them warmly.</td></tr>
              <tr><td>Email 2</td><td>Day 2</td><td>Share your story, who you are, and why you do this.</td></tr>
              <tr><td>Email 3</td><td>Day 5</td><td>Give your best tip and softly mention your product.</td></tr>
            </tbody>
          </table>
          <div class="callout">Tool pricing and free-plan limits change. Check Kit, MailerLite, Beehiiv, or your email platform before teaching exact subscriber limits.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-8">
        <div class="lesson-number"><a href="#lesson-8">8</a></div>
        <div>
          <h3>Affiliate Marketing for Moms</h3>
          <p>Moms recommend products to each other constantly. Affiliate marketing means you can get paid for recommendations that are honest, useful, and relevant.</p>
          <h4>Strong affiliate categories</h4>
          <ul>
            <li>Amazon Associates for baby gear, kitchen tools, books, home organization, and homeschool supplies.</li>
            <li>LTK for lifestyle, fashion, home, beauty, and baby content.</li>
            <li>ShareASale and Impact for educational toys, meal delivery, home goods, parenting apps, and subscription boxes.</li>
            <li>Meal planning apps, homeschool curriculum companies, budgeting tools, and family organization apps.</li>
          </ul>
          <h4>Natural ways to share links</h4>
          <ul>
            <li>What's in my diaper bag.</li>
            <li>Our homeschool favorites this year.</li>
            <li>Products that changed my mom life.</li>
            <li>Things I bought this month that were worth it.</li>
            <li>Product review Reels, blog posts, or YouTube videos.</li>
          </ul>
          <div class="callout">Always disclose affiliate links clearly. Your audience trusts you more when you are transparent.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-9">
        <div class="lesson-number"><a href="#lesson-9">9</a></div>
        <div>
          <h3>Coaching and Consulting for Moms</h3>
          <p>If you have solved a specific problem, you can coach other moms through the same process. You do not need to know everything. You need a clear result and a responsible process.</p>
          <div class="two-col">
            <div class="card">
              <h3>Popular Coaching Niches</h3>
              <ul>
                <li>Postpartum fitness and nutrition.</li>
                <li>Family budgeting and debt payoff.</li>
                <li>Homeschool planning.</li>
                <li>Organization and decluttering.</li>
                <li>Business coaching for moms.</li>
                <li>Sleep consulting.</li>
                <li>Motherhood mindset.</li>
              </ul>
            </div>
            <div class="card">
              <h3>Starter Path</h3>
              <ol>
                <li>Offer 3-5 beta sessions.</li>
                <li>Collect feedback and testimonials.</li>
                <li>Turn the process into a simple package.</li>
                <li>Raise your rate and open paid spots.</li>
              </ol>
            </div>
          </div>
          <table>
            <thead><tr><th>Offer</th><th>Typical Price Range</th></tr></thead>
            <tbody>
              <tr><td>One 60-minute session</td><td>$75-$250</td></tr>
              <tr><td>4-week 1:1 package</td><td>$300-$1,000</td></tr>
              <tr><td>6-8 week group coaching</td><td>$197-$597</td></tr>
              <tr><td>Self-paced course</td><td>$97-$297</td></tr>
            </tbody>
          </table>
        </div>
      </article>

      <article class="lesson" id="lesson-10">
        <div class="lesson-number"><a href="#lesson-10">10</a></div>
        <div>
          <h3>Protecting Your Energy and Avoiding Burnout</h3>
          <p>Burnout is real, especially when you are building a business while pouring into everyone else.</p>
          <div class="two-col">
            <div class="card">
              <h3>Signs of Burnout</h3>
              <ul>
                <li>Dreading tasks you used to enjoy.</li>
                <li>Snapping at your kids more than usual.</li>
                <li>Feeling behind no matter what you finish.</li>
                <li>Physical exhaustion that sleep does not fix.</li>
                <li>Constant comparison to other creators.</li>
              </ul>
            </div>
            <div class="card">
              <h3>Prevention Strategies</h3>
              <ul>
                <li>Schedule rest like a real appointment.</li>
                <li>Set office hours and honor them.</li>
                <li>Underschedule instead of overcommitting.</li>
                <li>Use the good-enough rule.</li>
                <li>Ask for help before you are desperate.</li>
              </ul>
            </div>
          </div>
          <div class="callout">Your business should support your family life, not quietly consume it.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-11">
        <div class="lesson-number"><a href="#lesson-11">11</a></div>
        <div>
          <h3>From Side Hustle to Real Business</h3>
          <p>There is a moment when your "little thing" becomes something real. This transition is easier when you know what stage you are in.</p>
          <table>
            <thead><tr><th>Stage</th><th>Monthly Revenue</th><th>Focus</th><th>Time</th></tr></thead>
            <tbody>
              <tr><td>Hobby to side hustle</td><td>$0-$500</td><td>Create your first product or offer and get proof of concept.</td><td>30 min-1 hr/day</td></tr>
              <tr><td>Side hustle to business</td><td>$500-$2,000</td><td>Build systems, grow email, and show up consistently.</td><td>1-3 hrs/day</td></tr>
              <tr><td>Business growth</td><td>$2,000-$5,000+</td><td>Scale what works and outsource what you can.</td><td>3-5 hrs/day or less with help</td></tr>
            </tbody>
          </table>
          <h4>What to outsource first</h4>
          <ul>
            <li>Social media scheduling.</li>
            <li>Customer service emails.</li>
            <li>Graphic design or Canva production.</li>
            <li>Bookkeeping or transaction organization.</li>
          </ul>
          <div class="callout warning"><strong>Business setup note:</strong> Opening a bank account, choosing a structure, registering an LLC, and setting aside taxes are business and legal decisions. Use official resources and talk to a CPA or attorney when needed.</div>
        </div>
      </article>

      <article class="lesson" id="lesson-12">
        <div class="lesson-number"><a href="#lesson-12">12</a></div>
        <div>
          <h3>The Mompreneur Income Stack</h3>
          <p>Once you build one revenue stream, stack more for security and growth.</p>
          <table>
            <thead><tr><th>Stream</th><th>What It Is</th><th>Monthly Potential</th></tr></thead>
            <tbody>
              <tr><td>Etsy printables shop</td><td>10-20 printables generating search-based sales.</td><td>$200-$1,000</td></tr>
              <tr><td>Email list + product</td><td>500-1,000 subscribers buying a $27 product.</td><td>$300-$1,500</td></tr>
              <tr><td>Affiliate income</td><td>Amazon, LTK, and niche links in content.</td><td>$100-$500</td></tr>
              <tr><td>Coaching</td><td>Two clients in 4-week packages.</td><td>$800+</td></tr>
              <tr><td>Facebook group</td><td>Warm audience for products and coaching.</td><td>Amplifies all streams</td></tr>
            </tbody>
          </table>
          <p>This is not overnight. It is 6-12 months of consistent, intentional effort. But it is real and achievable.</p>
        </div>
      </article>

      <article class="lesson" id="lesson-13">
        <div class="lesson-number"><a href="#lesson-13">13</a></div>
        <div>
          <h3>Community, Collaboration, and Not Doing It Alone</h3>
          <p>Other moms building businesses are not automatically your competition. Many of them are your future collaborators, referral partners, customers, and friends.</p>
          <div class="two-col">
            <div class="card">
              <h3>Find Your People</h3>
              <ul>
                <li>Facebook groups for mompreneurs and work-from-home moms.</li>
                <li>Instagram creators in your niche.</li>
                <li>Skool communities for women building businesses.</li>
                <li>Local meetups, chambers, and coworking spaces with childcare.</li>
              </ul>
            </div>
            <div class="card">
              <h3>Collaborate</h3>
              <ul>
                <li>Guest post on each other's blogs.</li>
                <li>Cross-promote digital products.</li>
                <li>Go live together.</li>
                <li>Bundle products for a joint sale.</li>
                <li>Refer each other's services.</li>
              </ul>
            </div>
          </div>
          <div class="callout">Find one other mom building a business and check in weekly. Share wins, struggles, and next steps. Accountability keeps momentum alive.</div>
        </div>
      </article>
    </section>

    <section class="section" id="launch-plan">
      <h2>30-Day Mompreneur Launch Plan</h2>
      <p class="section-intro">Use this plan to choose your niche, create your first offer, set up your list, and start building momentum.</p>
      <table>
        <thead><tr><th>Day</th><th>Action</th></tr></thead>
        <tbody>
          <tr><td>1</td><td>Choose your niche using the Lesson 3 framework.</td></tr>
          <tr><td>2</td><td>Choose your primary business model.</td></tr>
          <tr><td>3</td><td>Research what is already selling on Etsy, Gumroad, and Pinterest.</td></tr>
          <tr><td>4-5</td><td>Create your first digital product or outline your service.</td></tr>
          <tr><td>6</td><td>Set up Gumroad, Payhip, or Etsy.</td></tr>
          <tr><td>7</td><td>Create your lead magnet: one free printable, checklist, or guide.</td></tr>
          <tr><td>8</td><td>Set up your email platform and upload the lead magnet.</td></tr>
          <tr><td>9</td><td>Update your Instagram, TikTok, or Pinterest bio with your link.</td></tr>
          <tr><td>10-11</td><td>Post your first 3 pieces of content.</td></tr>
          <tr><td>12</td><td>Join 2-3 Facebook groups in your niche.</td></tr>
          <tr><td>13</td><td>Engage in those groups by commenting, helping, and adding value.</td></tr>
          <tr><td>14</td><td>Write and schedule your first email to new subscribers.</td></tr>
          <tr><td>15-17</td><td>Create 3 more pieces of content mentioning your product or freebie.</td></tr>
          <tr><td>18</td><td>Research and join 2 affiliate programs.</td></tr>
          <tr><td>19</td><td>Add affiliate links to your bio, resources page, or content.</td></tr>
          <tr><td>20</td><td>Create your second digital product or upgrade your first.</td></tr>
          <tr><td>21</td><td>Send an email with a helpful tip and soft product mention.</td></tr>
          <tr><td>22</td><td>Review what got engagement, clicks, subscribers, or sales.</td></tr>
          <tr><td>23</td><td>Double down on what worked and release what did not.</td></tr>
          <tr><td>24</td><td>Set your Month 2 income goal.</td></tr>
          <tr><td>25-26</td><td>Batch content for the next 2 weeks.</td></tr>
          <tr><td>27</td><td>Plan your next product idea.</td></tr>
          <tr><td>28-30</td><td>Celebrate what you built, share your progress, and keep going.</td></tr>
        </tbody>
      </table>
    </section>

    <section class="section" id="copy-tools">
      <h2>Copy Tools</h2>
      <p class="section-intro">Use these templates to move faster when planning your niche, product, and weekly schedule.</p>
      <div class="copy-row">
        <h3>Mompreneur Niche Statement</h3>
        <button class="copy-button" data-copy="niche-template">Copy</button>
      </div>
      <div class="script-box" id="niche-template">I help [specific type of mom] with [specific problem] so she can [desired result] without [main frustration].

Example: I help busy moms meal plan simple family dinners so they can save money without spending Sunday cooking all day.</div>

      <div class="copy-row" style="margin-top: 18px;">
        <h3>3-Task Daily Planner</h3>
        <button class="copy-button" data-copy="task-template">Copy</button>
      </div>
      <div class="script-box" id="task-template">Today I have [time available].

My top 3 business tasks:
1. [Highest-impact task]
2. [Second task]
3. [Small maintenance task]

If everything falls apart today, I will still complete:
[One tiny non-negotiable task]</div>

      <div class="copy-row" style="margin-top: 18px;">
        <h3>Lead Magnet CTA</h3>
        <button class="copy-button" data-copy="cta-template">Copy</button>
      </div>
      <div class="script-box" id="cta-template">I made a free [printable/checklist/guide] to help you [specific result]. Comment [keyword] or grab it through the link in my bio.</div>
    </section>

    <section class="section" id="toolkit">
      <h2>Mompreneur Toolkit</h2>
      <div class="two-col">
        <div class="card">
          <h3>Free or Low-Cost Tools to Start</h3>
          <ul>
            <li>Canva for products and graphics.</li>
            <li>Gumroad, Payhip, or Etsy for selling.</li>
            <li>Kit, MailerLite, or Beehiiv for email.</li>
            <li>Later, Buffer, or Meta Business Suite for scheduling.</li>
            <li>Google Drive for files and delivery.</li>
            <li>Notion for business organization.</li>
          </ul>
        </div>
        <div class="card">
          <h3>Content to Create This Week</h3>
          <ul class="checklist">
            <li>1 post introducing yourself and your niche.</li>
            <li>1 helpful tip in your niche.</li>
            <li>1 post mentioning your lead magnet or product.</li>
            <li>1 behind-the-scenes post showing real mom life.</li>
            <li>1 email to your list or draft if your list is not live yet.</li>
          </ul>
        </div>
      </div>
      <div class="callout"><strong>Remember:</strong> 30 minutes of focused work beats 3 hours of scattered effort. Tiny progress compounds into something real.</div>
    </section>

    <section class="section" id="resources">
      <h2>Resource Links</h2>
      <div class="three-col">
        <div class="card">
          <h3>Business Structure</h3>
          <p><a href="https://www.sba.gov/business-guide/launch-your-business/choose-business-structure" target="_blank" rel="noopener">SBA: Choose your business structure</a></p>
        </div>
        <div class="card">
          <h3>Taxes</h3>
          <p><a href="https://www.irs.gov/businesses/small-businesses-self-employed/self-employed-individuals-tax-center" target="_blank" rel="noopener">IRS: Self-employed tax center</a></p>
          <p><a href="https://www.irs.gov/businesses/small-businesses-self-employed/estimated-taxes" target="_blank" rel="noopener">IRS: Estimated taxes</a></p>
        </div>
        <div class="card">
          <h3>Affiliate Disclosure</h3>
          <p><a href="https://www.ftc.gov/business-guidance/resources/disclosures-101-social-media-influencers" target="_blank" rel="noopener">FTC: Disclosures 101 for influencers</a></p>
        </div>
      </div>
    </section>

    <footer class="footer">
      <p>Module 26 - The Creator Plug Academy | Next: Module 27 - Lil CEO Zone</p>
    </footer>
  </main>

  <script>
    document.querySelectorAll("[data-copy]").forEach((button) => {
      button.addEventListener("click", async () => {
        const target = document.getElementById(button.getAttribute("data-copy"));
        if (!target) return;
        await navigator.clipboard.writeText(target.innerText.trim());
        const original = button.innerText;
        button.innerText = "Copied";
        setTimeout(() => { button.innerText = original; }, 1600);
      });
    });
  </script>
