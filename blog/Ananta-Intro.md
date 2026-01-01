---
layout: page
permalink: /blog/web/Ananta-Intro.html
title: The Dream of Ananta
---
# The Dream of Ananta
> _This is the first post in a series about ಅಕ್ಷರ ಮಂಟಪ (Akshara-Mantapa), a Library of Babel implementation for Kannada. Over five posts, I'll trace the path from a night sky in Boston to a working infinite library through philosophy, linguistics, mathematics, and engineering._

**The Series:**

೧. **The Dream of Ananta**: You are here

೨. [Exploring the Infinite Libraries](/blog/web/Exploring-Infinity.html): a hands-on guide to both libraries

೩. [Taming Infinity](/blog/web/Taming-Infinity.html): the mathematics of bijection

೪. [Engineering Infinity](/blog/web/Engineering-inf.html): Rust, WASM, and making it run

೫. [Reflections from Infinity](/blog/web/Reflections-inf.html): what I learned



## I. The Night Sky and Boredom

It had been a few months since I landed in Boston, and I had been itching to do something interesting. Something fun. There were many inspirations, but a particularly beautiful night of Aurora Borealis in November got me thinking. The Sun's (ಸೂರ್ಯ) gift, arriving days after the geomagnetic storm that caused it. 

<br>

![](/images/post_images/night-sky.jpg){:style="display:block; margin-left:auto; margin-right:auto"}
*A beautiful night*

<br>

Watching the particles dance independently, each an aggregation of ions, yet creating something unified and breathtaking, made me think about emergence. And infinity. And with that came the old thoughts and problems.

---

## II. Old Fascinations

I was always fascinated with infinity (ಅನಂತ) once I first heard of it. The first formalized paradox I encountered was [Hilbert's Hotel](https://en.wikipedia.org/wiki/Hilbert%27s_paradox_of_the_Grand_Hotel). It seems obvious at first (of course you can shift rooms to accommodate another guest, it has infinite rooms!) but then, slowly, I started to understand the consequences: the countability, how mindbogglingly insane our abstractions are.

The [Banach-Tarski paradox](https://en.wikipedia.org/wiki/Banach%E2%80%93Tarski_paradox) made another appearance as a mathematical supermodel for confusing a person, splitting a sphere into two identical spheres, mathematics defying intuition. These ideas had festered in my mind for years, dormant but present. I had an inkling of the complexity, and I wanted to have fun with it.

---

## III. The Library Appears

One day, the YouTube gods blessed me with an [age-old video](https://www.youtube.com/watch?v=GDrBIKOR01c) from Vsauce about lasting messages. And then came the bomb: _The Library of Babel_. Such a fascinating story. Borges came across as someone who wrote no-bull stories about concepts that genuinely fascinated him, and I like him for it. His 1941 short story imagined hexagonal rooms containing every possible arrangement of 3,200 characters, every book that could ever be written, already there, waiting.

And then I discovered [Jonathan Basile'](https://jonathanbasile.com/)s implementation of it. He actually goddamn captured infinity. I urge you to go check out the website immediately. Watch Vsauce's explanation to get a better view of this idea. It is truly fascinating, and keep an open mind on it (don't mind the three-minute detour!)

→ [libraryofbabel.info](https://libraryofbabel.info/) → [Vsauce: Messages For The Future](https://www.youtube.com/watch?v=GDrBIKOR01c)

---

## IV. LLMs and Tamed Infinity

I have been working in deep learning for a few years now, and I've watched how slowly but surely, thoughts have become tokens, and thinking has become computing. This forms the crux of how generative AI is viewed nowadays. But Borges' infinity is older, eternal. It's more akin to what I'd call ಜ್ಞಾನ ದೈತ್ಯ, a knowledge demon, a cousin to Laplace's demon.

<br>

![](/images/post_images/mantapa-mandira.png){:style="display:block; margin-left:auto; margin-right:auto"}
*A temple for the mad*

<br>

LLMs extract value from infinity. We build them by burning vast amounts of money for better probabilistic outputs (imagine how crazy our ancestors from the 1950s would think we are, spending fortunes to keep computers running, and boom, you get AI). We're taming infinity, one bit at a time, with GPUs.

Here's an analogy: our training data is the boulder, and the neural networks are beautiful sculptures carved from it. The weights are the form we've extracted. No matter how big the boulder gets, infinity is always bigger. It's like comparing a grain of sand to the total length of the observable universe. But this infinity, the infinity of words we've captured in LLMs, is still bounded, still human-shaped, still compressible.

---

## V. True Infinity — ಅನಂತ

True infinity is different. Not dramatic. It is something passive, enormous, omniscient. Not "nature red in tooth and claw" but a liminal space where everything already exists, waiting. But what about raw infinity? We have tamed it yes, but what about the true nature of things, the connections and the missed connections, is it not as simple and as beautiful as Plato's world of forms?

I'd encountered the [infinite monkey theorem](https://en.wikipedia.org/wiki/Infinite_monkey_theorem) before, and I understood both its value and its futility the moment I tried to grasp its logic. At least the English library contains every work of Shakespeare, and every transliterated version of ಕನ್ನಡ and ಕುವೆಂಪು ([Kuvempu](https://en.wikipedia.org/wiki/Kuvempu)), as well as every work of Borges in Kannada. Weird, isn't it? But most of infinity is just noise. Terrifyingly ordinary. It's not something we humans can hold in our minds. Let us leave it for the ದೈತ್ಯ.

---

## VI. Structure Within Infinity

When I first watched Vsauce's video years ago, I didn't have the programming guts to understand how Basile's implementation worked. But now it seemed conquerable. After going through various blogs and theorems, I understood the shape of his algorithm, and I wanted to play with it.

The philosophical weight hit me: a mathematical system that knows everything that could ever exist. Though truly infinite, Basile shrunk it down to 3,200 characters per page (still 29^3200 possible pages, which is incomprehensibly large yet smaller than [Graham's number](https://en.wikipedia.org/wiki/Graham%27s_number)(my own g-factor certainly doesn't scale like g(n)). The number doesn't blow up the same way in Kannada, but I'll get to that later.

The website's invertibility is the key. It allows you to have omniscient knowledge of every text that ever existed or could exist. But the kicker: _you, the searcher_, must already know what you seek. From "seek and ye shall find" to "know and ye shall find."

> ಅರಿವೇ ಗುರು (Awareness itself is the teacher)

---

## VII. But What About Other Languages?

The library is beautiful in its Latin roots, but what about other languages? All of the thousands of combinations and concepts that we can use, all the phonetic and grammatical systems. I thought about [Claude Shannon](https://en.wikipedia.org/wiki/Claude_Shannon), the man who stripped communication down to bits, and [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing), who made a machine that works on bits, truly changing how we think about thought. (I read about this in [_The Information_](https://en.wikipedia.org/wiki/The_Information:_A_History,_a_Theory,_a_Flood) by James Gleick, you should give it a read.) It's infinite, how we choose to represent information. Each script is its own universe of possibilities. And that's why I turned to ಕನ್ನಡ , my mother tongue.

---

## VIII. Why Kannada

I am from [Karnataka](https://en.wikipedia.org/wiki/Karnataka), and my mother tongue is [Kannada](https://en.wikipedia.org/wiki/Kannada). You don't really think about your mother tongue until you understand its value. All those boring lessons in school were teaching me how to think in a language, and after gaining "language consciousness," I truly can't let go of my roots. The dialects, the imbued culture, it's something too real to release.

Not to be anthropomorphic about language, but mother tongue holds a deep connection with you, no matter where you are (unless someone gives me deranged amnesia lol). Being totally in sync with my language, no matter how many thoughts I have, is a lost goal. I would love to be fully lost in ಕನ್ನಡ, but computers and theory became my true calling. Maybe in another life, another time.

I wanted to give back to the language, to make a contribution to infinity by trying to capture it in Kannada's syllabary. And hence came this project: **ಅಕ್ಷರ ಮಂಟಪ** (Akshara-Mantapa), the Library of Babel in Kannada. Also, it involved fun math and engineering challenges, so the ride has been enjoyable.

---

## IX. What Comes Next

The project is live: [https://sanathnu.github.io/Akshara-Mantapa/](https://sanathnu.github.io/Akshara-Mantapa/)

In the next post, I'll give you a proper introduction to both libraries, how to use libraryofbabel.info and Akshara-Mantapa, what you can do with them, what it feels like to hold a piece of infinity.

Following that: how Kannada [graphemes](https://en.wikipedia.org/wiki/Grapheme) were modeled (it's not just different letters), the mathematics of bijection, the frontend and deployment, and finally, reflections from inside the infinite.

---

## X. Closing

I'll admit this has been a tongue-in-cheek philosophical pre-introduction to a project. But I wanted to convey the enormous weight of infinity and all its fascination. I'm not like an astronaut who can abstract away the problem and focus purely on solving it. I enjoy every part: the theory, the tangents, the wonder. It's fun.

Like the aurora that started this: particles acting alone, meaningless in isolation, yet creating something whole together. The library is the same. Individual characters, noise on their own, containing everything when combined.

> ಒಂದು ಅಗಳಲ್ಲಿ ಒಂದು ಸಾಗರ (An ocean in a grain)

The library has been waiting for you.

---

_Next: [Post 2 — Exploring the Infinite Libraries]_