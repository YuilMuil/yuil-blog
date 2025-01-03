---
title: The difficulties of finding an interesting field of research
published: 2025-01-04
description: already stated in the title bruh
tags: [English, Personal, Research]
category: Personal
draft: false
---

# Happy new years!

Heya it's YuilMuil back with another blog post, which is infact the very first post of 2025! Woo-hoo..

It's a joyous occasion and I've managed to grow so much across 2024. I started off with a education centered around Physics
and Computer Science taking multiple classes in the topic that interested and eventually went to Chung-Ang university to complete my
undergraduate education in Industrial Security which I thought was the closest to what I wanted to do.

While I don't regret this choice, I lament a tiddy-widdy bit when the required courses aren't centered to technical topics such as
Operating Systems, Compilers/Programming Languages, Networking, Distributed Systems, Multi-threading and etc which are all key topics that
I found very much interesting while doing both self-studying and taking upper-level courses at HUFS university.

Looking back, I feel that I've grown more as a person across this year where I managed to be lucky and get 3 awards in my second semester,
and learned much about management of a team/business when I was the Vulnerability Analysis basics mentor for the new recruits at SECURIOUS in my first semester.

I feel that I am rambling, but as I've gone through this journey, many times I've found that my focus or I suppose 'original resolution' often being lost in the middle of it.
Sometimes, I became arrogant in my abilites and other times I lost energy and faith at people; but throughout the time I remembered the hard times that I went through in my past
and was able to overcome each walls this year.

I also found that I've lost sight of my goals, not only because of 'corruption' or arrogance, but rather I found myself puzzled on what I want to be.

Not to toot my horn, but I've worked on both computers and software for a very long time tinkering with PSP firmware hacks and running Adventure Quest World private servers on
Hamachi and playing them with my friends when I was 10. So I'm quite adept at learning new technologies and techniques fairly quickly and getting to work on them,
but really this has lead to me trying multiple fields and changing my interests faster than a unvirtuous guy on Hongdae changing partners.

Looking back, I've really tried alot of things. 

Game Programming was really fun when I went to a Game Programming Academy by SBS when I graduated from High School for a few months,
working on DirectX11 API and Vulkan, but I quickly found that maintaining the software was mind-numbingly boring and that I only liked the idea part of creating a game rather than
debugging a collision detection function on some edge cases that made the game mechanics hacky.

Data Science was also fun, thanks to Professor Min Jin Yeong who taught both Security Statistics and Security Data Analysis classes. Infact, I feel that the aforementioned 
two classes improved my ability to connect the dots or I suppose lateral thinking ability. Because really it came down to training a model and fine-tuning it, but you have to
find a good dataset and do a EDA on it to find the insights, to then train your model based on those insights. The process of finding those insights by savaging through the Data
and looking at news articles to find topics was probably the most fun I've had in ages.

System Programming.. I'll be honest here and say that Windows/POSIX API is probably the most frustrating thing I've had to endure, but the performance improvements and decreased
overheads on some applications that I've built(namely, file managers for ElSword) was well worth it and I learned so much about how the logic underneath the abstractions of
libraries that we readily use like NettyIO work.

Reverse Engineering! This is actually what got me to work on computers to begin with, specifically I wanted to do game hacking and this is where I started out.
Dunno about other people, but reverse engineering is really a fun process and quite 'hacky' especially when you have to work with protected binaries that are protected with
say 'Themida' and have the code flow purposely obfuscated. But the process from doing static analysis and realizing that you can't read anything on IDA, so you have to check with
DiE(Detect-It-Easy) to see what protection there is and then Google how that protection works, dumping the memory using x64dbg because you don't know how to unpack it normally and
then doing analysis via IDA, finding the function you want to debug and then going to the debugger, creating theories on how it functions and confirming them via dynamic analysis..
Though, I've recently reached a 'wall' of sorts when dealing with things such as mutated code and code that is virtualized, or programs that can't simply be unpacked by
dumping the memory when it's decompressed/decrypted(.text). So recently I've been working on learning on how they work, and found out that virtualized code is essentially
a VM(Virtual Machine) and you can change it back to the original code by creating your own compiler that will translate the custom instructions back to x86(or whatever instruction set
that the protected program uses). This actually one of the reasons why my research topics include compiler/programming languages, because I want to attack this protection method in
general.

Deep Learning.. Specifically text classification is what I used for my conference paper and soon-to-be publicated journal paper at ICONI 2024. I always thought that AI
and especially text classification was resource waste compared to the output, but while doing background research on improving language model performance, I found out so much
about this domain that I didn't know about. Instruction Tuning, RAG, SLMs etc.. Which funnily enough,  I actually ended up writing a paper of a novel method of protecting
applications that make use of Prompt Engineering via Small Language Models. Looking back, I feel that this was probably the most 'research-oriented' work I've done in my entire
career. Great experience honestly, but I don't know if I'll do more work in this domain; especially because this was work based on a truly miraculous insight which I got while
talking with a reverse engineering friend on generative AI applications that aid in understanding code generated from decompilers. Shoutout to you 'KaoKao' :).

Web Programming hehe.. I have to say, I never really understood the memes behind 'fullstack engineer' but after working on a few backend APIs of my own and
making a few websites, I can safely say that 'TypeScript' is da way.(damn, am I too old to use Uganda Knuckle memes now.. eh whatever)

DevOps was interesting. Other than that AWS is expensive as hell, I found the whole thing interesting and I greatly improved my knowledge on infrastructure thanks to Professor
Jung Yong Sik's class on Informatic Security System. The whole serverless shnick, WAF(Web Application Firewall), rules etc AIO(All-In-One) package made me realize why
people say that cloud computing is the future and I think that it really is. You can basically setup a 100k$ infrastructure with most work and maintainance handled by
AWS or whatever provider(i.e Google Cloud/Azure) you use, although the fees truly brings tears to your eyes.

Anywho after going through all these topics and some more, I found all of them attractive but none of them truly appealing to the soul. Maybe it's just a 'me' problem
but I want to find 1 or 2 specialties to reach 'top' level at, while being a generalist at other things. I can do a logical argument and run them through a gauntlet, but eventually
it doesn't feel right to my 'soul'. I'm definitely interested in doing graduate level work, but it's really hard to decide what domain I want to do this in.

At any rate, I've typed my frustrations for about an hour.. I'm not sure if anyone else has this same predicament, but I hope that you will be able to resolve this problem.
I'm already at my senior year at undergrad and I graduate next year; yet I still haven't chosen a field to domain in. Hopefully, I can find the 'one' by this winter break and
join a research lab on that domain, and maybe find 'that girl'(a grill like a foremans xd) as well.

That's the end of this article. I'm too lazy to proof-read or put this through AI(+AI makes this seem that much less authentic), so do forgive me if the wording or grammar seems off.

gnight yall and happy 2025. I hope that you guys can achieve your dreams, just like how I will achieve mine. 

Yours truly, YuilMuil