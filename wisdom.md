```markdown
---
layout: page
title: Daily Wisdom
---
<div id="quote"></div>
<script>
  fetch('https://stoicquotesapi.com/api/v1/quotes/random')
    .then(response => response.json())
    .then(data => {
      document.getElementById('quote').innerHTML = 
        `<blockquote>${data.quoteBody} <footer>${data.quoteAuthor}</footer></blockquote>`;
    });
</script>
```
