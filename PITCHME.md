<img src="assets/studiumwave.ai.300.png" style="width: 300px; border: none; box-shadow: none"/>

## Underwriting system
Introduction

---

<span style="color: #e49436">Studium</span> is about to uproot the insurance
IT landscape by proving that IT is not as problematic
as it is experienced with large vendors.

---

The <span style="color: #666666">insurer</span> defines the <span style="color: #666666">product</span>,
the <span style="color: #666666">system</span> presents it in a consistent
manner to <span style="color: #666666">all channels</span>: in-house, intermediaries, service providers,
clients facing.

Let's look at what we have. <!-- .element: class="fragment" -->

---

#### Product lifecycle management

Implement new products within days

Adjust and release new product versions within clicks

---

A <span style="color: #666666">product definition</span> is a self contained entity.

Once it is done, can be saved into a <span style="color: #666666">text file</span> and <span style="color: #666666">uploaded</span> to the live
environment, where it is usable <span style="color: #666666">instantly</span>.

---

No redeployments!

(...at least not with the out-of-the-box functionality)

---

##### Product = Structure + Business rules

![Product definition declarative](assets/product_def_example.1.png)

---

... fields included, with formats and constraints.

![Product field definitions](assets/product_def_example.2.fields.png)

---
<span style="font-size: 0.6em">
...and business rules. We have an integrated rules engine
that does the heavy lifting.
</span>

![Business rules](assets/business_rules.png)

---

A rule is a simple thing:

![Rule sample](assets/rule_example_exclude_members_80plus.png)

---

The result of all changes can be seen and tested instantly.

Then just upload to production as a new product version.

---

Out of the box client facing UIs

![QQ Health 1](assets/qq_health.1.png)

---

![QQ Health 2](assets/qq_health.2.png)

---

![QQ Health 3](assets/qq_health.3.png)

---

![QQ Health 4](assets/qq_health.4.application.png)

---

![QQ Health 5](assets/qq_health.5.payment.png)

---
#### Technology
Integrated, fully online, works on devices with all screen sizes

---
###### Desktop
![Screen on a desktop](assets/screen_desktop.png)

---

###### Tablet
<img src="assets/screen_tablet.png" alt="Screen on a tablet" style="height: 500px" />

---
###### Phone
<img src="assets/screen_phone.png" alt="Screen on a phone" style="height: 500px" />

---

#### Client accounts support

Once a client buys a policy, an account is created to her and the link
is sent. The client can <span style="color: #666666">self-administer</span> policies / claims from there onwards.

---

#### Intermediary accounts self-management

Intermediaries can sign up with their Google, Facebook, LinkedIn identities,
or just by an email address.

Product access can be granted to them by inhouse staff.

---

Account owners may grant access to other people.

They can <span style="color: #666666">administer</span> their <span style="color: #666666">own workforce</span>!

<img src="assets/account_grants.png" alt="Account grants" />

---

#### Policy management

Endorsements

Cancellations

Renewals

---

#### Accounting

Proper pro-rata calculations out of the box.

The results can be fed to any <span style="color: #666666">general ledger</span> system.

---

#### Promotional campaigns

<img src="assets/promotional_campaigns.png" alt="Promotional campaigns" />

---

#### Coupons

<img src="assets/coupon_management.png" alt="Coupon management" />

---

#### Data output for analytics

We keep actuaries happy.

- all quotes
- client revisits to those, with request parameters
- success indicators
- all policies
- (...later claims data linked to benefits, planned)

---

#### Specialty products

No problem.
Our data model has the flexibility to support them.

In fact, in our reference products, in-house underwriters are already
able to define granular policy setups like some covers only at some risks
at specific date ranges, the system does the required slice-and-dicing.

---

E.g.

![Policy feature assembly](assets/policy_feature_assembly.png)

---

#### Performance

<ul style="font-size: 0.6em">
<li>Tested with 10M randomly generated policies</li>
<li>Generation speed 50 policy / second on a single I7 core (single threaded execution)</li>
<li>this includes applying business rules, validation, rating, persisting data to RDBMS</li>
<li>size on disk is 30G</li>
<li>with 10M policies in RDBMS the system performs with the same responsiveness</li>
</ul>

<img src="assets/policy_search.png" alt="Generated policies" />

---

#### Response times

<span style="font-size: 0.8em">
All tiers on a development desktop, 10M policies on the user's active account:
</span>

<ul style="font-size: 0.8em">
<li>Policy search
    <ul>
    <li>By policy number: 3ms exact, 30ms left substring match</li>
    </ul>
</li>
<li>Partner search
    <ul>
    <li>By name: 400ms +-200, both sides substring match</li>
    <li>By external ID: 10ms +-3 left ~</li>
    <li>By email: 50ms +-40 left ~</li>
    </ul>
</li>
<li>Start / issue endorsement on a policy, display policy, etc: 50ms</li>
</ul>

---

Don't take our word for all this.

#### Give us your product brochure, we come to your office with the products done!