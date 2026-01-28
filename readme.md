# Flirt-Sense 😏  
### idk ab u guys but i absolutely cannot read signals

a text classification model that detects whether a message contains flirting intent.

> built bc my brain takes ~10 years to process emotional information. jsfc.

---

## why does this even exist

idk ab u guys but i’ll be laying in bed at like **3am**, doing nothing,  
and my brain just decides to ruin my life.

suddenly i remember a message from YEARS ago and go:

“oh.  
that was flirting.”

and then i remember what i replied with.

“haha yeah”

absolute horrendous behavior.

so instead of growing as a person, i made a model.

---

## the problem

flirting is never clear.

it’s always hidden behind:
- “btw”
- “haha”
- “no worries!”
- “random thought but—”

and if you’re even slightly:
- tired  
- distracted  
- socially delayed (me)

you will miss it.

humans are bad at this.  
i am worse.

---

## the approach (aka me coping)

- distilbert fine-tuned for **binary classification**
  - `yes` → flirting detected
  - `no` → just talking (probably)
- custom dataset full of:
  - slang
  - mixed signals
  - texts that ruin your night once you understand them
  - “i wasn’t flirting… unless 👀” energy
- trained with **pytorch** + **hugging face transformers**
- evaluated on held-out validation + test sets

basically i stopped asking:
“was that flirting?”

and let the model decide bc i clearly can’t.

---

## results (embarrassingly good)

- **validation accuracy:** `0.98`
- works well on:
  - subtle flirting
  - mixed-signal texts
  - messages that only make sense after character development

the model gets it.  
i didn’t.

---

## examples

| text | prediction |
|------|-----------|
| “i finished the report btw… also i kinda miss talking to you” | yes 😏 |
| “can you send me the slides later?” | no |
| “haha ur funny we should hang out sometime maybe” | yes. wake up. |
| “no worries!!” | idk man. dangerous. |

---

## tech

- python  
- pytorch  
- hugging face transformers  
- distilbert  
- unresolved personal issues  

---

## use cases

- confirming you fumbled
- validating your overthinking
- rereading old chats and feeling worse
- avoiding the same mistake (optional)

---

## disclaimer

this model only detects **flirting intent**.

it does NOT:
- tell you what to reply
- stop you from panicking
- fix ur personality

if it says “yes” you can still mess it up.
trust me.

---

## tl;dr

**flirt-sense 😏** exists bc:
- i missed the signs
- i still think about it
- i had time, a gpu, and zero self-awareness

sometimes it wasn’t friendly.

u were just slow.
