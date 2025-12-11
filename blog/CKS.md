---
layout: page
permalink: /blog/web/CKS.html
title: "CKS Certification: Thoughts"
---

#  CKS Certification: Thoughts

![Badge](/images/resources/CKS/CKS_badge_1.png){: .align-center}


<!-- <figure  class="align-center" >
  <img src="{{ site.url }}{{ site.baseurl }}/images/resources/CKS_badge_1.png" alt="">
</figure> 
<br> -->

## Introduction
After passing CKA almost a year ago, I figured it was time to take on the Certified Kubernetes Security Specialist (CKS). The name itself suggests something exciting: secrets, exploits, some red-teaming and Pwning, and maybe some insights into securing large-scale systems. In reality? It’s more like... putting locks on doors you already installed during CKA.

I passed the exam with above average score, but felt a need to share a few thoughts on the course itself. Let's justify why.

---
## Why I took CKS
Because clearly, one Kubernetes cert wasn't enough self-inflicted pain.


Let’s start with what I *thought* I was signing up for. I assumed CKS would be a continuation of CKA, something in the lines of "now that you can deploy K8s clusters, let's secure it like a paranoid ex-NSA agent." 
But no. What it really taught me was how to apply some best practices from the Linux hardening playbook — [AppArmor](https://apparmor.net/), [seccomp](https://en.wikipedia.org/wiki/Seccomp), file permissions, and audit logs. Most of which I’d already seen before... in a different context.

Don't get me wrong, I enjoyed this course, I really did. I didn't take [Mumshad's CKS course](https://kodekloud.com/courses/certified-kubernetes-security-specialist-cks) (in retrospect, maybe I should have) But this godsend [video](https://www.youtube.com/watch?v=d9xfB5qaOfg) of the Killer Shell's online course saved my day. I think I didn't have as much practice as I wanted, but yeah, somehow I was able to scrap through.

<!-- <iframe width="420" height="315" src="http://www.youtube.com/embed/d9xfB5qaOfg" frameborder="0" allowfullscreen></iframe> -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/d9xfB5qaOfg?si=rzgDZ21skAB7UbXv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


Also, the Youtube course DOES NOT COVER CILIUM. You had no idea how much docs I had to parse through to get a feel of the tool. A thousand docs can’t beat one working example.

---
## What Surprised Me
Not all surprises are pleasant, but hey, at least they were consistent.
CKS requires CKA as a prerequisite, but I never bothered revisiting those old, practically unused (at least for me) CKA concepts. So, when it was time to dive into CKS, I ended up spending three hours just doing a rundown of the documentation. <br>I know many people manage to knock out both certifications within a few months, so it probably makes more sense for them. If you're interested in my [previous views](https://sanathnu.github.io/blogs/web/CKA.html) on CKA, check it out.<br>
That said, when it comes to CKS itself:
* **Security Principles?** Almost entirely assumed knowledge. If you’ve spent any time with Linux permissions, firewall rules, or container security basics, you’re already 80% there.
- **Tooling?** You’re introduced to tools like Falco (for runtime threat detection), AppArmor/SELinux (for confinement), and others. But most of it I felt was at surface-level:  “install this, write a config, hope it works.” ([CIS benchmarking](https://www.cisecurity.org/benchmark/kubernetes), you're good, don't worry)
- **Network Policies?** Honestly, they’re probably the easiest part of the exam if you’ve practised even a little beforehand.

There’s an underlying assumption that you already know how containers and pods behave, and now you just need to lock them down with some `yaml` and good intentions.

---
## What Fell Short
Besides my expectations? The idea that this cert was about _security systems_ .

I expected this to be about learning about threat modelling, defence in depth, compartmentalisation , maybe maybe some read teaming. What I got instead was....an applied patchwork.

Case in point: one of the exam scenarios pulls out the same tired example of the [Tesla Hack](https://www.wired.com/story/cryptojacking-tesla-amazon-cloud/). I’ve seen that example so many times (while studying) it might as well be part of the CKS welcome banner. In any halfway decent org today, you're not just flipping admin access like a switch. **You’re filing a Jira ticket, then waiting three business days while the approval chain makes its slow pilgrimage through the temple of compliance.** RBAC is standard hygiene now, not some cutting-edge revelation.
![Tesla hack!](/images/resources/CKS/telsa_hack.png)

<br>
The certification  isn't about **understanding security** in the context of cloud (of which k8s is a huge part now), but about applying pre-baked controls in a time-boxed fashion. You don’t need to *understand* security concepts but just need to memorize which command disables privilege escalation and how to configure a PodSecurityPolicy (or whatever’s [replacing it](https://kubernetes.io/blog/2021/04/06/podsecuritypolicy-deprecation-past-present-and-future/) this week).[^1]

Also: **time limits are brutal**. You don’t really have the luxury of pausing to understand why something works. I realized this in the trial exam on [Killer Koda](https://killercoda.com/killer-shell-cks) which gave me a reality check. You apply what you practised, and you move on.

---
## Where It Wins
There *is* a bright side. Despite everything, the CKS does a few things well and they're worth acknowledging.
- **Hands-on Realism:** I enjoyed debugging more in CKS scenarios than in CKA. They reflect the kind of chaos I've seen in real world. Misbehaving pods, weird log outputs, tools falling silently, the whole shenanigans.
- **Tooling Diversity:** I liked the general exposure apart from the K8s ecosystem to the Linux environment. (Thought windows is out of the loop though[^2]). How audit logs , runtime security tooling, file monitoring and all are integrated into some tightly coupled linux tools (especially something like apparmour) is the right method.
- **A macroscopic attacker POV**: I've done my fair share of red-team YouTube video binging and some thoughts like [security](https://kubenomicon.com/Persistence/Malicious_admission_controller.html) in MutatingAdmissionWebhook and ValidatingAdmissionWebhook were something that genuinely I liked.

There’s something uniquely satisfying about spotting a misconfigured RBAC rule or a permissive seccomp profile and fixing it, especially when under pressure. That experience alone makes the cert *feel* valuable, even if the learning curve isn’t as steep as you’d hoped.

---
## Final Take
Would I recommend CKS? That depends. If you're coming from CKA and expecting to *go deeper*, you might be disappointed. There are some interesting resources online regarding breaking large k8s clusters, this isn't about it. It doesn’t teach you how to build secure systems; it shows you how to lock down what's already built.

The irony of modern DevSecOps is that it preaches security as culture but practices it as compliance. Going through CKS felt like that. You're not taught to think securely, just to behave securely, like a well-trained monkey with `kubectl`. 

But if you like hands-on debugging, practical applications, and learning to quickly recognize misconfigurations in high-stress environments? CKS is excellent practice.
### TL;DR:
- Don’t expect deep security theory. Expect checklists and YAML.
- Practice more than you study.
- Learn to debug 3rd-party tools as they *will* break.
- Don’t look for “aha!” moments. Look for “oh crap, better fix this fast.”

Would I do it again? Probably.  
Would I recommend it to someone expecting a security deep dive? Absolutely not, unless you believe watching cricket highlights is the same as experiencing a full Test match.

---
## Resources
#### Mindmap
Here's a very crude mindmap of what notes I summarized right before the exam. Might be helpful for visual folks. 

![I don't know how Obsidian canvas works man, it's just weird! ](/images/resources/CKS/CKS_mindmap.png)
If the font is too hard to read, download the image maybe?

#### Github links
* [Walid Shaari's CKS repo](https://github.com/walidshaari/Certified-Kubernetes-Security-Specialist)
* [Abdennour's CKS repo](https://github.com/abdennour/certified-kubernetes-security-specialist)
* [Kubernetes Security Checklist and Requirements](https://github.com/Vinum-Security/kubernetes-security-checklist) (old but gold)

#### Other
* [Killer.sh CKS practice exam](https://killer.sh/cks)
* [Killer Shell CKS scenariors](https://killercoda.com/killer-shell-cks)

And of course, the docs, which I'm confident y'all can find yourselves 😄

*PS: This is a great cert to put on your resume. Just don't expect it to turn you into a security architect overnight.*

[^1]: I found this very cool gitbook called [The Kubenomicon](https://kubenomicon.com/Kubenomicon.html#what-is-the-kubenomicon) which was actually something that I liked. It gives you "knowledge to the cloud hacker". I still have to read through it.
[^2]: I have absolutely zero k8s on windows experience. The security principles there should open another Pandora's box. I'll get into it maybe later in my career?
