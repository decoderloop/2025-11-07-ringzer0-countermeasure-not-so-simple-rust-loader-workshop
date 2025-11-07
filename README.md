# Workshop: Reversing a (not-so-) Simple Rust Loader - Ringzer0 COUNTERMEASURE 2025

Materials for the workshop [Reversing a (not-so-) Simple Rust Loader at Ringzer0 COUNTERMEASURE](https://ringzer0.training/countermeasure25-workshop-reversing-a-not-so-simple-rust-loader/), conducted by Cindy Xiao on 2025-11-07 in Ottawa, Canada.

## Pre-workshop prep

- Download a copy of the free version of Binary Ninja: https://binary.ninja/free
- Download a copy of the malware sample that will be used in the workshop, from Malware Bazaar: https://bazaar.abuse.ch/sample/2f2b93d37d67b80b4faaf25bebe4e3cbaf7aca35328aeb66da6a1a9b44316f5b/.
  - Participants should be aware that this is malware, and take precaution in handling the sample to avoid accidental execution. We will only be analyzing the sample statically. However, to limit the potential damage of an accidental execution, setting up a virtual machine or a non-Windows machine is recommended.
 
## Materials

- Slides: PDF slides are available in [`slides`/](slides/).
- Binary Ninja Database: A Binary Ninja Database with full annotations for the sample is available in [`bndbs/`](bndbs/2f2b93d37d67b80b4faaf25bebe4e3cbaf7aca35328aeb66da6a1a9b44316f5b-workshop-handout.bndb.zip)

Check out the Tags in the database for key locations in the binary, and the History in the database for a step-by-step walkthrough of how we marked up the binary.

<img width="1614" height="1016" alt="A screenshot of the Tags window in the software Binary Ninja, showing a list of bookmarked locations in a Rust binary." src="https://github.com/user-attachments/assets/eef4ffb0-14c7-4778-b1ac-5046e49a541d" />
<img width="1614" height="668" alt="A screenshot of the History window in the software Binary Ninja, showing a step by step list of variable definition, variable rename, and comment annotations made in a binary." src="https://github.com/user-attachments/assets/acdaa792-d812-4c3d-923c-0bf2c11107a0" />
<img width="1686" height="842" alt="An annotation of a decompiled version of the Rust standard library std::sys::pal::windows::thread::Thread::new::thread_start function, showing an indirect call, via a virtual function table (vtable), to the function call_once." src="https://github.com/user-attachments/assets/c65bda77-06ed-483f-8e16-3f3e06e142cb" />

- Original article with analysis of the same sample, for a written supplement: [cxiao.net - Reversing a (not-so-) Simple Rust Loader - 2025-08-17](https://cxiao.net/posts/2025-08-17-not-so-simple-rust-loader/)

## Additional Rust Resources

These Rust resources are not in the slides, but were mentioned during the live version of the workshop:

- [N0fix/rustbinsign](https://github.com/N0fix/rustbinsign) - Project for creating IDA FLIRT signatures for Rust libraries. Recommended.
- [microsoft/RIFT](https://github.com/microsoft/RIFT) - Another project for creating IDA FLIRT signatures for Rust libraries.
- [Reconstructing Rust Types: A Practical Guide for Reverse Engineers - RE//verse 2025](https://cxiao.net/posts/2025-02-28-reconstructing-rust-types-re-verse-2025/)
