---
show: true
width: 12
date: 2026-06-15 00:00:00 +0800
group: Research
---

<div class="p-4">

  <!-- ===== HEADER ===== -->
  <div class="text-center mb-4">
    <div class="mb-2">
      <span class="badge badge-pill badge-publication badge-primary">ICPC 2026</span>
      <span class="badge badge-pill badge-publication badge-secondary">Conference</span>
      <span class="badge badge-pill badge-light border text-muted ml-1"><i class="fas fa-map-marker-alt mr-1"></i>Rio de Janeiro, Brazil</span>
    </div>
    <h3 class="font-weight-bold mb-2">Understanding CI/CD Workflow Runs<br>Through Interactive and Animated Visualizations</h3>
    <p class="text-muted small mb-2">
      <strong>Pablo Valenzuela-Toledo</strong> <span class="text-muted">(University of Bern &middot; Universidad de La Frontera)</span> &middot;
      <strong>Timo Kehrer</strong> <span class="text-muted">(University of Bern)</span> &middot;
      <strong>Sebastiano Panichella</strong> <span class="text-muted">(University of Bern &middot; AI4I)</span>
    </p>
    <div>
      <a href="/assets/pdfs/Understanding-CICD-Workflow-Runs-Interactive-Animated-Visualizations.pdf" target="_blank" class="btn btn-sm btn-primary mr-1">
        <i class="fas fa-file-pdf mr-1"></i>Paper
      </a>
      <a href="https://doi.org/10.5281/zenodo.17635512" target="_blank" class="btn btn-sm btn-outline-secondary mr-1">
        <i class="fas fa-database mr-1"></i>Replication Package
      </a>
      <a href="https://doi.org/10.5281/zenodo.18272174" target="_blank" class="btn btn-sm btn-outline-secondary">
        <i class="fas fa-bookmark mr-1"></i>DOI
      </a>
    </div>
  </div>

  <hr />

  <!-- ===== APPROACH PIPELINE ===== -->
  <div class="text-center mb-4">
    <img src="{{ 'assets/images/showcase/run-visualizer/app_overview.png' | relative_url }}" alt="Approach Overview" class="img-fluid rounded" style="max-height: 100px;">
  </div>

  <!-- ===== MOTIVATION + APPROACH ===== -->
  <div class="row mb-4">
    <div class="col-md-5 mb-3">
      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-exclamation-circle mr-1"></i>Problem
      </h6>
      <p class="small" style="line-height: 1.7;">
        Workflow runs involve multiple interdependent execution units (attempts, jobs, steps) whose relationships are not immediately visible. Current tools provide fragmented and predominantly textual representations that limit pattern detection and failure diagnosis across run histories.
      </p>
    </div>
    <div class="col-md-7 mb-3">
      <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
        <i class="fas fa-cogs mr-1"></i>Approach
      </h6>
      <div class="small" style="line-height: 1.7;">
        <div class="row">
          <div class="col-sm-4 mb-2">
            <div class="p-2 rounded text-center" style="background-color: #f8f9fa;">
              <i class="fas fa-download mb-1" style="color: #6c757d;"></i>
              <div><strong>Data Extraction</strong></div>
              <div class="text-muted" style="font-size: 0.85em;">GitHub REST API<br>JSON + Logs</div>
            </div>
          </div>
          <div class="col-sm-4 mb-2">
            <div class="p-2 rounded text-center" style="background-color: #f8f9fa;">
              <i class="fas fa-project-diagram mb-1" style="color: #6c757d;"></i>
              <div><strong>Domain Model</strong></div>
              <div class="text-muted" style="font-size: 0.85em;">Execution + Context<br>entities</div>
            </div>
          </div>
          <div class="col-sm-4 mb-2">
            <div class="p-2 rounded text-center" style="background-color: #f8f9fa;">
              <i class="fas fa-chart-bar mb-1" style="color: #6c757d;"></i>
              <div><strong>Visualization</strong></div>
              <div class="text-muted" style="font-size: 0.85em;">Interactive &amp; animated<br>multi-level views</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <hr />

  <!-- ===== VISUALIZATIONS ===== -->
  <h6 class="font-weight-bold text-uppercase text-center mb-3" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
    <i class="fas fa-eye mr-1"></i>Visualizations — Run-Visualizer
  </h6>

  <!-- Tool screenshot -->
  <div class="mb-4">
    <img src="{{ 'assets/images/showcase/run-visualizer/coarse-fine-views.png' | relative_url }}" alt="Run-Visualizer Tool" class="img-fluid rounded shadow-sm w-100">
    <p class="text-center text-muted small mt-1"><em>Run-Visualizer</em> — Coarse-grained (left) and fine-grained (right) views built on Glamorous Toolkit</p>
  </div>

  <!-- Views grid: 2x2 -->
  <div class="row mb-3">

    <!-- Polymetric Run View -->
    <div class="col-md-6 mb-3">
      <div class="border rounded p-3 h-100" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-2"><span class="badge badge-success mr-1">Coarse</span> Polymetric Run View</h6>
        <img src="{{ 'assets/images/showcase/run-visualizer/polymetric-view.png' | relative_url }}" alt="Polymetric Run View" class="img-fluid rounded mb-2">
        <p class="small text-muted mb-0">Each run is a rectangle: width = # jobs, height = duration, color = conclusion state. Hatched headers encode triggering events.</p>
      </div>
    </div>

    <!-- Run Anatomy View -->
    <div class="col-md-6 mb-3">
      <div class="border rounded p-3 h-100" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-2"><span class="badge badge-info mr-1">Fine</span> Run Anatomy View</h6>
        <img src="{{ 'assets/images/showcase/run-visualizer/run-anatomy-view.png' | relative_url }}" alt="Run Anatomy View" class="img-fluid rounded mb-2">
        <p class="small text-muted mb-0">Coordinated panels (Attempts, Jobs, Steps, Log, Commit) with animated transitions to trace execution flow.</p>
      </div>
    </div>

    <!-- Failure Context View -->
    <div class="col-md-6 mb-3">
      <div class="border rounded p-3 h-100" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-2"><span class="badge badge-danger mr-1">Fine</span> Failure-Context View</h6>
        <img src="{{ 'assets/images/showcase/run-visualizer/context-view.png' | relative_url }}" alt="Failure Context View" class="img-fluid rounded mb-2">
        <p class="small text-muted mb-0">Failure collection, author-workflow matrix, failures by step, and failures by commit — linking developers to instability sources.</p>
      </div>
    </div>

    <!-- Run Anatomy View 2 (from paper) -->
    <div class="col-md-6 mb-3">
      <div class="border rounded p-3 h-100" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-2"><span class="badge badge-info mr-1">Fine</span> Run Anatomy — electron/electron</h6>
        <img src="{{ 'assets/images/showcase/run-visualizer/run-anatomy-view-2.png' | relative_url }}" alt="Run Anatomy View electron" class="img-fluid rounded mb-2">
        <p class="small text-muted mb-0">Build workflow run trace showing failure propagation across attempts, jobs, steps, and log microprints.</p>
      </div>
    </div>

  </div>

  <hr />

  <!-- ===== FOOTER ===== -->
  <div class="d-flex justify-content-between align-items-center flex-wrap">
    <div>
      <span class="small text-muted mr-2"><i class="fas fa-tags mr-1"></i></span>
      <span class="badge badge-light border mr-1">GitHub Actions</span>
      <span class="badge badge-light border mr-1">CI/CD</span>
      <span class="badge badge-light border mr-1">Workflow Runs</span>
      <span class="badge badge-light border mr-1">Software Visualization</span>
      <span class="badge badge-light border mr-1">Program Comprehension</span>
    </div>
    <div class="small text-muted mt-2 mt-md-0">
      <i class="fas fa-tools mr-1"></i>Built on <a href="https://gtoolkit.com/" target="_blank">Glamorous Toolkit</a>
    </div>
  </div>

</div>
