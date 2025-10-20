# VitalVox: https://vitalvox.netlify.app/
Devpost: https://devpost.com/software/vitalvox

Demo: https://youtu.be/ndIbq4j0uBA?si=NljyFuIEbSggVsYu

## Inspiration
I (Allison) volunteered at a rescue squad in high school, riding in ambulances alongside EMTs and responding to local 911 calls. There, I saw the inner workings of emergency response -- and I was shocked. We were almost always thrown on scene with very little information from dispatchers, so we constantly had to walk up to patients having no idea what their emergency was. It wasn't uncommon to just get a message saying "motor vehicle accident" -- which told us nothing about how many patients there were, how severe the accident was, or what kinds of injuries were present. I soon learned that this was because dispatchers had to juggle countless responsibilities at once, making it impossible for them to give us all the information they received. That's why Arvin and I built VitalVox. VitalVox makes it much easier for dispatchers to transmit information to EMTs before they arrive on scene, allowing them to make faster, smarter decisions and save more lives.

## What it does
When someone dials 911, a dispatcher can use VitalVox to record the call in real-time. VitalVox will produce a transcript of the call, give a summary of the patient's symptoms, and let EMTs know what they might encounter. This allows EMTs to find out what's going on before they meet the patient, not after. VitalVox can also give suggestions on what equipment to bring, as well as what conditions the patient could potentially have, making EMTs well-equipped to treat patients faster.

## How we built it
We built the front-end using JavaScript, HTML, and CSS (with Tailwind). The back-end utilizes Node.js and Express.js. We obtain a live audio stream using the browser's media recorder, then generate a transcript using speaker diarization through a convolution-augmented transformer, via the AssemblyAI API. Next, we use the Gemini API to summarize the transcript and suggest ideas for what the EMTs might run into while on scene
