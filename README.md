<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Parea Collective</title>
    <meta
      name="description"
      content="Parea Collective is the operating layer behind modern business through systems, doctrine, and long-term ownership."
    />
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&amp;family=Montserrat:wght@500;600;700;800&amp;display=swap"
      rel="stylesheet"
    />
    <link rel="stylesheet" href="styles.css" />
    <script src="script.js" defer></script>
  </head>
  <body>
    <header class="site-header">
      <div class="container header-shell">
        <a class="brand" href="#top" aria-label="Parea Collective home">Parea Collective</a>

        <nav class="site-nav desktop-nav" aria-label="Primary">
          <a href="#top">Home</a>
          <a href="#philosophy">Philosophy</a>
          <a href="#ecosystem-view">Ecosystem</a>
          <a href="#systems">Systems</a>
          <a href="#pcaa">Education</a>
          <a href="#acquisitions-overview">Acquisitions</a>
        </nav>

        <a class="button button-accent desktop-cta" href="mailto:hello@pareacollective.com"
          >Contact</a
        >

        <button
          class="menu-toggle"
          type="button"
          aria-expanded="false"
          aria-controls="site-navigation"
          data-menu-toggle
        >
          <span></span>
          <span></span>
          <span class="sr-only">Toggle navigation</span>
        </button>
      </div>

      <div class="container mobile-nav-shell" id="site-navigation" data-nav>
        <nav class="site-nav mobile-nav" aria-label="Mobile primary">
          <a href="#top">Home</a>
          <a href="#philosophy">Philosophy</a>
          <a href="#ecosystem-view">Ecosystem</a>
          <a href="#systems">Systems</a>
          <a href="#pcaa">Education</a>
          <a href="#acquisitions-overview">Acquisitions</a>
        </nav>
        <a class="button button-accent mobile-cta" href="mailto:hello@pareacollective.com"
          >Contact</a
        >
      </div>
    </header>

    <main id="top">
      <section class="hero">
        <div class="container hero-shell">
          <div class="hero-main reveal">
            <p class="eyebrow">Operations, Systems and Ownership</p>
            <h1>
              <span class="hero-desktop-line">The Operating Layer</span>
              <span class="hero-desktop-line">of Modern Business</span>
            </h1>
          </div>

          <aside class="hero-side reveal">
            <p class="hero-support">
              <span class="hero-support-line">Modern businesses don&rsquo;t scale people.</span>
              <span class="hero-support-line">They scale systems.</span>
            </p>

            <div class="hero-actions">
              <a class="button button-dark" href="#systems">View Systems</a>
              <a class="button button-secondary" href="#acquisitions-overview"
                >Explore Acquisitions</a
              >
            </div>
          </aside>
        </div>

        <div
          class="container spotlight-grid spotlight-grid-anchors spotlight-ecosystem mobile-spotlight-reveal desktop-spotlight-reveal reveal"
          data-spotlight-ecosystem
          data-featured-card="0"
        >
          <article
            class="spotlight-card anchor-card reveal"
            id="aegis-co"
            data-spotlight-card
            data-spotlight-index="0"
          >
            <div class="spotlight-copy">
              <span class="spotlight-label">Systems</span>
              <h2>Aegis &amp; Co.</h2>
              <p>AI and RPA for cleaner operations.</p>
              <a class="spotlight-link" href="#ecosystem-view">
                View Aegis &amp; Co.
                <span class="spotlight-link-icon" aria-hidden="true">
                  <svg viewBox="0 0 20 20" fill="none">
                    <path d="M12.5 4H6.5A2.5 2.5 0 0 0 4 6.5v7A2.5 2.5 0 0 0 6.5 16h7a2.5 2.5 0 0 0 2.5-2.5v-6" />
                    <path d="M11.5 4H16v4.5" />
                    <path d="M15.75 4.25 9.5 10.5" />
                  </svg>
                </span>
              </a>
            </div>
          </article>

          <article
            class="spotlight-card anchor-card reveal"
            id="nami"
            data-spotlight-card
            data-spotlight-index="1"
          >
            <div class="spotlight-copy">
              <span class="spotlight-label">Marketing</span>
              <h2>NAMI Studio</h2>
              <p>Design and communication systems.</p>
              <a class="spotlight-link" href="#ecosystem-view">
                View NAMI Studio
                <span class="spotlight-link-icon" aria-hidden="true">
                  <svg viewBox="0 0 20 20" fill="none">
                    <path d="M12.5 4H6.5A2.5 2.5 0 0 0 4 6.5v7A2.5 2.5 0 0 0 6.5 16h7a2.5 2.5 0 0 0 2.5-2.5v-6" />
                    <path d="M11.5 4H16v4.5" />
                    <path d="M15.75 4.25 9.5 10.5" />
                  </svg>
                </span>
              </a>
            </div>
          </article>

          <article
            class="spotlight-card anchor-card reveal"
            id="pcaa"
            data-spotlight-card
            data-spotlight-index="2"
          >
            <div class="spotlight-copy">
              <span class="spotlight-label">Education</span>
              <h2>PCAA</h2>
              <p>Doctrine for modern operators.</p>
              <a class="spotlight-link" href="#ecosystem-view">
                View PCAA
                <span class="spotlight-link-icon" aria-hidden="true">
                  <svg viewBox="0 0 20 20" fill="none">
                    <path d="M12.5 4H6.5A2.5 2.5 0 0 0 4 6.5v7A2.5 2.5 0 0 0 6.5 16h7a2.5 2.5 0 0 0 2.5-2.5v-6" />
                    <path d="M11.5 4H16v4.5" />
                    <path d="M15.75 4.25 9.5 10.5" />
                  </svg>
                </span>
              </a>
            </div>
          </article>

          <article
            class="spotlight-card anchor-card reveal"
            id="acquisitions"
            data-spotlight-card
            data-spotlight-index="3"
          >
            <div class="spotlight-copy">
              <span class="spotlight-label">Ownership</span>
              <h2>Acquisitions</h2>
              <p>Long term ownership and improvement.</p>
              <a class="spotlight-link" href="#acquisitions-overview">
                View Acquisitions
                <span class="spotlight-link-icon" aria-hidden="true">
                  <svg viewBox="0 0 20 20" fill="none">
                    <path d="M12.5 4H6.5A2.5 2.5 0 0 0 4 6.5v7A2.5 2.5 0 0 0 6.5 16h7a2.5 2.5 0 0 0 2.5-2.5v-6" />
                    <path d="M11.5 4H16v4.5" />
                    <path d="M15.75 4.25 9.5 10.5" />
                  </svg>
                </span>
              </a>
            </div>
          </article>
        </div>
      </section>

      <section class="section companies-showcase" id="systems" data-carousel>
        <div class="section-anchor" id="ecosystem-view" aria-hidden="true"></div>
        <div class="container">
          <div class="companies-head reveal">
            <div class="companies-intro">
              <p class="eyebrow">Systems &amp; Companies</p>
              <h2>Where systems turn into leverage.</h2>
              <p class="companies-subhead">
                Every business runs on systems &ndash; whether they&rsquo;re visible or not.
              </p>
              <p>Most of them aren&rsquo;t designed. They just happen.</p>
            </div>

            <div class="carousel-controls" aria-label="Systems and companies carousel controls">
              <button
                class="carousel-button"
                type="button"
                data-carousel-prev
                aria-label="Show previous cards"
              >
                <span aria-hidden="true">&larr;</span>
              </button>
              <button
                class="carousel-button"
                type="button"
                data-carousel-next
                aria-label="Show next cards"
              >
                <span aria-hidden="true">&rarr;</span>
              </button>
            </div>
          </div>

          <div class="companies-carousel reveal">
            <div class="companies-track" data-carousel-track id="systems-track">
              <article class="company-card company-card-operations" data-system-card="operating-design">
                <div class="company-head">
                  <h3>Operating Design</h3>
                  <p class="company-card-pill">Operations</p>
                  <p class="company-lead">
                    Who does what, how decisions get made, and where things get stuck.
                  </p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>Less confusion.</dd>
                  </div>
                </dl>
                <p class="company-support">Things move without constant back-and-forth.</p>
              </article>

              <article class="company-card company-card-infrastructure" data-system-card="reporting">
                <div class="company-head">
                  <h3>Reporting</h3>
                  <p class="company-card-pill">Infrastructure</p>
                  <p class="company-lead">See what&rsquo;s actually happening inside the business.</p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>Faster decisions.</dd>
                  </div>
                </dl>
                <p class="company-support">No more guessing.</p>
              </article>

              <article class="company-card company-card-automation" data-system-card="automation">
                <div class="company-head">
                  <h3>Automation</h3>
                  <p class="company-card-pill">Workflows</p>
                  <p class="company-lead">
                    Remove the repetitive work people shouldn&rsquo;t be doing in the first place.
                  </p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>More leverage.</dd>
                  </div>
                </dl>
                <p class="company-support">People focus on what actually matters.</p>
              </article>

              <article class="company-card company-card-operations" data-system-card="doctrine">
                <div class="company-head">
                  <h3>Doctrine</h3>
                  <p class="company-card-pill">Standards</p>
                  <p class="company-lead">A shared way of thinking about how things get done.</p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>Better decisions.</dd>
                  </div>
                </dl>
                <p class="company-support">Everyone operates the same way.</p>
              </article>

              <article class="company-card company-card-infrastructure" data-system-card="modernization">
                <div class="company-head">
                  <h3>Modernization</h3>
                  <p class="company-card-pill">Infrastructure</p>
                  <p class="company-lead">
                    Upgrade how the business runs without breaking what&rsquo;s already working.
                  </p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>Things run smoother.</dd>
                  </div>
                </dl>
                <p class="company-support">Less friction across the business.</p>
              </article>

              <article class="company-card company-card-operations" data-system-card="acquisitions">
                <div class="company-head">
                  <h3>Acquisitions</h3>
                  <p class="company-card-pill">Ownership</p>
                  <p class="company-lead">We buy businesses and hold them long term.</p>
                </div>
                <dl class="company-meta">
                  <div>
                    <dt>Effect</dt>
                    <dd>Built to last.</dd>
                  </div>
                </dl>
                <p class="company-support">Not flipped, not stripped.</p>
              </article>
            </div>
          </div>

          <p class="companies-browse-hint reveal">Browse Systems</p>

          <div class="companies-footer reveal">
            <button
              class="button button-secondary companies-toggle"
              type="button"
              data-ecosystem-view
              aria-controls="systems-track"
              aria-pressed="false"
            >
              View Ecosystem
            </button>
            <a class="button button-dark" href="#acquisitions-overview">View Acquisitions</a>
          </div>
        </div>
      </section>

      <section class="section identity philosophy-section" id="philosophy">
        <div class="container philosophy-shell">
          <div class="philosophy-header reveal">
            <p class="eyebrow">Philosophy</p>
            <h2 class="philosophy-title">
              Most businesses don&rsquo;t have a people problem. They have a system problem.
            </h2>
            <p class="philosophy-intro">
              Work gets buried in coordination, handoffs, and invisible friction. The role of
              systems is to remove work that should not exist in the first place.
            </p>
          </div>

          <ol class="philosophy-principles reveal">
            <li class="philosophy-principle-card">
              <div class="philosophy-principle-card-face">
                <span class="philosophy-principle-pill">01</span>
                <div class="philosophy-principle-copy">
                  <h3>Systems remove invisible work</h3>
                  <p>Good systems remove friction before it reaches people.</p>
                </div>
              </div>
            </li>
            <li class="philosophy-principle-card">
              <div class="philosophy-principle-card-face">
                <span class="philosophy-principle-pill">02</span>
                <div class="philosophy-principle-copy">
                  <h3>People should focus on meaningful work</h3>
                  <p>The goal is not more activity. It is better use of attention.</p>
                </div>
              </div>
            </li>
            <li class="philosophy-principle-card">
              <div class="philosophy-principle-card-face">
                <span class="philosophy-principle-pill">03</span>
                <div class="philosophy-principle-copy">
                  <h3>Structure makes growth sustainable</h3>
                  <p>Clear ownership, cleaner handoffs, and better decisions compound over time.</p>
                </div>
              </div>
            </li>
          </ol>
        </div>
      </section>

      <section class="section closing" id="acquisitions-overview">
        <div class="container">
          <div class="closing-panel reveal">
            <div class="closing-primary">
              <p class="eyebrow">Acquisitions</p>
              <h2>Built to own, not to flip.</h2>
            </div>

            <div class="closing-secondary">
              <div class="closing-copy">
                <p>
                  We focus on businesses that already work &ndash; and make them run better.
                  Cleaner systems, better visibility, less friction.
                </p>
                <p>We keep what works and make it better over time.</p>
              </div>
              <div class="hero-actions closing-actions">
                <a class="button button-accent" href="mailto:hello@pareacollective.com"
                  >Get in Touch</a
                >
              </div>
            </div>
          </div>
        </div>
      </section>
    </main>

    <footer class="site-footer">
      <div class="container footer-shell">
        <div class="footer-branding">
          <a class="brand" href="#top">Parea Collective</a>
          <p class="footer-note">The operating layer behind modern business.</p>
        </div>

        <nav class="footer-mobile-nav" aria-label="Mobile footer">
          <a href="#top">Home</a>
          <a href="#ecosystem-view">Ecosystem</a>
          <a href="#systems">Systems</a>
          <a href="mailto:hello@pareacollective.com">Contact</a>
          <a href="mailto:hello@pareacollective.com?subject=LinkedIn">LinkedIn</a>
        </nav>

        <div class="footer-groups">
          <div class="footer-group">
            <p class="footer-heading">Parea Collective</p>
            <nav class="footer-nav" aria-label="Parea footer">
              <a href="#top">Home</a>
              <a href="#philosophy">Philosophy</a>
              <a href="#ecosystem-view">Ecosystem</a>
              <a href="#systems">Systems</a>
            </nav>
          </div>

          <div class="footer-group">
            <p class="footer-heading">Ecosystem</p>
            <nav class="footer-nav" aria-label="Ecosystem footer">
              <a href="#aegis-co">Aegis &amp; Co.</a>
              <a href="#nami">NAMI Studio</a>
              <a href="#pcaa">PCAA</a>
              <a href="#acquisitions">Acquisitions</a>
            </nav>
          </div>

          <div class="footer-group">
            <p class="footer-heading">Connect</p>
            <nav class="footer-nav" aria-label="Connect footer">
              <a href="mailto:hello@pareacollective.com?subject=LinkedIn">LinkedIn</a>
              <a href="mailto:hello@pareacollective.com">Contact</a>
              <a href="mailto:hello@pareacollective.com?subject=Legal">Legal</a>
            </nav>
          </div>
        </div>

        <p class="footer-copy">&copy; 2026 Parea Collective. All rights reserved.</p>
      </div>
    </footer>
  </body>
</html>
