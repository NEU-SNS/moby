---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

Paper published at [PETS 2022](https://petsymposium.org/2022/files/papers/issue3/popets-2022-0071.pdf).

Moby: A Blackout-resistant Anonymity Network for Mobile Devices

*Amogh Pradeep (Northeastern University), Hira Javaid (Northeastern University), Ryan Williams (Northeastern University), Antoine Rault (EPFL), David Choffnes (Northeastern University), Stevens Le Blond (EPFL), and Bryan Ford (EPFL)*

## Code

### Client

The Moby Client is implemented as an Android app.
It is based on the Signal application and extends it to enable P2P communication using WiFi direct and Bluetooth.

Client [code](https://github.com/amoghbl1/moby_android) can be found on github.

### Simulator

We run Moby simulations on CDR data.
The CDR data is as follows.
- Towers with associated locations
- User call data
  - Tower where this was made/received
  - Hour where this was performed
- User SMS data
  - Tower where this was sent/received
  - Hour where this was performed

Using this, we simulate Moby and multiple attacks on its Ad-hoc network. The [code](https://github.com/00h-i-r-a00/moby_simulator) used to process and work on CDR data can be found on github.

Use of this data was approved by Northeastern's [IRB](https://research.northeastern.edu/hsrp/).

---

This work was supported by the National Science Foundation (Grants: SaTC-1618955 and ProperData SaTC-1955227)
