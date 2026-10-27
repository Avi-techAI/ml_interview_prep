# Contributing

Thank you for helping improve this guide. It is revision material written by a student, so corrections genuinely matter.

## The most useful contributions

1. **Corrections.** If an explanation is wrong, misleading or out of date, open an issue titled `Correction: <section> Q<number>`. Say what is wrong and what it should say. A link to a source helps but is not required.
2. **Real interview questions.** A question you were actually asked, in a graduate or entry-level Machine Learning Engineer interview, is worth more than anything invented. Please do not include the company name if you signed anything, and never include a take-home task or any material you were asked to keep confidential.
3. **Better explanations.** If an answer is technically right but confusing, a clearer version is welcome.

## Ground rules for content

- Plain British English, active voice.
- Expand every abbreviation in brackets on first use, for example "MSc (Master of Science)".
- Four options per question, exactly one correct.
- Every question needs an explanation of why the correct answer is right, plus a separate rebuttal for each of the three wrong options. The rebuttal is written to follow the words "Option (x) is wrong because".
- Pitch it at a graduate: assume Python, do not assume production machine learning jargon.
- No copied text from books, courses or other question banks. Write it in your own words.

## How the file is put together

Everything lives in `index.html`. The questions sit in a JavaScript array near the bottom of the file, grouped by section. A question looks like this:

```js
{
  prompt: "The question text",
  options: ["first", "second", "third", "fourth"],
  answer: 2,                       // index of the correct option
  why: "Why the correct answer is correct, two to four sentences.",
  rebuttals: ["because ...", "because ...", null, "because ..."],
  alsoNote: "Optional extra line shown only on a correct answer."
}
```

`rebuttals` must have one entry per option, with `null` in the position of the correct answer.

The practice papers are built automatically at page load from whatever is in the bank, so you do not need to edit them. Answer positions are also shuffled automatically, which is why it is fine to write the correct option first.

## Submitting a change

Fork the repository, edit `index.html`, open the file in a browser to check your question renders and the feedback reads correctly, then open a pull request. If editing the file is awkward, open an issue with the question written out and I will add it for you.

Contributors are credited in the repository.
