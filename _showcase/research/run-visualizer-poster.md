---
show: true
width: 12
date: 2026-06-15 00:00:00 +0800
group: Research
---

<div class="p-4">

  <!-- Header -->
  <div class="mb-3">
    <span class="badge badge-pill badge-publication badge-primary">ICPC 2026</span>
    <span class="badge badge-pill badge-publication badge-secondary">Conference</span>
    <span class="badge badge-pill badge-light border text-muted ml-1"><i class="fas fa-map-marker-alt mr-1"></i>Rio de Janeiro, Brazil</span>
  </div>
  <h4 class="font-weight-bold mb-1">Understanding CI/CD Workflow Runs Through Interactive and Animated Visualizations</h4>
  <hr />

  <!-- Body: 3 columns -->
  <div class="row">

    <!-- Col 1: Motivation -->
    <div class="col-md-4 mb-3">
      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-exclamation-circle mr-1"></i>Motivation
      </h6>
      <ul class="small pl-3 mb-2" style="line-height: 1.6;">
        <li>Workflow runs involve multiple interdependent execution units whose relationships are not immediately visible.</li>
        <li>Current tools provide fragmented and predominantly textual representations, limiting pattern detection.</li>
        <li>Diagnosing failures and assessing resource usage across run histories remains challenging.</li>
      </ul>
    </div>

    <!-- Col 2: Approach -->
    <div class="col-md-5 mb-3">
      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-cogs mr-1"></i>Approach
      </h6>
      <div class="small" style="line-height: 1.6;">
        <ol class="pl-3 mb-2">
          <li><strong>Data Extraction</strong> — Mining structured and unstructured run data from GitHub REST API.</li>
          <li><strong>Domain Model</strong> — A Workflow Run Domain Model capturing execution and contextual entities.</li>
          <li><strong>Visualization</strong> — Interactive and animated views at multiple granularity levels.</li>
        </ol>
        <div class="mt-2 p-2 rounded" style="background-color: #f8f9fa;">
          <span class="small font-weight-bold"><i class="fas fa-tools mr-1"></i>Tool:</span>
          <span class="small"><em>Run-Visualizer</em> — built on <a href="https://gtoolkit.com/" target="_blank">Glamorous Toolkit</a></span>
        </div>
        <div class="mt-2">
          <span class="small font-weight-bold">Views:</span>
          <span class="badge badge-light border small">Polymetric Runs</span>
          <span class="badge badge-light border small">Polymetric Actors</span>
          <span class="badge badge-light border small">Run Anatomy</span>
          <span class="badge badge-light border small">Failure Context</span>
        </div>
      </div>
    </div>

    <!-- Col 3: Authors & Links -->
    <div class="col-md-3 mb-3">
      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-users mr-1"></i>Authors
      </h6>
      <div class="small mb-3" style="line-height: 1.8;">
        <div><strong>Pablo Valenzuela-Toledo</strong></div>
        <div class="text-muted" style="font-size: 0.8em;">University of Bern · Universidad de La Frontera</div>
        <div class="mt-1"><strong>Timo Kehrer</strong></div>
        <div class="text-muted" style="font-size: 0.8em;">University of Bern</div>
        <div class="mt-1"><strong>Sebastiano Panichella</strong></div>
        <div class="text-muted" style="font-size: 0.8em;">University of Bern · AI4I</div>
      </div>

      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-link mr-1"></i>Links
      </h6>
      <div class="small">
        <a href="/assets/pdfs/Understanding-CICD-Workflow-Runs-Interactive-Animated-Visualizations.pdf" target="_blank" class="btn btn-sm btn-outline-primary mr-1 mb-1">
          <i class="fas fa-file-pdf mr-1"></i>Paper
        </a>
        <a href="https://doi.org/10.5281/zenodo.17635512" target="_blank" class="btn btn-sm btn-outline-secondary mr-1 mb-1">
          <i class="fas fa-database mr-1"></i>Replication Package
        </a>
      </div>
    </div>

  </div>

  <!-- Footer: Keywords -->
  <hr class="mt-0" />
  <div class="d-flex align-items-center flex-wrap">
    <span class="small text-muted mr-2"><i class="fas fa-tags mr-1"></i>Keywords:</span>
    <span class="badge badge-light border mr-1">GitHub Actions</span>
    <span class="badge badge-light border mr-1">CI/CD</span>
    <span class="badge badge-light border mr-1">Workflow Runs</span>
    <span class="badge badge-light border mr-1">Visualization</span>
    <span class="badge badge-light border mr-1">Program Comprehension</span>
  </div>

</div>
