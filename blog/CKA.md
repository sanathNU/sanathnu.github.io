---
layout: page
permalink: /blog/web/CKA.html
title: CKA
---
# CKA Certification: Insights and Experiences

<!-- ![](https://upload.wikimedia.org/wikipedia/commons/thumb/3/39/Kubernetes_logo_without_workmark.svg/2109px-Kubernetes_logo_without_workmark.svg.png){: width="200px" height="100px" .align-center}
 -->

![Badge](/images/resources/CKA_badge.png){: .align-center}


## Introduction

Hello, first things first. This is not for people who have never heard of terms [containerization](https://en.wikipedia.org/wiki/Containerization_(computing)) and/or [Kubernetes](https://kubernetes.io/) (which is more [container orchestration](https://www.redhat.com/en/topics/containers/what-is-container-orchestration)). This post dwelves into depth of the [Certified Kubernetes Administrator (CKA)](https://training.linuxfoundation.org/certification/certified-kubernetes-administrator-cka/) exam, which seems to be gaining traction.

So, if any of those folks are here, consider yourself warned. I do not want to bore you with the details of how the exam was or what the procedure is. I'm sure you will find lots of resources on the internet. If you want an optimistic outlook, take a look at the [CNCF success story](https://www.cncf.io/blog/2021/07/30/success-story-preparing-for-kubernetes-certification-improves-a-platform-development-engineers-skill-set/) from four years ago.

Now, with those preliminaries out of the way, let me tell you what this post is about. Many people online drone on about the benefits of the CKA exam. I wanted to offer a more balanced view after undergoing the examination and experiencing its practical benefits. I've gotten my certification in 2024, which gives me exactly 1 year worth of brownie points to talk about the exam. 

After this extensive testing and examination (high usage!). I've come to a nuanced conclusion: the CKA certification is indeed useful, but not necessarily essential for advancing as an engineer in the cloud computing domain.

---
## Understanding CKA Certification
If you're diving into K8s from scratch, think of it as Google's way of managing containers, born from their original [Borg](https://en.wikipedia.org/wiki/Borg_(cluster_manager))[^1] system. Getting CKA status boosts your skills, showing you can handle app development and troubleshooting in real-world situations. It's a part of becoming the recently released a [Kubestronaut Program](https://www.cncf.io/training/kubestronaut/), which CKA is a starting point.

People go for CKA because they think it'll make them more employable (it does, but it's not a silver bullet). It's good for getting a solid grip on the basics of Kubernetes, though the exam isn't overly tough if you prep well.

Since it can be [pricey](https://www.cncf.io/training/certification/cka/) ($445 in 2025!) to certify on your own, a lot of folks get their companies to foot the bill. Fun fact: in 2023, a whopping 176,000 people signed up—that's more than double the numbers from 2021 (2023 report, 2021 report). This shows how hot Kubernetes skills are becoming in tech, especially for cloud-native development.

---
## My Comments on the Exam
Well, diving into Kubernetes opened my eyes to its [awesome documentation](https://kubernetes.io/docs/home/) — seriously good stuff. It's well-organized and explains things way in a lucid way. But I was thoroughly disappointed by the [shutdown of the K8s labs](https://kubernetes.io/blog/2023/02/14/kubernetes-katacoda-tutorials-stop-from-2023-03-31/) that were there earlier. I remember playing around it in 2020, and I totally didn't understand what I was doing. But the platform being present gave me a sense of "I could come back to it anytime I want".

On the flip side, KillerCoda's [exam simulations](https://killercoda.com/cka) are top-notch. They really nail down how to debug in a cloud setup, which is crucial. Personally, tackling the exam shed light on complex systems like Kubernetes certification mechanisms (not just the piece of paper, but tools like cert-manager) and schedulers — it was a rewarding experience.

It also helps you keep up with the evolving cloud native ecosystem.The world has moved to containerized services and it ain't going away at least for a decade. By then you can make your millions and retire. 

Plus, getting involved in Kubernetes open-source community opens up some exciting possibilities. As K8s becomes the backbone for AI and beyond, contributing to its evolution puts you right in the thick of things—like being a top surgeon in a cutting-edge operation.

---
## Study Thoughts
> "All topics are equal, but some topics are more equal than others."  

**TL;DR**: It's easier than your term exam in uni.
<br> <br>
This is because most of the exam dwells on the fact that you _understand_ the concepts behind the exam, and are able to work with it. The exam is completely hands on. There's literally no way for anyone to pass the exam without ever touching a k8s cluster before. It's not because no knowledge, it's because the time is short.
I'd compare this hands-on practical certification exam to a "Karate Combat" rather than "university type exam". You simply can't go in without experience.

Here's a list of distilled thoughts on the exam:

* Get your exam scheduled first. This gives you a deadline to work with. Keep 3 weeks minimum.
* Try your hand at setting up Kubernetes on different platforms—bare metal, cloud setups like AWS or Azure, or Docker. Check out resources like Kubernetes the Hard Way on Bare Metal[^2], or Kubernetes the Hard Way on Docker[^3] 
*  Definitely some concepts are much more important than the others. Focus on mastering concepts like configmap, secrets, and network mesh—they're crucial for building and testing apps, unlike lower-level stuff like [cri-o](https://cri-o.io/) or [containerd](https://containerd.io/) (not to say that they are unimportant, but not for the exam).
*  Know the documentation like your instagram ID. Be sure to able to navigate to important topics (like [this one](https://kubernetes.io/docs/tasks/administer-cluster/configure-upgrade-etcd/)) and be finger-quick.
*  Time is of absolute essence, treat it right. My question attempt approach order: easy-but-long ones first, easy-small-ones, documentation required medium-small-ones, unknown-ones.
*  Practice, practice and practice.

At the very end, have fun! Unlike the routine of rote memorization, this is fun, there's some problem, created by a very specific breakdown of a component or a configuration. If you know it, you can solve it. It's as simple as that. There's no ambiguity. Only the lack of knowledge.

---
## Resources
These resources are just some of them which I used during my preparation for the exam. Most of it was the K8s documentation. But some of them helped me gain perspective on how to study for the exam. These are also very unstructured. Go through them at your own risk lol.


#### Basic Resources
* [CKA curriculum v1.29](https://github.com/cncf/curriculum/blob/master/CKA_Curriculum_v1.29.pdf)
* [Borg Orignal paper](https://research.google/pubs/large-scale-cluster-management-at-google-with-borg/)
* [David's Study Guide](https://github.com/David-VTUK/CKA-StudyGuide/tree/master)
* [OWASP Kubernetes Security Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Kubernetes_Security_Cheat_Sheet.html)
* [CKA Practice Questions](https://gist.github.com/texasdave2/8f4ce19a467180b6e3a02d7be0c765e7)

#### Reddit Threads
* [https://www.reddit.com/r/kubernetes/comments/s6rpb6/free_materials_for_cka_certified_kubernetes/](https://www.reddit.com/r/kubernetes/comments/s6rpb6/free_materials_for_cka_certified_kubernetes/)
* [https://www.reddit.com/r/kubernetes/comments/s6l7xs/just_passed_the_cka_here_are_some_tips_and_tricks/](https://www.reddit.com/r/kubernetes/comments/s6l7xs/just_passed_the_cka_here_are_some_tips_and_tricks/)
* [https://www.reddit.com/r/kubernetes/comments/ssxhsd/cleared_my_cka_exam_with_a_score_of_92_here_are_a/](https://www.reddit.com/r/kubernetes/comments/ssxhsd/cleared_my_cka_exam_with_a_score_of_92_here_are_a/)


#### Youtube Videos
* Pretty Awesome video: [CKA Certification SURE SHOT Questions ](https://www.youtube.com/watch?v=vVIcyFH20qU)
* [K8s Source Code Walkthrough](https://www.youtube.com/watch?v=F8dZMKP6xyg)

#### **K8s the hard way**
* [The OG k8s the hard way](https://github.com/kelseyhightower/kubernetes-the-hard-way ): 
* [On AWS](https://github.com/Praqma/LearnKubernetes/blob/master/kamran/Kubernetes-The-Hard-Way-on-AWS.md)
* [On Baremetal](https://github.com/Praqma/LearnKubernetes/blob/master/kamran/Kubernetes-The-Hard-Way-on-BareMetal.md)
* [On Docker](https://github.com/brightzheng100/kubernetes-the-hard-way-on-docker)

[^1]: [Borg Orignal paper](https://research.google/pubs/large-scale-cluster-management-at-google-with-borg/)
[^2]: https://github.com/Praqma/LearnKubernetes/blob/master/kamran/Kubernetes-The-Hard-Way-on-BareMetal.md
[^3]: https://github.com/brightzheng100/kubernetes-the-hard-way-on-docker
