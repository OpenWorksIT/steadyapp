---
title: "The science"
description: "Why Steady asks between sessions, which questionnaires it uses, how its flags work, and who signs off the clinical side."
lead: "The science and research behind Steady come from Kempie van Rooyen and VR Clinical Psychology, who sign off every questionnaire, exercise, score band and line of clinical wording. This page explains the thinking behind it."
---

## Why ask between sessions

Two lines of research shape Steady.

**Tracking progress helps therapy.** When therapists routinely measure how their patients are doing and look at the results, outcomes improve a little, and fewer patients drop out or get worse without anyone noticing. A meta-analysis of 24 studies found feedback-assisted therapy did better than usual care in about two-thirds of them, with small to moderate effects, and the clearest gains for patients who weren't on track ([Lambert, Whipple and Kleinstäuber, 2018](https://doi.org/10.1037/pst0000167)). A larger one, of 58 studies and more than 21,000 patients, found a small but reliable improvement in symptoms and less drop-out ([de Jong and colleagues, 2021](https://doi.org/10.1016/j.cpr.2021.102002)). The effects are modest. Measurement supports good therapy; it doesn't replace it.

**Asking in the moment is more accurate than asking later.** People's memory of how a fortnight went leans on its best and worst days and on how they feel when asked. Short, repeated ratings in daily life, known as ecological momentary assessment, avoid much of that ([Shiffman, Stone and Hufford, 2008](https://doi.org/10.1146/annurev.clinpsy.3.022806.091415)).

So Steady asks four quick questions a day, lets the psychologist send standard questionnaires on a schedule, and puts the results in front of them before the next session.

## The daily check-in

Mood, anxiety, sleep and energy, each from 1 to 5, and a few words if the patient wants. It's deliberately short: a check-in someone does most days is worth more than a long one they abandon. It isn't a validated scale, and Steady doesn't score it; it shows the trend.

## The questionnaires

| Questionnaire | What it measures | Original paper |
|---|---|---|
| PHQ-9 | Depression severity | [Kroenke, Spitzer and Williams, 2001](https://doi.org/10.1046/j.1525-1497.2001.016009606.x) |
| GAD-7 | Generalised anxiety | [Spitzer and colleagues, 2006](https://doi.org/10.1001/archinte.166.10.1092) |
| PCL-5 | Post-traumatic stress symptoms | [Blevins and colleagues, 2015](https://doi.org/10.1002/jts.22059) |
| WHO-5 | Wellbeing | [Topp and colleagues, 2015](https://doi.org/10.1159/000376585) |

Steady scores them with their published bands, and patients don't see their own scores: the psychologist talks them through.

Psychologists can add instruments: written in the app, or imported from the open [ReproSchema library](https://github.com/ReproNim/reproschema-library) or a FHIR Questionnaire file. Every instrument carries its licence. Imported ones can't be sent until the practice confirms it may use them, and copyright-protected entries are blocked. WHO-5 ships marked for review, because its licence restricts commercial use and each practice should confirm it applies to them.

## Flags are for review, not for alarm

Steady highlights a few things for the psychologist to look at:

- any answer above "not at all" on PHQ-9 item 9, about thoughts of death or self-harm
- low mood in three check-ins in a row
- scores in the higher bands
- a run of missed check-ins

They're review aids. Steady doesn't calculate risk, doesn't diagnose, and doesn't alert anyone outside office hours. The psychologist decides what a flag means and marks it as reviewed.

## Watch data

If a patient chooses to share it, Steady shows a daily summary from their watch or phone: resting heart rate, sleep, steps and blood oxygen. Each is shown against the patient's own usual range rather than a population norm, because what's normal for one person isn't for another. There are no alerts. It's context for a conversation, and the start of a baseline for research that practices may do later, only with patients' consent.

## Who signs off

{{< person name="Kempie van Rooyen" role="clinical psychologist, VR Clinical Psychology, Gqeberha" photo="/img/kempie.jpg" >}}
Kempie has worked as a clinician for 18 years, as an academic psychologist and in the public service before private practice. His clinical and research interests are traumatic stress, burnout and adult personality. He leads the clinical side of Steady and its community of psychologists.
{{< /person >}}

Kempie and VR Clinical Psychology sign off every clinical decision in Steady: which questionnaires ship, how they're scored, what's flagged, and every word patients read about their care and their safety. OpenWorks IT writes the code and develops Steady to match.
