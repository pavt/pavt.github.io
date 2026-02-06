---
show: true
width: 12
date: 2026-06-15 00:00:00 +0800
group: ""
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

  <!-- ===== ABSTRACT ===== -->
  <div class="mb-4">
    <h6 class="font-weight-bold text-uppercase" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
      <i class="fas fa-align-left mr-1"></i>Abstract
    </h6>
    <p class="small text-justify" style="line-height: 1.7;">
      Workflow runs record the executions of continuous integration and delivery specifications. They serve as the primary monitoring mechanism, enabling failure detection and integration reliability assessment. However, understanding run intricacies is far from trivial. Each run involves multiple interdependent execution units (e.g., attempts, jobs, and steps) whose relationships are not immediately visible. Moreover, current tools provide limited support for detecting patterns across runs, particularly in projects with high workflow execution frequency. As a result, run monitoring remains constrained to fragmented views that are cumbersome to use.
    </p>
    <p class="small text-justify" style="line-height: 1.7;">
      We present a novel approach that supports workflow run comprehension through interactive and animated visualizations. Our approach enables developers to inspect end-to-end execution traces and to identify structural and behavioral patterns. We implemented a GitHub Actions prototype and analyzed runs from public repositories to illustrate its potential. Preliminary insights suggest that the approach is feasible and provides a starting point for workflow run comprehension analysis.
    </p>
  </div>

  <!-- ===== APPROACH PIPELINE ===== -->
  <div class="text-center mb-4">
    <img src="{{ 'assets/images/showcase/run-visualizer/app_overview.png' | relative_url }}" alt="Approach Overview" class="img-fluid rounded" style="max-height: 120px;">
    <p class="text-center text-muted small mt-1">Approach: GitHub repositories &rarr; Data extraction &rarr; Run Domain Model &rarr; Specific Views &rarr; Interactive Visual Narratives</p>
  </div>

  <hr />

  <!-- ===== APPROACH STEPS ===== -->
  <div class="row mb-4">
    <div class="col-md-4 mb-2">
      <div class="p-3 rounded text-center h-100" style="background-color: #f8f9fa;">
        <i class="fas fa-download mb-2" style="font-size: 1.2rem; color: #6c757d;"></i>
        <div class="font-weight-bold">Data Extraction</div>
        <div class="small text-muted">Mining structured and unstructured run data from GitHub REST API (JSON metadata + log files).</div>
      </div>
    </div>
    <div class="col-md-4 mb-2">
      <div class="p-3 rounded text-center h-100" style="background-color: #f8f9fa;">
        <i class="fas fa-project-diagram mb-2" style="font-size: 1.2rem; color: #6c757d;"></i>
        <div class="font-weight-bold">Domain Model</div>
        <div class="small text-muted">A Workflow Run Domain Model capturing execution entities (attempts, jobs, steps) and contextual entities (failure-context, commits).</div>
      </div>
    </div>
    <div class="col-md-4 mb-2">
      <div class="p-3 rounded text-center h-100" style="background-color: #f8f9fa;">
        <i class="fas fa-chart-bar mb-2" style="font-size: 1.2rem; color: #6c757d;"></i>
        <div class="font-weight-bold">Visualization</div>
        <div class="small text-muted">Interactive and animated coarse- and fine-grained views revealing execution behavior at multiple levels of detail.</div>
      </div>
    </div>
  </div>

  <hr />

  <!-- ===== VISUALIZATIONS ===== -->
  <h6 class="font-weight-bold text-uppercase text-center mb-3" style="letter-spacing: 0.05em; font-size: 0.75rem; color: #6c757d;">
    <i class="fas fa-eye mr-1"></i>Run-Visualizer
  </h6>

  <!-- Tool screenshot (highest res image) -->
  <div class="mb-4">
    <img src="{{ 'assets/images/showcase/run-visualizer/coarse-fine-views.png' | relative_url }}" alt="Run-Visualizer Tool" class="img-fluid rounded shadow-sm w-100">
    <p class="text-center text-muted small mt-2"><em>Run-Visualizer</em> — Coarse-grained polymetric view (left) and fine-grained run anatomy view (right), built on <a href="https://gtoolkit.com/" target="_blank">Glamorous Toolkit</a></p>
  </div>

  <!-- Run Anatomy detail -->
  <div class="row mb-3">
    <div class="col-md-7 mb-3">
      <div class="border rounded p-3 h-100" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-2"><span class="badge badge-info mr-1">Fine-grained</span> Run Anatomy View</h6>
        <img src="{{ 'assets/images/showcase/run-visualizer/run-anatomy-view.png' | relative_url }}" alt="Run Anatomy View" class="img-fluid rounded mb-2">
        <p class="small text-muted mb-0">Five coordinated panels — Attempts, Jobs, Steps, Log (microprint), and Commit — with animated transitions to reconstruct end-to-end execution traces.</p>
      </div>
    </div>
    <div class="col-md-5 mb-3">
      <div class="border rounded p-3 h-100 d-flex flex-column justify-content-center" style="background-color: #fdfdfd;">
        <h6 class="font-weight-bold mb-3">Supported Views</h6>
        <div class="small">
          <div class="mb-2">
            <span class="badge badge-success mr-1">Coarse</span>
            <strong>Polymetric Runs</strong>
            <div class="text-muted ml-4" style="font-size: 0.85em;">Rectangles encoding jobs, duration, conclusion state, and triggering events across workflows.</div>
          </div>
          <div class="mb-2">
            <span class="badge badge-success mr-1">Coarse</span>
            <strong>Polymetric Actors</strong>
            <div class="text-muted ml-4" style="font-size: 0.85em;">Actor participation: runs triggered, workflows involved, bot vs. human distinction.</div>
          </div>
          <div class="mb-2">
            <span class="badge badge-info mr-1">Fine</span>
            <strong>Run Anatomy</strong>
            <div class="text-muted ml-4" style="font-size: 0.85em;">Animated decomposition of a single run into attempts, jobs, steps, and log microprints.</div>
          </div>
          <div class="mb-2">
            <span class="badge badge-danger mr-1">Fine</span>
            <strong>Failure-Context Collection</strong>
            <div class="text-muted ml-4" style="font-size: 0.85em;">Author-workflow matrix, failures by step, and failures by commit.</div>
          </div>
        </div>
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
