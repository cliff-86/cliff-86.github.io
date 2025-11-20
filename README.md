# Media Directors & Audit Fees  
_Project Overview, Structure, and Findings_

This project investigates whether the presence of media-linked directors influences firms' audit fees, audit effort, and accounting quality. The core idea is that media expertise on the board may change auditors’ perceptions of firm transparency, governance quality, and reputational risk.

---

## 1. Research Questions

### Core Question
- Do firms with media-linked directors pay different audit fees?

### Mechanism / Channel Questions
- Does media expertise strengthen governance and transparency (→ lower audit fees)?  
- Or does higher public visibility raise litigation/regulatory risk (→ higher audit fees)?

### Additional Outcome Questions
- Does the presence of media directors improve accounting quality?  
- Does it reduce internal control weaknesses?  
- Does it affect audit report lag or audit effort?

---

## 2. Conceptual Framework

### Media Director Definition
Media directors are board members with:
- journalism or broadcasting careers,  
- senior positions in media corporations,  
- public-facing roles or high visibility,  
- extensive communication or public-relations experience.

### Two Competing Hypotheses

#### **H1: Governance & Transparency Channel**
Media skills → better communication & oversight → reduced information risk  
→ auditors require **lower fees**

#### **H2: Visibility & Reputational Risk Channel**
Media presence → higher public attention → increased litigation risk  
→ auditors charge **higher fees**

The project empirically identifies which channel dominates.

---

## 3. Data Structure

### Data Sources
- BoardEx director biographies  
- Audit fees from Audit Analytics or Compustat  
- Financial statement data from Compustat  
- CUSIP/GVKEY linking files for merging  

### Core Variables
- `media_dir` – indicator for presence of media-linked director  
- `ln_auditfees` – natural log of audit fees  
- `big4` – auditor type  
- Firm controls – size, leverage, ROA, segments, foreign operations  
- Governance controls – board size, independence, female directors, institutional ownership  

### Governance Composite (Optional)
- PCA1 index constructed from governance variables (board gender diversity, transient institutional ownership, firm efficiency)

---

## 4. Empirical Strategy

### Baseline Specification

### Identification Approaches
- Firm fixed effects  
- Year fixed effects  
- Industry × year fixed effects  
- Alternative media director definitions  
- PSM matching (media vs. non-media director firms)  
- Appointment-based future event design (extension)

### Robustness Checks
- Audit vs. non-audit fee decomposition  
- Alternative visibility measures  
- Removing media-industry firms  
- Subsample analysis by governance strength  
- Using PCA1 as moderation channel  

---

## 5. **Key Empirical Findings**

### ✔ **1. Media-linked directors are associated with *lower* audit fees.**  
Audit fees decline by a statistically meaningful amount after controlling for firm characteristics and fixed effects.

This supports the **governance transparency channel**, not the visibility-risk channel.

### ✔ **2. The fee reduction is stronger where baseline firm governance is weaker.**  
- Firms with weaker governance exhibit **larger decreases** in audit fees.  
- This implies media directors **substitute for weak existing oversight**.

### ✔ **3. Media directors are linked to improvements in governance-related variables.**  
Empirically observed patterns include:  
- reductions in transient institutional ownership (lower short-term pressure),  
- increases in independent female directors,  
- improved managerial ability/efficiency measures.

These improvements align with the mechanism that media directors enhance monitoring or communication quality.

### ✔ **4. No evidence that auditors perceive higher litigation risk.**  
The data do **not** show increases in audit fees, audit effort, or risk-related audit variables.  
This rejects the visibility-risk hypothesis in this setting.

### ✔ **5. Governance mediation (PCA1) is consistent with the main mechanism.**  
When using PCA1 (the composite governance factor) as a mediator:  
- Better governance partially explains lower audit fees.  
- Suggests a **governance substitution effect**.

### ✔ **6. Accounting quality outcomes (preliminary).**  
Early tests show:  
- no significant deterioration in accrual quality,  
- some evidence of reduced internal control weaknesses in firms with media directors.

These patterns are directionally consistent with improved governance.

---

## 6. Extensions

### Accounting Quality
- discretionary accruals  
- restatements  
- internal control weaknesses  
- earnings management behavior  

### Auditor Behavior
- audit report lag  
- auditor switching  
- engagement-level effort (if audit-hour data are available)

### Market Perception
- event study around new media-director appointments  
- changes in analyst coverage or press tone  

---

## 7. Project Folder Structure

---

## 8. Summary Contribution

This project contributes to the literature by demonstrating that:

- Media-linked directors represent a **novel governance characteristic**.  
- Their presence is associated with **lower audit fees**, consistent with improved transparency and monitoring.  
- The effect is stronger in firms with weaker governance, implying a **governance substitution role**.  
- Auditors do not price higher visibility risk in this context.  
- Governance improvements (as captured through individual metrics and PCA1) help explain the observed audit fee reduction.


