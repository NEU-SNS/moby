---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

Moby: A Blackout-resistant Anonymity Network for Mobile Devices [PETS 2022](https://petsymposium.org/2022/files/papers/issue3/popets-2022-0071.pdf)

*Amogh Pradeep (Northeastern University), Hira Javaid (Northeastern University), Ryan Williams (Northeastern University), Antoine Rault (EPFL), David Choffnes (Northeastern University), Stevens Le Blond (EPFL), and Bryan Ford (EPFL)*

**Abstract:** Internet blackouts are challenging environments for anonymity and censorship resistance.
Existing popular anonymity networks (e.g., Freenet, I2P, Tor) rely on Internet connectivity to function, making them impracticable during such blackouts.
In such a setting, mobile ad-hoc networks can provide connectivity, but prior communication protocols for ad-hoc networks are not designed for anonymity and attack resilience.
We address this need by designing, implementing, and evaluating Moby, a blackout-resistant anonymity network for mobile devices.
Moby provides end-to-end encryption, forward secrecy and sender-receiver anonymity.
It features a bi-modal design of operation, using Internet connectivity when available and ad-hoc networks during blackouts.
During periods of Internet connectivity, Moby functions as a regular messaging application and bootstraps information that is later used in the absence of Internet connectivity to achieve secure anonymous communications.
Moby incorporates a model of trust based on users’ contact lists, and a trust establishment protocol that mitigates flooding attacks.
We perform an empirically informed simulation-based study based on cellphone traces of 268,596 users over the span of a week for a large cellular provider to determine Moby’s feasibility and present our findings.
Last, we implement and evaluate the Moby client as an Android app.

---

## Code

### Client

The Moby Client is implemented as an Android app.
It is based on the Signal application and extends it to enable P2P communication using Wi-Fi direct and Bluetooth.

Client [code](https://github.com/amoghbl1/moby_android) can be found on GitHub.

### Simulator

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

This data was approved by Northeastern's [IRB](https://research.northeastern.edu/hsrp/).

---

This work was supported by the National Science Foundation (Grants: SaTC-1618955 and ProperData SaTC-1955227).
