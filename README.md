# Exploring Genome Mining for Natural Product Discovery

**Aishat Faderera Akere**  
Botany Graduate | Natural Products Enthusiast  
akereaishat8@gmail.com | www.linkedin.com/in/aishaakere

---

## Why I'm Learning This

I've always been fascinated by how plants and their microbial partners produce bioactive compounds. During my thesis on endophytic fungi from *Mitracarpus scaber*, I kept wondering: **what other compounds might these organisms be capable of making that we're missing with traditional isolation methods?**

That question led me here—to genome mining and computational predictions. I wanted to see if I could "peek" into a microbe's genetic potential before spending months in the lab trying to coax it into producing compounds.

This repository is my learning journal as I figure out how to bridge my wet-lab natural products background with computational tools.

---

## What I'm Learning

I'm working through the Galaxy Training Network's secondary metabolite discovery tutorial, which covers:

### **Getting Genomes & Quality Control**
- Finding and downloading bacterial genomes from NCBI
- Using FastQC to check sequencing quality
- Understanding what makes "good" sequence data

### **Finding Biosynthetic Gene Clusters (BGCs)**
- Using antiSMASH to predict what compounds a microbe *might* produce
- Understanding different BGC types: PKS (polyketides), NRPS (peptides), terpenes, etc.
- Reading antiSMASH outputs—honestly, this took a while to make sense of!
- Comparing predictions against known BGCs in MIBiG database

### **Scripting & Automation**
- Using Jupyter notebooks within Galaxy to process data
- Writing small Python scripts to connect different tools
- Building workflows so I can reuse the pipeline

### **Cheminformatics (The Chemistry Part)**
- Converting predicted structures into formats for chemical analysis
- Molecular fingerprinting—basically creating "signatures" for each compound
- Comparing predicted molecules to known natural products
- Checking if predictions look like drug-like molecules (Lipinski's rules, etc.)
- Assessing novelty—are these predictions actually new?

---

## My Background

I just finished my BSc in Botany at Bayero University, Kano. My thesis focused on isolating endophytic fungi from a medicinal plant and testing their antifungal activity against *Candida albicans*. I found some really promising isolates, but the big question was: **what compounds are they actually making?**

Traditional natural product isolation is:
- Time-consuming (months of extraction, fractionation, purification)
- Resource-intensive (lots of solvents, chromatography)
- Sometimes you end up rediscovering known compounds
- You only find what the organism produces under your specific culture conditions

**Genome mining flips this around**: look at the genetic blueprint first, predict what's possible, then target your wet-lab work accordingly. It's not replacing traditional methods—it's making them smarter.

---

## Tools I'm Using

- **Galaxy Platform** (usegalaxy.eu) - web-based workflow builder
- **antiSMASH** - the main BGC prediction tool
- **FastQC** - sequence quality checking
- **Various cheminformatics tools** - for molecular analysis
- **JupyTool/Jupyter** - for custom Python scripts

Everything runs in a web browser. No need to install complex software or have a powerful computer—just need internet access.

---

## What's in This Repository

I'm organizing my learning materials here:

**`/workflows`** - Galaxy workflow files I've built  
**`/documentation`** - My notes, things I've learned, problems I've solved  
**`/examples`** - Sample outputs from my practice runs  
**`/analysis-reports`** - When I apply this to real genomes (upcoming)

---

## Progress So Far

### ✅ Completed: Basic Workflow
- Can now download a genome, run it through antiSMASH, and interpret the results
- Understand what different BGC types mean biologically
- Can assess whether a prediction is novel or already known

### ✅ Completed: Cheminformatics Integration  
- Learned how to evaluate drug-likeness of predicted compounds
- Can compare predictions against databases of known molecules
- Understanding novelty scoring

### 🔄 Currently Working On
- Analyzing genomes of endophytic bacteria from medicinal plants
- Seeing if BGC predictions correlate with reported bioactivities in literature
- Building a collection of interesting strains for potential future work

### 🎯 Next Up
- Compare BGC diversity across different plant-microbe associations
- Try to connect computational predictions with my wet-lab experience
- Maybe look at genomes from some of my thesis isolates if sequencing becomes accessible

---

## Why This Matters (To Me)

**Short answer**: I want to find new antimicrobial drugs, and I think computational approaches can help us look in smarter places.

**Longer answer**: 

Traditional medicine in Nigeria (and across Africa) has used plants like *M. scaber* for centuries. Modern science is showing that many of these effects come from plant-associated microbes, not just the plants themselves. But we've barely scratched the surface of microbial chemical diversity.

There are thousands of bacterial and fungal genomes now publicly available. Many are from understudied environments—tropical soils, medicinal plants, extreme habitats. Genome mining lets us:

1. **Prioritize** which organisms to study in the lab
2. **Predict** what kinds of chemistry to expect
3. **Avoid** rediscovering the same compounds repeatedly
4. **Connect** genomic potential with observed bioactivity

I'm not trying to become a pure computational person—I love being at the bench. But having these computational skills means I can ask better questions and design more targeted experiments.

---

## Learning Resources I'm Using

**Main Tutorial:**  
[Galaxy Training Network - Secondary Metabolite Discovery](https://training.galaxyproject.org/training-material/topics/genome-annotation/tutorials/secondary-metabolites/tutorial.html)

**Essential Reading:**
- antiSMASH documentation (for when I get confused about outputs)
- MIBiG database papers (understanding validated BGCs)
- Papers from labs that combine genome mining with experimental validation

**Databases I Check Regularly:**
- NCBI Genome Database
- MIBiG (Minimum Information about BGCs)
- PubChem / ChEMBL for chemical structures

---

## Challenges I've Faced

**Understanding antiSMASH output** was overwhelming at first. So many predictions, domains, modules... I learned to start with the "Known Clusters" section and work from there.

**Interpreting novelty scores** took practice. Just because something is "novel" computationally doesn't mean it's automatically interesting biologically.

**Cheminformatics was completely new** to me as a botanist. Understanding molecular fingerprints and similarity metrics required going back to basic chemistry concepts.

**Workflow troubleshooting** in Galaxy—sometimes steps fail for cryptic reasons. Learning to check file formats and tool parameters carefully.

---

## Connecting to Real Research

Here's how I'm thinking about applying this:

### For My Thesis Isolates
If I can get them sequenced someday:
- Predict which BGCs might be responsible for the antifungal activity I observed
- See if there are other BGCs that weren't expressed under my culture conditions
- Guide targeted fermentation to activate specific clusters

### For Future Projects
- Screen public genomes of endophytes from African medicinal plants
- Look for underexplored BGC families in tropical microbial communities
- Combine predictions with metabolomics to validate computational approaches

### Understanding Natural Products Biosynthesis
Even just as a learning tool, seeing how PKS and NRPS modules are organized helps me understand HOW microbes make these complex molecules. It's bridging genetics with chemistry in a way I hadn't appreciated before.

---

## Some Interesting Things I've Noticed

- **Streptomyces** genomes are PACKED with BGCs—20-30+ clusters per genome!
- Many predicted compounds don't match anything in databases—huge unexplored chemical space
- The same BGC can produce different compounds depending on substrate availability
- Some BGCs are conserved across species, others are super unique
- Plant-associated microbes sometimes have different BGC profiles than soil ones

---

## Open Questions I'm Thinking About

- How much does the plant host influence which BGCs endophytes carry?
- Can we predict bioactivity from BGC structure computationally?
- What percentage of predicted BGCs are actually expressed?
- How do you validate computational predictions efficiently in the lab?
- Are there patterns in BGCs from traditional medicinal plant microbiomes?

---

## What I've Published

My thesis work just came out:  
**Akere, A.F., Galalain, A.M.** (2025). Bioprospecting of Endophytes in Medicinal Plants for Antifungal Properties Against *Candida albicans*: Case study of *Mitracarpus scaber*. *World News Natural Sciences*, 63(2), 193-204.

This computational training is helping me think about the next phase of that research.

---

## Collaboration & Discussion

I'm always happy to chat with other students or researchers interested in:
- Natural products from African biodiversity
- Endophyte biology and chemistry
- Computational approaches to drug discovery
- Bridging traditional medicine with modern science

Feel free to reach out: akereaishat8@gmail.com | www.linkedin.com/in/aishaakere

---

## Acknowledgments

- **Galaxy Training Network** for making high-quality bioinformatics training freely accessible
- **antiSMASH team** for an incredible tool
- **Dr. Aisha Muhammade Galalain** who encouraged me to expand beyond wet-lab skills
- **Open science community** for sharing data, tools, and knowledge
- **My fellow BOSAN members** who tolerated me talking endlessly about BGCs

---

## A Note on This Repository

This is a learning project, not a polished research product. I'm documenting as I go—mistakes, confusions, and all. If you're also learning genome mining, maybe these notes will help you avoid some of the confusion I experienced.

If you're an experienced computational person and see something I've misunderstood, I'd genuinely appreciate the feedback.

---

**Last Updated**: November 2025  
**Status**: Active learning project

---

*"The best time to learn bioinformatics was five years ago. The second best time is now."*  
*— Something I tell myself when I get frustrated with workflow errors*                                                                                                                       
