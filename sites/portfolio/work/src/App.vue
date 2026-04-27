<script setup lang="ts">
  // The Shop Floor.
  // No complex logic today. Just the foundation.
</script>

<template>
  <main class="studio-layout">
    <nav class="studio-nav">
      <div class="brand">Joseph Baranoski</div>
      <div class="role">Lead Architect & Engineer</div>
    </nav>

    <header class="hero">
      <h1 class="headline">
        Engineering
        <br />
        <span class="italic-serif">with Intent.</span>
      </h1>
      <p class="mission-statement">
        Specializing in institutional-grade architecture, forensic frontend
        recovery, and high-performance interactive systems. Building the digital
        shop floor with clarity and precision.
      </p>
    </header>

    <section class="workbench">
      <div class="project-card placeholder">
        <span class="label">01 // Case Study</span>
        <h2>Accent Capital</h2>
        <p>
          Institutional investment platform featuring a custom Canvas-driven
          state engine.
        </p>
      </div>

      <div class="project-card placeholder">
        <span class="label">02 // Forensic Architecture</span>
        <h2>Enterprise Scale</h2>
        <p>
          Untangling legacy monorepos to restore performance and developer
          velocity.
        </p>
      </div>

      <div class="project-card placeholder lab-card">
        <span class="label">03 // The Lab</span>
        <h2>Interactive Web</h2>
        <p>
          R&D experiments in data visualization, Vue reactivity, and Canvas
          mechanics.
        </p>
      </div>
    </section>
  </main>
</template>

<style scoped>
  /* The "Institutional" Aesthetic
  Deep slates, cream text, and high-contrast serifs.
*/
  .studio-layout {
    min-height: 100vh;
    background-color: #1a1a1c; /* Deep architectural charcoal */
    color: #f4f4f0; /* Cream/off-white for less eye strain */
    font-family:
      -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial,
      sans-serif;
    padding: 2rem 4rem;
    box-sizing: border-box;
  }

  .studio-nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid rgba(244, 244, 240, 0.1);
    padding-bottom: 1.5rem;
    font-size: 0.85rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: #a3a3a3;
  }

  .hero {
    margin-top: 8rem;
    margin-bottom: 6rem;
    max-width: 800px;
  }

  .headline {
    font-size: 4.5rem;
    line-height: 1.1;
    margin-bottom: 2rem;
    font-weight: 300;
    letter-spacing: -0.02em;
  }

  .italic-serif {
    font-family: 'Playfair Display', 'Georgia', serif;
    font-style: italic;
    color: #d4af37; /* A subtle, muted gold/accent */
  }

  .mission-statement {
    font-size: 1.25rem;
    line-height: 1.6;
    color: #a3a3a3;
    max-width: 600px;
  }

  .workbench {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
    margin-top: 4rem;
  }

  .project-card {
    border: 1px solid rgba(244, 244, 240, 0.1);
    padding: 2rem;
    transition: border-color 0.3s ease;
    background-color: #1f1f22;
  }

  .project-card:hover {
    border-color: rgba(244, 244, 240, 0.4);
  }

  .label {
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    color: #d4af37;
    display: block;
    margin-bottom: 1.5rem;
  }

  h2 {
    font-family: 'Playfair Display', 'Georgia', serif;
    font-size: 1.8rem;
    font-weight: 400;
    margin-bottom: 1rem;
  }

  p {
    font-size: 0.95rem;
    line-height: 1.5;
    color: #888;
  }

  /* A slight visual shift for the "Lab" experiments */
  .lab-card {
    background: linear-gradient(145deg, #1f1f22 0%, #171c21 100%);
  }
</style>
