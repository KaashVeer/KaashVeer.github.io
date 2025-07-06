```markdown
---
layout: page
title: Daily Challenge
---
<div id="challenge"></div>
<script>
  const challenges = [
    "Go 24 hours without checking stock prices.",
    "Write down three non-financial things you are grateful for today.",
    // Add more challenges...
  ];
  const today = new Date();
  const dayOfYear = Math.floor((today - new Date(today.getFullYear(), 0, 0)) / (1000 * 60 * 60 * 24));
  const index = dayOfYear % challenges.length;
  document.getElementById('challenge').innerHTML = challenges[index];
</script>
```
