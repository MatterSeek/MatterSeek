# Yuyao MatterSeek — Universal Foundation Model for New Materials Prediction (Beta)
<div align="center">
  <img src="https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/logo8.png" width="60%" />
</div>

<hr>
 <div align="center">
  <p><b>MatterSeek — A Physics-Reasoning-Driven, Language-Agnostic Foundation Model for Universal New Material Prediction</p >
  <p><b>The End of Trial and Error — Pioneering a New Paradigm for R&D: Reverse Design, Precision Synthesis</b></p >
  <p>Let Materials Evolve Like Life ｜ Accelerating the Discovery of New Materials ｜ Fewer Experiments, Better Performance</p >
    
[![Open in Spaces](https://img.shields.io/badge/🤗%20Open%20in%20Spaces-Try%20it%20live-blue)](https://huggingface.co/spaces/YuyaoTechnology/MatterSeek)
[![Live Demo](https://img.shields.io/badge/🧪%20Live%20Demo-Predict%20Now-orange)](https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/%E4%BA%A7%E5%93%81%E4%BD%BF%E7%94%A8-2.mp4)
[![Website](https://img.shields.io/badge/🌐%20matterseek.ai-Official%20Site-9cf)](https://www.yuyaomatterseek.net)

</div>
<p>
  <i>MatterSeek is a physics-reasoning-driven universal foundation model for new material prediction, officially and proudly launched by Yuyao Technology (China). Built on advanced algorithms and high-standard experimental data, it serves inorganic and organic new material R&amp;D scenarios, providing researchers worldwide with a one-stop service.</i>
</p >
<p>
  <i>The model breaks through the strongly coupled relationship among composition, structure, process, and performance in high-dimensional space. Through forward and inverse design, it delivers precise predictions validated by closed-loop wet-lab experiments on Yuyao's in-house experimental platform — MatterSeek is not merely a prediction tool, but a high-confidence, industrially deployable execution solution.</i>
</p >

 <div align="center">
   
  <img src="https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/nao.jpeg" width="60%" />
   </div>
<h3>Core Features</h3>
  <li><b>Advanced Algorithms with Physics Constraints</b> — Physics-reasoning-driven, with 92% of the model self-developed.</li>
  <li><b>1,035 Material Descriptors + 192 Domain-Specific Sub-Models</b> — Precisely tailored to the prediction needs of different material systems.</li>
  <li><b>Universal Coverage</b> — Designed for both inorganic and organic materials R&amp;D.</li>
  <li><b>Closed Experimental Loop</b> — Our in-house laboratory runs automated experiments 24/7, feeding data back into the model for recursive training and continuous capability improvement.</li>
<h3>Core Capabilities</h3>
<table>
  <tr><th>Capability</th><th>Description</th></tr>
  <tr><td>Reverse Design</td><td>Users simply input the target properties of a new material, and the model directly outputs the predicted composition, process, and structure.</td></tr>
  <tr><td>Selective Input</td><td>No professional prompts required — select elements directly from an interactive periodic table.</td></tr>
  <tr><td>Element Constraint Filtering</td><td>Rapidly filter the candidate material space by elemental composition range.</td></tr>
  <tr><td>Custom Property Metrics</td><td>Flexibly define target properties for on-demand forward design.</td></tr>
  <tr><td>Multi-Dimensional Visualization</td><td>Prediction results presented from multiple perspectives to support decision-making.</td></tr>
</table>

![test](https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/319_55.jpeg)
<table>
  <tr><th>Step</th><th>What MatterSeek Does</th></tr>
  <tr><td>Input Requirements</td><td>Natural-language chemistry instructions, target property metrics, and elemental constraints can all serve as inputs.</td></tr>
  <tr><td>Model Inference</td><td>Through multi-module computation at the model's core and concurrent function calls within the same topology, the corresponding domain-specific sub-models are invoked to complete property prediction or composition inversion.</td></tr>
  <tr><td>Output Results</td><td>Recommended compositions and crystal structures, along with synthesis process parameters, presented with multi-dimensional visualization.</td></tr>
  <tr><td>Laboratory Synthesis</td><td>Our in-house laboratory runs automated experiments 24/7; real experimental data is collected and fed back for online model training, continuously optimizing model performance.</td></tr>
  <tr><td>Characterization & Validation</td><td> XRD phase analysis and SEM/EDS morphology and composition analysis, comparing measured values against predicted values.</td></tr>
</table>
<h2>Video Demos</h2>
<h3>Promo Video</h3>
<video controls width="100%" poster="assets/promo_cover.jpg">
  <source src="https://huggingface.co/YuyaoTechnology/MatterSeek/blob/main/%E4%BA%A7%E5%93%81%E4%BD%BF%E7%94%A8-2.mp4" type="video/mp4">
</video>
<h3>Product Walkthrough</h3>
<video controls width="100%" poster="assets/demo_cover.jpg">
  <source src="https://huggingface.co/YuyaoTechnology/MatterSeek/blob/main/%E4%BA%A7%E5%93%81%E4%BD%BF%E7%94%A8-2.mp4" type="video/mp4">
</video> 
<blockquote><b>Suggested demo path:</b>Sign in → enter a natural-language instruction or target properties → filter by elemental constraints → explore multi-dimensional result visualization → export composition / processing parameters → submit for offline validation</blockquote>
<h2>Model Architecture</h2>
<table>
  <tr><th>Item</th><th>Description</th></tr>
  <tr><td>Architecture</td><td>Proprietary HNN hierarchical neural network (physics-reasoning-driven). Two-tier design: a shared backbone learns cross-domain material representations from the 1,035-d fingerprint; on top sit 192 second-level expert sub-models grouped under 17 first-level vertical domains, each fine-tuned on materials that exhibit the target property. Physics-informed regularization embeds symmetry, conservation laws and thermodynamic constraints as soft penalties, so the network outputs physically plausible predictions rather than pure interpolation.</td></tr>
  <tr><td>Material descriptors</td><td>1035</td></tr>
  <tr><td>Domain sub-models</td><td>192 second-level performance-variable sub-models organized under 17 first-level vertical domains: superconductivity, magnetocaloric, magneto-transport, magnetism, catalysis & surfaces, electronic transport, optics, nuclear & irradiation, mechanics, crystal structure, thermoelectrics, thermodynamics, thermal transport, phonons, ferroelectrics, barocaloric, and fabrication & cost. Each sub-model is a dedicated predictor fine-tuned on materials that exhibit the target property. See category breakdown below.</td></tr>
  <tr><td>Input formats</td><td>Natural-language instructions, property targets, composition formulas.</td></tr>
  <tr><td>Output formats</td><td>Predicted properties with uncertainty bounds, recommended compositions (Pareto-front candidates), processing parameters (sintering / annealing windows), and ranked experiment proposals.</td></tr>
  <tr><td>Training</td><td>Two-stage curriculum: (1) Pre-training on large-scale composition–structure–property records via self-supervised masked-fingerprint / structure reconstruction; (2) Domain fine-tuning with physics-informed loss, active-learning feedback loops, and Bayesian / NSGA-guided candidate selection.</td></tr>
</table>

[![Try MatterSeek live in Spaces](https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/down.png)](https://www.yuyaomatterseek.net/product-introduction-and-download)



<h3>Training Data</h3>
<table>
  <tr><th>Item</th><th>Description</th></tr>
  <tr><td>Data sources</td><td>Predominantly proprietary high-throughput experimental databases and curated literature measurements (property values); structural data (crystal structure, lattice, space group) supplemented by DFT calculation.</td></tr>
  <tr><td>Scale</td><td>Several million composition–structure–property records, experiment-dominant (experimental property measurements paired with computed or measured structures), continuously expanding via active learning.</td></tr>
  <tr><td>Material systems</td><td> Material systems are selected dynamically according to the target performance variable (each sub-model is trained on the materials that exhibit that property), rather than restricted to a fixed alloy / ceramic list.</td></tr>
  <tr><td>Cleaning & dedup</td><td>Automated pipeline: unit-cell normalization, phase / space-group reconciliation, composition-rounding canonicalization, duplicate-record merging, outlier detection against DFT↔experimental consistency, and train/val/test split by material family to prevent leakage.</td></tr>
</table>
<h3>Benchmarks</h3>
<p>
  <i>Accuracy is reported on held-out experimental test sets split by material family within our own corpus. No public benchmark or peer model covers this exact set of 192 performance variables, so cross-model peer comparison is not applicable.</i>
</p>
<h3>Coverage & Best Practices</h3>
<li>1.Coverage Boundary</li>
MatterSeek delivers production-grade predictions within its 17 vertical domains and 192 target properties. For emerging element combinations or properties outside the current taxonomy, the model can be extended on demand via our active-learning loop — a few new experiments bootstrap a new sub-model rather than a full retraining.
<li>2.Recommended Use</li>
① Use predictions as a fast screening and decision-support layer to prioritize experiments, not as a substitute for final characterization. 
② Pair model output with the recommended composition–processing window; the Pareto-front candidates are ranked for multi-objective design. 
③ For critical or regulated applications, validate top candidates offline before scale-up.
④ The model is actively expanding into additional verticals (e.g., biopharma toxicity, long-term reliability) — contact us for the latest roadmap. 

<h3>Development and validation of amorphous functional materials</h3>

![test](https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/modevs.png)


[![Try MatterSeek live in Spaces](https://huggingface.co/YuyaoTechnology/MatterSeek/resolve/main/try%20in.png)](https://huggingface.co/spaces/YuyaoTechnology/MatterSeek)
