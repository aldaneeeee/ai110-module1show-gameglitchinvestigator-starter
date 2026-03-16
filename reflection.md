# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

Somethings I noticed was the there was a glitch with the attempts that the user gets
like it wouldn't update properly and it actually gave me 7 attempts rather than 8 . Also saw that the new game button didnt work and when you lose, it tells you that the secret number is actually less than what its guiding you towards withe the "go hight/go lower" prompt. Also the hit button doesnt actually give you hints. The game looked normal honestly 

- What did the game look like the first time you ran it? 
- List at least two concrete bugs you noticed at the start  
  (for example: "the secret number kept changing" or "the hints were backwards").

---

## 2. How did you use AI as a teammate?

I used claude copilot, I actually didnt have any bad suggestion from the copilot but i think thats because i told it to keep it simple and was always very clear with my prompts on what I wanted.


- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

I decided if a bug was fixed after i tested out all of the edge cases i could think of. I tried negative numbers and numbers +100. I mean it worked but it didnt like give a special warning about it being out of bounds. which is okay because it still gave the regular hints. AI helped me me understand the bugs and how they were fixed and what was the misunderstanding with the logic.

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

the secret would overwrite itself everytime the script was executed but also the "low " and the "high" was never defined because of a syntax error. Streamlit reruns your code from the beginning just in case you added anything new and session state is something the streamlit has access to, to basically keep track of everything it has done so everytime you rerun, it has a list of everything it has already done. The change i made was wrapping the secret assignment if statement so that its created only once.

- In your own words, explain why the secret number kept changing in the original app.
- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
- What change did you make that finally gave the game a stable secret number?

---

## 5. Looking ahead: your developer habits

i think questioning every single think copilot did is something ill continue doing because it feels like your talking to a fellow developer and it somewhat helps copilot review its own code and question if its any good. 

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
