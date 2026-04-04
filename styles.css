document.documentElement.classList.add("js-enabled");

const header = document.querySelector(".site-header");
const menuToggle = document.querySelector("[data-menu-toggle]");
const navLinks = document.querySelectorAll(".mobile-nav a, .mobile-cta");
const revealItems = document.querySelectorAll(".reveal");
const carousels = document.querySelectorAll("[data-carousel]");
const spotlightEcosystem = document.querySelector("[data-spotlight-ecosystem]");

if (menuToggle && header) {
  menuToggle.addEventListener("click", () => {
    const isOpen = header.classList.toggle("is-open");
    menuToggle.setAttribute("aria-expanded", String(isOpen));
  });

  navLinks.forEach((link) => {
    link.addEventListener("click", () => {
      header.classList.remove("is-open");
      menuToggle.setAttribute("aria-expanded", "false");
    });
  });
}

if (spotlightEcosystem) {
  const spotlightCards = Array.from(spotlightEcosystem.querySelectorAll("[data-spotlight-card]"));
  const spotlightWide = window.matchMedia("(min-width: 861px)");
  const spotlightHover = window.matchMedia("(min-width: 861px) and (hover: hover) and (pointer: fine)");
  const defaultFeaturedIndex = "0";
  let spotlightHoverTimer = 0;
  let spotlightResetTimer = 0;

  const clearSpotlightTimers = () => {
    window.clearTimeout(spotlightHoverTimer);
    window.clearTimeout(spotlightResetTimer);
  };

  const setFeaturedSpotlightCard = (index) => {
    const nextIndex = String(index);

    if (spotlightEcosystem.dataset.featuredCard === nextIndex) {
      return;
    }

    spotlightEcosystem.dataset.featuredCard = nextIndex;
  };

  const resetSpotlightLayout = () => {
    setFeaturedSpotlightCard(defaultFeaturedIndex);
  };

  spotlightCards.forEach((card, index) => {
    card.addEventListener("mouseenter", () => {
      if (!spotlightHover.matches) {
        return;
      }

      window.clearTimeout(spotlightResetTimer);
      window.clearTimeout(spotlightHoverTimer);
      spotlightHoverTimer = window.setTimeout(() => {
        setFeaturedSpotlightCard(index);
      }, 90);
    });

    card.addEventListener("focusin", () => {
      if (!spotlightWide.matches) {
        return;
      }

      clearSpotlightTimers();
      setFeaturedSpotlightCard(index);
    });
  });

  spotlightEcosystem.addEventListener("mouseleave", () => {
    if (!spotlightHover.matches || spotlightEcosystem.matches(":focus-within")) {
      return;
    }

    window.clearTimeout(spotlightHoverTimer);
    spotlightResetTimer = window.setTimeout(() => {
      resetSpotlightLayout();
    }, 120);
  });

  spotlightEcosystem.addEventListener("focusout", (event) => {
    if (spotlightEcosystem.contains(event.relatedTarget)) {
      return;
    }

    clearSpotlightTimers();
    resetSpotlightLayout();
  });

  window.addEventListener("resize", () => {
    clearSpotlightTimers();

    if (!spotlightWide.matches) {
      resetSpotlightLayout();
      return;
    }

    if (!spotlightEcosystem.dataset.featuredCard) {
      resetSpotlightLayout();
    }
  });
}

carousels.forEach((carousel) => {
  const track = carousel.querySelector("[data-carousel-track]");
  const prevButton = carousel.querySelector("[data-carousel-prev]");
  const nextButton = carousel.querySelector("[data-carousel-next]");

  if (!track || !prevButton || !nextButton) {
    return;
  }

  const getScrollAmount = () => {
    const firstCard = track.querySelector(".company-card");

    if (!firstCard) {
      return track.clientWidth * 0.9;
    }

    const styles = window.getComputedStyle(track);
    const gap = Number.parseFloat(styles.columnGap || styles.gap || "0") || 0;

    return firstCard.getBoundingClientRect().width + gap;
  };

  const updateControls = () => {
    const maxScrollLeft = track.scrollWidth - track.clientWidth - 4;
    const isScrollable = maxScrollLeft > 8;
    prevButton.disabled = track.scrollLeft <= 4;
    nextButton.disabled = track.scrollLeft >= maxScrollLeft;
    carousel.classList.toggle("is-scrollable", isScrollable);
    carousel.classList.toggle("is-scroll-start", !isScrollable || track.scrollLeft <= 4);
    carousel.classList.toggle("is-scroll-end", !isScrollable || track.scrollLeft >= maxScrollLeft);
  };

  prevButton.addEventListener("click", () => {
    track.scrollBy({ left: -getScrollAmount(), behavior: "smooth" });
  });

  nextButton.addEventListener("click", () => {
    track.scrollBy({ left: getScrollAmount(), behavior: "smooth" });
  });

  track.addEventListener("scroll", updateControls, { passive: true });
  window.addEventListener("resize", updateControls);
  updateControls();

  if (carousel.id !== "systems") {
    return;
  }

  const viewToggle = carousel.querySelector("[data-ecosystem-view]");
  const browseHint = carousel.querySelector(".companies-browse-hint");

  if (!viewToggle) {
    return;
  }

  const systemsMarkup = track.innerHTML;
  const systemsLinks = document.querySelectorAll('a[href="#systems"]');
  const ecosystemLinks = document.querySelectorAll('a[href="#ecosystem-view"]');
  const ecosystemButtonLabel = "View Ecosystem";
  const systemsButtonLabel = "View Systems";
  let activeView = "systems";
  let pendingView = "systems";
  let switchTimer = 0;
  const ecosystemProfiles = [
    {
      name: "Aegis & Co.",
      category: "Systems",
      lead: "Where operations are rebuilt through AI and RPA.",
      support: "This is where the work that slows businesses down gets removed.",
      tone: "operations",
    },
    {
      name: "NAMI Studio",
      category: "Marketing",
      lead: "Where positioning, design, and communication get aligned.",
      support: "Clear positioning. No mixed signals.",
      tone: "automation",
    },
    {
      name: "PCAA",
      category: "Education",
      lead: "Where modern business thinking gets documented.",
      support: "Meant to be used, not just learned.",
      tone: "infrastructure",
    },
    {
      name: "Acquisitions",
      category: "Ownership",
      lead: "Where businesses get owned and improved.",
      support: "We keep what works and make it better over time.",
      tone: "operations",
    },
  ];

  const escapeHtml = (value) =>
    String(value)
      .replaceAll("&", "&amp;")
      .replaceAll("<", "&lt;")
      .replaceAll(">", "&gt;")
      .replaceAll('"', "&quot;")
      .replaceAll("'", "&#39;");

  const renderEcosystemMarkup = () =>
    ecosystemProfiles
      .map(
        (entry) => `
          <article class="company-card ecosystem-card company-card-${entry.tone}">
            <div class="company-head">
              <h3>${escapeHtml(entry.name)}</h3>
              <p class="company-card-pill">${escapeHtml(entry.category)}</p>
              <p class="company-lead">${escapeHtml(entry.lead)}</p>
            </div>
            <p class="company-support">${escapeHtml(entry.support)}</p>
          </article>
        `
      )
      .join("");

  const syncViewToggle = (nextView) => {
    const isEcosystemView = nextView === "ecosystem";
    viewToggle.classList.toggle("is-active", isEcosystemView);
    viewToggle.setAttribute("aria-pressed", String(isEcosystemView));
    viewToggle.textContent = isEcosystemView ? systemsButtonLabel : ecosystemButtonLabel;
  };

  const syncBrowseHint = (nextView) => {
    if (!browseHint) {
      return;
    }

    browseHint.textContent = nextView === "ecosystem" ? "Browse Ecosystem" : "Browse Systems";
  };

  const commitView = (nextView) => {
    track.innerHTML = nextView === "ecosystem" ? renderEcosystemMarkup() : systemsMarkup;
    track.scrollLeft = 0;
    activeView = nextView;
    pendingView = nextView;
    carousel.dataset.view = nextView;
    syncViewToggle(nextView);
    syncBrowseHint(nextView);
    updateControls();
  };

  const setSystemsView = (nextView, options = {}) => {
    const { animate = true } = options;

    if (nextView === activeView && nextView === pendingView) {
      syncViewToggle(nextView);
      syncBrowseHint(nextView);
      carousel.dataset.view = nextView;
      return;
    }

    window.clearTimeout(switchTimer);
    pendingView = nextView;

    if (!animate) {
      carousel.classList.remove("is-view-transitioning");
      commitView(nextView);
      return;
    }

    if (nextView === activeView) {
      carousel.classList.remove("is-view-transitioning");
      syncViewToggle(nextView);
      syncBrowseHint(nextView);
      carousel.dataset.view = nextView;
      return;
    }

    carousel.classList.add("is-view-transitioning");
    switchTimer = window.setTimeout(() => {
      commitView(nextView);
      requestAnimationFrame(() => {
        carousel.classList.remove("is-view-transitioning");
      });
    }, 120);
  };

  viewToggle.addEventListener("click", () => {
    const nextView = activeView === "ecosystem" ? "systems" : "ecosystem";

    setSystemsView(nextView);

    if (nextView === "ecosystem") {
      if (window.location.hash !== "#ecosystem-view") {
        window.history.replaceState(null, "", "#ecosystem-view");
      }
      return;
    }

    if (window.location.hash !== "#systems") {
      window.history.replaceState(null, "", "#systems");
    }
  });

  systemsLinks.forEach((link) => {
    link.addEventListener("click", () => {
      setSystemsView("systems");
    });
  });

  ecosystemLinks.forEach((link) => {
    link.addEventListener("click", () => {
      setSystemsView("ecosystem");
    });
  });

  const syncSystemsViewFromHash = () => {
    if (window.location.hash === "#ecosystem-view") {
      setSystemsView("ecosystem", { animate: false });
      return;
    }

    if (window.location.hash === "#systems") {
      setSystemsView("systems", { animate: false });
    }
  };

  syncSystemsViewFromHash();
  window.addEventListener("hashchange", syncSystemsViewFromHash);
});

if ("IntersectionObserver" in window) {
  const observer = new IntersectionObserver(
    (entries, currentObserver) => {
      entries.forEach((entry) => {
        if (!entry.isIntersecting) {
          return;
        }

        entry.target.classList.add("is-visible");
        currentObserver.unobserve(entry.target);
      });
    },
    {
      rootMargin: "0px 0px -8% 0px",
      threshold: 0.15,
    }
  );

  revealItems.forEach((item) => observer.observe(item));
} else {
  revealItems.forEach((item) => item.classList.add("is-visible"));
}
