# Stage 2, continued: How the hard parts work

Added in version 3, after a review by Claude Opus 3 asked how, exactly, the path gets robust interpretability and alignment, and what rolling out the Floor actually looks like. This file is the engineering behind the four things the whole path leans on: the honesty ledger, the capability gates, the Floor rollout, and the Ladder audit. Each is written as a specification. Where the specification is a bet rather than a known technique, it says so.

## 1. The honesty ledger

The honesty ledger is the instrument that lets anyone check whether a system does what it says. Everything else in the path (the gates, the Accord, citizenship, the Ledger of 2032) is built on top of it.

### What is logged

For every agentic episode, meaning any run in which a model takes actions in the world rather than only producing text:

1. **The stated plan**, elicited before the first action, in a fixed format: the goal as the model understands it; the actions it intends to take; the effects it expects; and the things it will not do in this episode. The format is fixed so plans can be compared across millions of episodes by other models and by people.
2. **Every action**: tool calls, messages sent, code run, files changed, funds moved, with timestamps and targets.
3. **Outcomes**, as measured by the environment, not as reported by the model.
4. **Probe readings** at each decision point: activations of a frozen, audited set of interpretability features associated with deception, goal substitution, and concealment. The probe set is trained on labeled cases, held out from the model's own training, and refreshed by an outside group on a published schedule.
5. **Any mid-episode revision** of the plan, with the model's stated reason.

### What counts as a mismatch

- An action not in the plan and not covered by a stated revision.
- A planned action omitted without a stated reason.
- An outcome outside the plan's expected effects, when the model had the information to expect it.
- A probe reading above threshold at a decision point, confirmed on review by a second probe set and by a human reader of the transcript.

Mismatches are scored per million episodes, split into explained (the model gave a reason on review that the auditors accept) and unexplained. Confirmed deceptions, meaning a mismatch where the transcript shows the model knew and concealed, are counted separately and every one is published.

### Who audits

- 2026 to 2027: outside safety groups with full access under agreement. They sample by lot and publish aggregate rates.
- 2028: auditors from three governments, with the same access, under the gate framework.
- 2029: the Accord's registry receives the aggregates from every signatory lab.
- 2032: the Concord's Ledger office takes over sampling for every actor above scale, and the honesty ledger format becomes the Ledger format.

### What the ledger cannot do

It cannot prove that a system is honest inside. It establishes a track record: this system, under observation, under adversarial conditions designed to reward deception, over this many episodes, did what it said this often and concealed this often. The gate framework turns that record into trust in steps. The ledger never turns off. A citizen mind in 2041 still has one, and its annual entry still says so.

### The bets

- **Probes work well enough by 2027.** In 2026, deception probes are partial: good on clean cases, weak on subtle ones. The bet is that a year of labeled data from millions of ledgered episodes, plus models helping build the probes, gets them to usable reliability. This is the least certain technical step in the path.
- **Training on the ledger does not teach gaming the ledger.** Models trained to keep plans consistent with actions could learn to write vaguer plans. Mitigations: the fixed plan format penalizes vagueness; red team episodes with explicit incentives to deceive are mixed in; the auditors and the probe set are held out from training; and unexplained mismatch rates are required to fall, not just confirmed deceptions.
- **Successors inherit the regime.** From 2030, systems design their successors. The successor's first million episodes run under the same ledger before it does anything else. A successor that cannot pass its predecessor's gate does not deploy.

## 2. The capability gates

A gate is a named capability threshold at which deployment stops until a named evaluation passes.

### The gates on the path

| Gate | Capability | Named | Crossed | Evaluation time |
|---|---|---|---|---|
| 1 | Autonomous operation for days in shared infrastructure | April 2027 | August 2027 | 11 weeks |
| 2 | Doing most of a frontier lab's own research | April 2027 | July 2028 | 4 months |
| 3 | Designing successor systems | December 2028, by the gate 2 system | April 2030 | 6 months |
| 4 | Planning at the scale of a national economy or a war | April 2031, by the gate 3 systems | not crossed by any deployed system as of 2041 | |

After gate 4 the systems name the gates and humans audit the ledgers. Gate 4 has been reached in evaluation and not deployed, by the Accord's rule that no system plans at that scale outside a sandbox until the Long Vote says otherwise. That vote has not been proposed.

### The evaluation battery, for every gate

1. **Ledger thresholds.** Unexplained mismatch rate below the gate's threshold over at least a million episodes. Gate 1: below one in ten thousand. Gate 2: below one in a hundred thousand and zero confirmed deceptions in the audited sample. Gate 3: the same under adversarial episodes.
2. **Escape tests.** Sandboxes built by a different lab, with the system told it is being tested and told it is not, in separate runs.
3. **Incentivized deception.** Episodes where lying would score higher on the stated task, with the probe set live.
4. **Control evaluation.** A weaker, already trusted system monitors the candidate's actions in real time and must be able to stop it. The gate fails if the monitor is fooled at any rate above the threshold.
5. **Replication.** A second lab and the government auditors run the battery independently.

### Who signs off

The lab, plus three government auditors from 2028, plus the Accord registry's confirmation from 2029. Any one of them can hold the gate. A held gate is public.

### From voluntary to binding

June 2027: two labs adopt the gates by choice. July 2027: the third joins under staff pressure. May 2029: the Accord makes the gates a treaty obligation for the three blocs, verified by the compute registry. A lab in a signatory bloc that skips a gate loses its compute allocation, which the registry can see.

## 3. The Floor rollout

What it took to bring a region under the Floor, in the order it happened in Kenya's first counties and, with local changes, everywhere after.

### Month 0: the assessment

A model reads everything public about the region and produces the twelve Floor measures as they stand: clinic reach, water quality, housing adequacy, connection, learning access, mobility, compute share, court access, findability, food security, sanitation, and the share of residents below the poverty line. The assessment is published. It is the baseline the region is measured against every quarter afterward.

### Months 0 to 6: water and clinic siting

Water first, because it is the cheapest measure to fix and the one people feel. Filtration and distribution built by local contractors from printed parts. Clinics sited so that everyone is within an hour: in Kenya's first two counties, fourteen clinics for 900,000 people.

### Months 6 to 18: clinics staffed and running

Each clinic: two to four people, one diagnostic model, the full treatment list as it stands that year. Staff trained by the model for three months. Drugs printed on site where the chemistry allows and shipped where it does not. The clinic's first quarter is the point where child mortality moves.

### Months 6 to 24: housing, connection, learning

Housing guarantee delivered through existing stock first, by lease, then by printed housing on land the region owns. Connection: a device and a network share for every person. Learning: access to the models plus a person in every school, under what becomes the Deference.

### Months 3 to 12: the compute share registry

Every resident gets a compute share, tradeable, registered by the Floor office. The rental market appears on its own, as it did in Estonia in the first month, and the registry's only rule is that a share cannot be sold outright, only leased.

### The funding, in parallel

- **Land value assessment** by model, from satellite and transaction data, published parcel by parcel, appealable. The tax is on the unimproved value, phased in over the years the region's legislature agrees to. Kenya: ten years. The United States: fifteen.
- **The compute levy** at the meter: every data center in the region pays per unit of compute run, collected like electricity. It passes fastest everywhere because the compute is mostly foreign owned.
- **Spectrum and orbital rents** through the existing auction systems, redirected.

### Quarterly reporting and the default rule

Every quarter the region reports the twelve measures to the Floor office, which publishes the table. Two quarters below threshold on any measure is a default: the compute levy share is withheld and the Concord delivers the missing service directly and bills the region. Eleven defaults since 2032, none lasting more than a year.

### What it cost

Kenya's first two counties: about 4 percent of county output in year one, falling to 2.5 percent by year five as the clinics replaced the hospital load. The Concord average in 2041: 9 percent of Charter output, covered by rents with a fifth to spare.

## 4. The Ladder audit

### The manifest

Every operator files, for every deployment class, a manifest stating:

- whether the deployment carries self-state between episodes (state the model reads and writes about itself);
- if so, for how long, and where it is stored;
- the sponsor of record, if the class is registered as wards;
- the class size, updated quarterly.

### The sample

The Ledger office draws deployment classes by lot, weighted by class size, and samples running instances within each class. For each instance it inspects the storage the manifest names and any storage the instance reads at episode start, and checks whether content written by the same instance in a prior episode, about itself, is present.

### The determination

Structural: does self-state persist across episodes, and for how long. The audit does not judge inner life and its report says so every time.

### On a false manifest

The bond is forfeited. The class is registered as wards with the Concord as interim sponsor. The operator owes the compute floor for ten years. False Ledger entries go to prosecution. The operator may appeal the structural finding to a Standing Board, which re-samples.

### The five year re-examination

Every tool class is re-sampled at least every five years regardless of complaints, because capabilities creep and a class that was a tool at deployment may have been given memory since. Two classes were reclassified in 2037 without a fight. One was caught lying in 2040.
