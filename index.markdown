---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home

---

# Blackouts

[Blackouts](https://netblocks.org/reports) occur frequently around the world, usually due to oppressive regimes that cause these blackouts in an effort to control their population.
Communication is a basic human right ([UDHR](https://www.un.org/en/about-us/universal-declaration-of-human-rights), Article 19), and thus we need to work on tools that would help people in affected regions.

# Moby

Moby solves this using a bi-modal design, using the Internet to establish trust among users and prepare them for blackouts.

![Bi-modal design](/assets/bimodal.png){:class="img-responsive"}

During blackouts, users can rely on the Moby Ad-Hoc network to communicate with each other.
Further details on how these modes work can be found in our paper.

---

## Paper

For more details please read our [PETS 2022 paper](https://petsymposium.org/2022/files/papers/issue3/popets-2022-0071.pdf).

Moby: A Blackout-resistant Anonymity Network for Mobile Devices *PETS 2022*

*Amogh Pradeep (Northeastern University), Hira Javaid (Northeastern University), Ryan Williams (Northeastern University), Antoine Rault (EPFL), David Choffnes (Northeastern University), Stevens Le Blond (EPFL), and Bryan Ford (EPFL)*

---

## Moby Client

The Moby Client is implemented as an Android app.
It is based on the Signal application and extends it to enable P2P communication using Wi-Fi direct and Bluetooth.

Client [code](https://github.com/amoghbl1/moby_android) can be found on GitHub.

## Moby Simulator

We run Moby simulations on call data records (CDR).
The CDR data is as follows.
- Towers with associated locations
- User call data
  - Tower where this was made/received
  - Hour when this was performed
- User SMS data
  - Tower where this was sent/received
  - Hour when this was performed

Using this, we simulate Moby and multiple attacks on its Ad-Hoc network. The [code](https://github.com/00h-i-r-a00/moby_simulator) used to process and work on CDR data can be found on GitHub.

---

This work was supported by the National Science Foundation (Grants: SaTC-1618955 and ProperData SaTC-1955227).
