<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Map–Territory Practice 3 (Advanced + Reasoning)</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 900px;
      margin: 20px auto;
      line-height: 1.5;
      padding: 0 10px;
    }
    h1, h2 {
      margin-top: 1.4em;
    }
    .card {
      border: 1px solid #bbb;
      border-radius: 8px;
      padding: 14px;
      margin: 14px 0;
      background: #fafafa;
    }
    .question-title {
      font-weight: bold;
      margin-bottom: 8px;
    }
    .feedback {
      margin-top: 8px;
      padding: 8px;
      border-radius: 6px;
      background: #fff;
      border-left: 4px solid #888;
      display: none;
    }
    .correct {
      border-left-color: green;
      color: green;
    }
    .incorrect {
      border-left-color: darkred;
      color: darkred;
    }
    button {
      margin-top: 6px;
      padding: 6px 10px;
      border-radius: 6px;
      border: 1px solid #666;
      cursor: pointer;
    }
    textarea {
      width: 100%;
      min-height: 90px;
      margin-top: 8px;
    }
  </style>
</head>
<body>

<h1>Map–Territory Practice 3 (Advanced)</h1>
<p>
  This practice is designed to be trickier than the previous ones.
  Some answers might sound reasonable, but only one is the <strong>best</strong>
  map–territory interpretation. When you make a mistake, you’ll see
  a detailed explanation of <strong>why</strong> it’s not the best option.
</p>

<h2>Part A – Advanced Multiple-Choice Scenarios</h2>

<!-- Q1 -->
<div class="card">
  <div class="question-title">1. Personality Test in Hiring</div>
  <p>
    A company uses a personality test to filter candidates for a sales role.
    They reject candidates who fall into a certain “introverted” category,
    <em>but</em> they still check CVs, references, and run a trial sales call
    with the remaining candidates.
    <br><br>
    Which option is the best assessment in terms of map–territory?
  </p>
  <label>
    <input type="radio" name="q1" value="A">
    A) This is a strong map–territory confusion: the test is treated as the whole truth.
  </label><br>
  <label>
    <input type="radio" name="q1" value="B">
    B) This is a <em>partial</em> map–territory risk: the test is just one map, and it may be over-weighted, but other checks still bring them closer to the territory.
  </label><br>
  <label>
    <input type="radio" name="q1" value="C">
    C) There is no map–territory issue at all if the test is statistically validated.
  </label><br>
  <button onclick="checkAdvancedQ(1)">Check</button>
  <div id="fb1" class="feedback"></div>
</div>

<!-- Q2 -->
<div class="card">
  <div class="question-title">2. Data-Driven, User-Ignoring Product Team</div>
  <p>
    A product team improves their “daily active users” metric after a redesign,
    but they receive many qualitative complaints from their best paying customers
    about frustration with the new interface. The team decides the complaints are
    “just noise” because the main metric is up.
    <br><br>
    What is the best diagnosis?
  </p>
  <label>
    <input type="radio" name="q2" value="A">
    A) They’re confusing the metric (map) with the overall customer experience (territory).
  </label><br>
  <label>
    <input type="radio" name="q2" value="B">
    B) There is no map–territory issue; if the main KPI is up, the territory is clearly better.
  </label><br>
  <label>
    <input type="radio" name="q2" value="C">
    C) The only problem is confirmation bias, not map–territory confusion.
  </label><br>
  <button onclick="checkAdvancedQ(2)">Check</button>
  <div id="fb2" class="feedback"></div>
</div>

<!-- Q3 -->
<div class="card">
  <div class="question-title">3. Backtest-Obsessed Investor</div>
  <p>
    An investor builds a backtest model showing that a certain strategy
    (using value screens and timing signals) would have performed extremely well
    in the last 15 years. He then allocates almost all his capital to this strategy,
    assuming “the model has proven it works.”
    <br><br>
    Which statement is the best map–territory analysis?
  </p>
  <label>
    <input type="radio" name="q3" value="A">
    A) This is fine: a good backtest makes the model essentially equivalent to reality.
  </label><br>
  <label>
    <input type="radio" name="q3" value="B">
    B) There might be a small risk, but since the backtest uses real historical data, there is no real map–territory problem.
  </label><br>
  <label>
    <input type="radio" name="q3" value="C">
    C) This is a serious map–territory confusion: the backtest is a limited map of specific past conditions, not the full future territory.
  </label><br>
  <button onclick="checkAdvancedQ(3)">Check</button>
  <div id="fb3" class="feedback"></div>
</div>

<!-- Q4 -->
<div class="card">
  <div class="question-title">4. Teacher Redesigning a Course</div>
  <p>
    A language teacher gives a diagnostic grammar test at the beginning of a course.
    The results show that 70% of the class is weak on conditionals. The teacher uses this data
    to redesign the next weeks of lessons with extra practice on conditionals,
    <em>and</em> then observes the students in real activities and adjusts again.
    <br><br>
    Which is the best interpretation?
  </p>
  <label>
    <input type="radio" name="q4" value="A">
    A) Strong map–territory confusion: the teacher is blindly trusting the test.
  </label><br>
  <label>
    <input type="radio" name="q4" value="B">
    B) Good map usage: the test is a starting map, then the teacher checks and updates it with territory (real performance).
  </label><br>
  <label>
    <input type="radio" name="q4" value="C">
    C) No maps are involved here; tests are part of the territory.
  </label><br>
  <button onclick="checkAdvancedQ(4)">Check</button>
  <div id="fb4" class="feedback"></div>
</div>

<!-- Q5 -->
<div class="card">
  <div class="question-title">5. “Lazy Student” Label</div>
  <p>
    You have a student who often submits homework late and seems distracted in class.
    You internally label them as “lazy”. A few weeks later, you discover they are
    taking care of a sick family member and working a night job, and they still
    try to keep up with the course.
    <br><br>
    Regarding the label “lazy”, which option is the most accurate map–territory insight?
  </p>
  <label>
    <input type="radio" name="q5" value="A">
    A) The label “lazy” was a low-quality map that ignored important territory (their real situation).
  </label><br>
  <label>
    <input type="radio" name="q5" value="B">
    B) The label “lazy” was accurate because behaviour is all that matters.
  </label><br>
  <label>
    <input type="radio" name="q5" value="C">
    C) There was no map–territory issue, because personal context should never influence teaching decisions.
  </label><br>
  <button onclick="checkAdvancedQ(5)">Check</button>
  <div id="fb5" class="feedback"></div>
</div>

<h2>Part B – Written Reasoning Practice</h2>
<p>
  In this part, you need to <strong>write your reasoning</strong>, not just pick an option.
  The feedback will check whether you explicitly talk about <em>maps vs territory</em>,
  simplification, and why it matters for decisions.
</p>

<!-- Reasoning Task 1 -->
<div class="card">
  <div class="question-title">6. Explain a Map–Territory Error (Scenario)</div>
  <p>
    Imagine a freelancer who only looks at “monthly income” as a measure of success,
    ignoring things like burnout, long-term client relationships, and skill growth.
    <br><br>
    In a short paragraph, explain why this is a <strong>map–territory</strong> problem.
  </p>
  <textarea id="reason1" placeholder="Write your explanation here..."></textarea>
  <button onclick="evaluateReasoning('reason1','fb6')">Evaluate my reasoning</button>
  <div id="fb6" class="feedback"></div>
</div>

<!-- Reasoning Task 2 -->
<div class="card">
  <div class="question-title">7. Teach the Concept to a Friend</div>
  <p>
    Write a short explanation (3–6 sentences) that you could tell a friend:
    <br>
    <em>“What does ‘the map is not the territory’ mean, and how could misunderstanding this hurt your decisions?”</em>
  </p>
  <textarea id="reason2" placeholder="Explain it as if you were talking to a friend..."></textarea>
  <button onclick="evaluateReasoning('reason2','fb7')">Evaluate my explanation</button>
  <div id="fb7" class="feedback"></div>
</div>

<script>
  // Correct answers for Part A
  const advancedAnswers = {
    1: "B",
    2: "A",
    3: "C",
    4: "B",
    5: "A"
  };

  const advancedExplanations = {
    1: {
      A: "Not the best choice. There is a map–territory risk, but it’s not purely blind faith. They still use other information (CVs, references, trial calls), so the test isn’t treated as the whole territory.",
      B: "Correct. The personality test is a map. Using it as one input among several is safer, but it can still be over-weighted. So there is a partial map–territory risk, not a total confusion.",
      C: "Not the best choice. Even a validated test is still a simplified map. Treating it as if it perfectly reflects reality would itself be a map–territory confusion."
    },
    2: {
      A: "Correct. The KPI is a narrow map of behaviour. Complaints from high-value customers are part of the territory. Ignoring that because a single metric improved is a classic map–territory mistake.",
      B: "Not the best choice. A single metric up doesn’t guarantee that reality is better, especially if valuable customers are unhappy. That’s treating the map as the territory.",
      C: "Not the best choice. Confirmation bias may be involved, but the core problem here is treating the KPI (map) as if it fully represented customer experience (territory)."
    },
    3: {
      A: "Not the best choice. A good backtest is still just a model of past conditions. It cannot capture all future scenarios. Treating it as equivalent to reality is exactly the map–territory error.",
      B: "Not the best choice. The risk is not small: past market regimes can be very different from future ones. The backtest is a restricted map in time.",
      C: "Correct. The backtest is a limited, historical map. The investor is acting as if this map fully describes the future territory, which is a serious map–territory confusion."
    },
    4: {
      A: "Not the best choice. The teacher is not blindly trusting the test; they use it to design lessons, then check and update based on real performance. That’s good map usage.",
      B: "Correct. The test is a map; the teacher uses it as a starting point and then updates their view from the territory (how students actually perform). That’s exactly how to use maps well.",
      C: "Not the best choice. A test is definitely a map, not the territory. It is a structured measurement, not reality itself."
    },
    5: {
      A: "Correct. The label “lazy” was a poor-quality map. It ignored the student’s real-life constraints and effort. The territory was far more complex and compassionate.",
      B: "Not the best choice. Behaviour matters, but the model “lazy” compresses complex reality into a harsh stereotype. That ignores the full territory behind the behaviour.",
      C: "Not the best choice. Personal context often changes how we interpret behaviour and how we support students. Saying it ‘never’ matters is itself a kind of bad map."
    }
  };

  function checkAdvancedQ(num) {
    const name = "q" + num;
    const radios = document.getElementsByName(name);
    let choice = null;

    for (const r of radios) {
      if (r.checked) {
        choice = r.value;
        break;
      }
    }

    const fb = document.getElementById("fb" + num);
    fb.style.display = "block";

    if (!choice) {
      fb.className = "feedback incorrect";
      fb.innerHTML = "Please choose an option first.";
      return;
    }

    if (choice === advancedAnswers[num]) {
      fb.className = "feedback correct";
    } else {
      fb.className = "feedback incorrect";
    }

    fb.innerHTML = advancedExplanations[num][choice];
  }

  // Reasoning evaluation for Part B
  function evaluateReasoning(textId, fbId) {
    const text = document.getElementById(textId).value.trim();
    const fb = document.getElementById(fbId);
    fb.style.display = "block";

    if (!text) {
      fb.className = "feedback incorrect";
      fb.innerHTML = "Try writing at least a few sentences in your own words 🙂";
      return;
    }

    const lower = text.toLowerCase();
    const mentionsMap = lower.includes("map") || lower.includes("mappa");
    const mentionsTerritory = lower.includes("territory") || lower.includes("territorio");
    const mentionsSimplify = lower.includes("simpl") || lower.includes("modello") || lower.includes("model");
    const mentionsDecision = lower.includes("decis") || lower.includes("scelta") || lower.includes("errore") || lower.includes("mistake");
    const lengthOK = text.length >= 120;

    let comments = [];

    if (mentionsMap && mentionsTerritory && mentionsSimplify && mentionsDecision && lengthOK) {
      fb.className = "feedback correct";
      comments.push("Nice work – you’re explicitly talking about maps vs territory, simplification, and consequences for decisions. This is a solid explanation.");
    } else {
      fb.className = "feedback incorrect";
      comments.push("Good start, but you can make your reasoning even sharper:");
      if (!mentionsMap || !mentionsTerritory) {
        comments.push("- Explicitly mention both the <strong>map</strong> (your model/metric/label) and the <strong>territory</strong> (messy reality).");
      }
      if (!mentionsSimplify) {
        comments.push("- Emphasise that the map is a <strong>simplified representation</strong> that leaves things out.");
      }
      if (!mentionsDecision) {
        comments.push("- Add how confusing the two can lead to <strong>bad decisions or wrong conclusions</strong>.");
      }
      if (!lengthOK) {
        comments.push("- Write a little more (at least 3–5 sentences) so you can include an example and why it matters.");
      }
    }

    fb.innerHTML = comments.join("<br>");
  }
</script>

</body>
</html>
