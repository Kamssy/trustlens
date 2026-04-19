# trustlens
# TrustLens

> AI classification, explained. TrustLens shows you not just what a model decided — but which words made it decide that way.

---

## What is this?

TrustLens is a React application that takes text input — a loan application, a job description, a product review — runs it through a pre-trained classification model, and then does something most AI interfaces don't bother with: it explains *why*.

Not just a label. Not just a confidence score. It shows you which words pushed the decision, in which direction, and by how much. It turns a black box into something a non-expert can actually interrogate.

---

## The problem it's solving

Most AI-powered interfaces give you a result and expect you to trust it. "Application declined." "High risk." "Negative sentiment." No context, no reasoning, no recourse.

This is a design problem as much as a technical one. The model may be doing exactly what it was trained to do — but if the person receiving the decision can't understand it, the system has failed them regardless of its accuracy.

TrustLens is an experiment in what it looks like when an interface takes explainability seriously.

---

## How it works

The user inputs any piece of text and submits it. The app sends it to a Hugging Face inference API — no model training required — and receives a classification result alongside a confidence score. TrustLens then analyses which words most strongly influenced that result and renders them as a bar chart, colour-coded by direction. Words that pushed the result positive point one way. Words that pushed it negative point the other. The user sees not just what the model decided, but what it was paying attention to.

---

## Stack

```
React + Vite
Recharts
Hugging Face Inference API (free tier)
Deployed on Vercel
```

---

## Status

Currently in active development. This README describes the project intention — the build is in progress.

---

*Built by Kamsiriochi*
