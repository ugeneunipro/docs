---
title: "Align Profile to Profile with MUSCLE Element"
weight: 100
---

# Align Profile to Profile with MUSCLE Element

Aligns the second profile to the master profile using the MUSCLE aligner.

**Type:** align-profile-to-profile

## Input/Output Ports

The element has 1 _input port_:

**Name in GUI:** in-profiles  
**Name in Workflow File:** in-profiles  
**Slots:**

| Slot In GUI        | Slot in Workflow File | Type         |
|--------------------|-----------------------|--------------|
| **Master profile** | master-msa            | _malignment_ |
| **Second profile** | second-msa            | _malignment_ |

And 1 _output port_:

**Name in GUI:** out-msa  
**Name in Workflow File:** out-msa  
**Slots:**

| Slot In GUI | Slot in Workflow File | Type         |
|-------------|-----------------------|--------------|
| **MSA**     | msa                   | _malignment_ |
