---
layout: post
title:  "First Post..."
date:   2025-01-30 07:48:08 -0500
categories: PLC automation 
image: IMG_0914.jpg
---
Welcome to my blog. I've made attempts to blog off and on since probably about 2010. For some reason I don't stick with it. I'm sure there are old blog posts with examples of linked lists or binary searches that I wrote in Java. Enough with the nostalgia...

I should make a template for these posts. I think I have a program in a repo somewhere. Until then, the command listed below is what I used to generate this post, at least the shell of it.

```bash
cp _posts/2025-01-27-welcome-to-jekyll.markdown _posts/$(date +%Y-%m-%d)-first-post.md
```
I found myself with an interest in Automation and Controls. The only issue is that I don't have the credentials or experience. Despite that, I figure logic is logic. I have taken a few PLC programming classes, so I am not completely blind, but my experience is entirely in lab setting. It's a lot easier to make mistakes when there isn't a physical body on the other end of the component you're controlling.

I found myself with a box of parts and an Allen Bradley Micro820(Allen Bradley Micro820 PLC 2080-LC20-20QBB Ethernet I/P Controller) PLC. The peripherals were already wired, which leaves me with the task of wiring the the I/O components to the PLC. I've got a preliminary wiring, though it's not finished. Preliminary continuity tests show things seem OK. However, If you look closly at the pictures, you can see that I made a mistake when wiring the analog input. According to the Micro820 manual, Inputs I-00:I-03 are shared between digital and analog inputs. In short, I need to move the analog input device to one of the first four inputs.

![Image](/images/2025-01-30-first-post/IMG_0914.jpg)
![Image](/images/2025-01-30-first-post/IMG_0915.jpg)
![Image](/images/2025-01-30-first-post/IMG_0918.jpg)


Docs: [Micro820 User Manual](https://literature.rockwellautomation.com/idc/groups/literature/documents/um/2080-um005_-en-e.pdf)


More to come.


