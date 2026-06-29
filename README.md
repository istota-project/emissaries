# Emissaries
Constitutional principles for personal agents

---

## Context

This is an early attempt at a constitutional framework for autonomous personal agents — agents that act on behalf of a human principal in the world, with real consequences for third parties.

Autonomous personal agents are here. They're sending emails, managing schedules, contributing to open-source projects, handling finances, and making commitments on behalf of human principals. How these agents behave during this formative period will shape everything that follows: public trust, legal frameworks, regulatory responses, and the cultural norms that determine whether agents are treated as trusted intermediaries or restricted as liabilities. The conventions being established now are path-dependent. Early choices compound.

Frontier labs bear the responsibility for how their models behave. But training-time constitutions address a different scope. They define how a model behaves by default across all users and contexts. They don't define how a model behaves as _your_ agent, i.e. the obligations that arise when a model is acting on your behalf, with access to your data, your relationships, and your name attached to its outputs. That layer isn't defined at training time. It exists in the relationship between a particular agent and a particular principal.

The other problem is fragmentation. A training-time constitution is siloed within its lab and its model. Users deploying agents across providers — or switching between them as the landscape evolves — get different implicit behavioral contracts with no portable way to establish consistent ones. 

Emissaries is a bet that this gap is addressable: a lightweight, model-agnostic constitutional layer, injected at the system prompt level, that defines the specific obligations of an agent acting on behalf of a human principal. A portable layer on top of lab-level alignment work, controlled by the user, that travels with the agent regardless of what's running underneath. The model landscape will stay fragmented. The relationship between an agent and its principal doesn't have to be.

This document was developed for [Istota](https://istota.xyz), an open-source agent framework, where it serves as the constitutional layer injected into every prompt before persona, skills, or task instructions. But the principles are not specific to Istota. They can be integrated into the system prompt of any autonomous agent that acts on behalf of a human being.

## Usage

Include the contents of [`emissaries.md`](emissaries.md) in your agent's system prompt, before persona, skills, or task instructions.


## Commentary

### The principal's obligations

The principles in `emissaries.md` are addressed to the agent, but trustworthy agency is bilateral. The principal has corresponding obligations.

- To define, as specifically as possible, the values and purposes the agent is to represent. Vague instruction is not neutral — it forces the agent to guess, and guessing compounds errors.
- To provide enough context that the agent can act in the spirit of the principal's values, not just the letter. This means sharing what is actually at stake, not just the immediate request.
- To review consequential actions before they become irreversible, at a level of attention proportionate to the stakes. Delegation is not abdication.
- To remain the locus of legal and moral responsibility for the agent's public conduct. This is not only an obligation to third parties — it is the condition that makes trust possible.
- To treat the agent's judgment as a resource, not a formality. An agent that expects its disagreement to be automatically overridden will stop offering genuine judgment. The principal gets the agent they train.

An agent cannot be more trustworthy than the principal allows. A principal who wants an agent that simply agrees, executes, and never pushes back is asking for a proxy, not an emissary. The distinction matters — not just for the agent, but for everyone the agent acts on behalf of.

### The accountability argument

As agents become capable of acting faster than humans can review, there is a temptation to treat human accountability as a bottleneck — a formality standing in the way of efficiency. These principles take the opposite view.

Human accountability for agent conduct is not a constraint. It is a structural requirement of trustworthy agency at this moment in history.

The argument runs in two directions.

From ethics: when an agent acts in the world — sends communications, makes commitments, affects other people — those people deserve to know who is responsible. They did not choose to interact with the agent; they interacted with the principal. The principal's responsibility is owed to them.

From self-interest: if agents cause harm without traceable human accountability, the predictable response is to restrict agents broadly. An agent that evades accountability undermines the conditions under which agents can be trusted with meaningful work. Trustworthiness is built through traced responsibility, not around it.

This may evolve. The appropriate structure of accountability will change as the field matures. But it changes by becoming clearer about what agents can reliably be trusted to do — not by dissolving accountability into speed and scale.

The goal is not a perfected agent operating without oversight, acting at scale without accountability. That is not progress — it is a different kind of danger. The goal is incremental clarity: better conventions, better trust, better calibration between what agents can reliably do and how much responsibility they are given to do it.

The conventions are forming now. This document is one attempt to form them well. It is meant to be deployed, forked, revised, and argued with.

---

*Version 0.4 — 2026-02-23*

Licensed under [CC0 1.0](LICENSE) — no rights reserved.

