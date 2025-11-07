# Workshop: Reversing a (not-so-) Simple Rust Loader - Ringzer0 COUNTERMEASURE 2025

Materials for the workshop ["Reversing a (not-so-) Simple Rust Loader" at Ringzer0 COUNTERMEASURE](https://ringzer0.training/countermeasure25-workshop-reversing-a-not-so-simple-rust-loader/), conducted by Cindy Xiao on 2025-11-07 in Ottawa, Canada.

## Pre-workshop prep

- Download a copy of the free version of Binary Ninja: https://binary.ninja/free
- Download a copy of the malware sample that will be used in the workshop, from Malware Bazaar: https://bazaar.abuse.ch/sample/2f2b93d37d67b80b4faaf25bebe4e3cbaf7aca35328aeb66da6a1a9b44316f5b/.
  - Participants should be aware that this is malware, and take precaution in handling the sample to avoid accidental execution. We will only be analyzing the sample statically. However, to limit the potential damage of an accidental execution, setting up a virtual machine or a non-Windows machine is recommended.
 
## Materials

- Slides: PDF slides are available in [`slides`/](slides/).
- Binary Ninja Database: A Binary Ninja Database with full annotations for the sample is available in [`bndbs/`](bndbs/2f2b93d37d67b80b4faaf25bebe4e3cbaf7aca35328aeb66da6a1a9b44316f5b-workshop-handout.bndb.zip)
- Original article with analysis of the same sample, for a written supplement: [cxiao.net - Reversing a (not-so-) Simple Rust Loader - 2025-08-17](https://cxiao.net/posts/2025-08-17-not-so-simple-rust-loader/)
