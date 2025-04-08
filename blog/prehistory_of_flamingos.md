---
pub_date: Tue, 08 Apr 2025 09:01:37 -0700
description: Explains Flamingos history
---

# Prehistory of Flamingos

Back in the day (around 2017), Philipp Oppermann published
the first version of his blog entitled [Writing an OS in
Rust]. As the name implies, this blog described how to write
a very simple OS mostly from scratch in Rust. The resulting
"Blog OS" ran on a standard x86 laptop. This project was
quite a popular read. Philipp produced [Writing an OS in
Rust (2nd ed)] soon thereafter.

In 2024 Bart Massey wanted to reproduce this success on
newer hardware. Very cheap ARM processor boards were
available that were nonetheless multicore, with decent MMUs.
These boards were also better-documented and more accessible
than x86 laptops.

Bart was lazy and a bit ignorant, and thus asked Phil to
"help". Phil graciously agreed, and thus a new Blog OS was
born.

The new team looked at a lot of hardware options. A first
attempt with the [milkV Duo], a ridiculously inexpensive
(US$5-ish) board running Linux out-of-the-box, failed due to
lack of documentation and concerns about future
availability. The second try involved the [Raspberry Pi Zero
2 W] (PZ2W). This board was a little more expensive at around
US$15, but much better documented and with a clear long-term
availability story. As a 64-bit quad-core part with an MMU,
the PZ2W would be a great target for a "real OS". This seemed
promising.

As the team started to poke at this, they found an
interesting thing. Hidden in plain sight was *another* Blog
OS, published under the banner of the Rust Embedded Working
Group. This was `rust-raspberrypi-OS-tutorials` by Andre
Richter, with a kernel semi-secretly known as [mingo]. This
series showed a lot of development of an OS for Raspberry Pi
3b and Raspberry Pi 4 with clear code and many exciting
features. The code also turned out to work well with the
PZ2W, which is very similar to the Pi 3b. Philipp and Bart
decided not to do their own thing, but revamp Mingo and blog
it, with Andre's blessing.

Andre had named the kernel Mingo as a short form of
Flamingo. Philipp and Bart decided the OS as a whole would
be Flamingos: not a "flaming OS", just two or more birds.

[Writing an OS in Rust]: https://os.phil-opp.com/edition-1/
[Writing an OS in Rust (2nd ed)]: https://os.phil-opp.com/
[milkV Duo]: https://milkv.io/duo
[Raspberry Pi Zero 2 W]: https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/
[mingo]: https://github.com/rust-embedded/rust-raspberrypi-OS-tutorials/
