---
layout: default
title: Home
---

<style>
/* The shared Hyde column is 38rem; give the home page a little more room so the
   meeting details and calendar can sit side by side without crowding. */
@media (min-width: 48em) {
  .content { max-width: 46rem; }
}

/* Masthead: small logo locked up with the title rather than floating above it. */
.hero {
  display: flex;
  align-items: center;
  gap: 1.25rem;
  margin-bottom: 1.5rem;
  padding-bottom: 1.5rem;
  border-bottom: 1px solid #e5e5e5;
}
.hero-logo {
  flex: 0 0 auto;
  width: 112px;   /* transparent PNG, trimmed and squared, so it optically centres */
  height: auto;
}
.hero-title {
  margin: 0;
  font-size: 1.85rem;
  line-height: 1.15;
  letter-spacing: -0.02rem;
}
.hero-tagline {
  margin: 0.4rem 0 0;
  color: #7a7a7a;
  font-size: 0.95rem;
}

/* Meeting block: details beside the calendar, collapsing to one column when narrow. */
.meet-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(17rem, 1fr));
  gap: 1.5rem;
  align-items: start;
  margin-bottom: 1rem;
}
.meet-photo {
  width: 100%;
  height: auto;
  border-radius: 4px;
  margin-bottom: 0.85rem;
}
.meet-list {
  margin: 0;
  padding-left: 1.1rem;
}
.meet-list li { margin-bottom: 0.35rem; }
.meet-calendar iframe {
  width: 100%;
  height: 22rem;
  border: 1px solid #e5e5e5;
  border-radius: 4px;
}

/* Mailing-list sign-up */
.joinlist {
  margin: 1rem 0 0;
  padding: 1.1rem 1.25rem;
  background: #faf9fc;
  border: 1px solid #e5e3ec;
  border-radius: 5px;
}
.joinlist-label {
  display: block;
  font-size: 0.95rem;
  margin-bottom: 0.6rem;
}
.joinlist-row { display: flex; flex-wrap: wrap; gap: 0.6rem; }
.joinlist input[type="email"] {
  flex: 1 1 14rem;
  min-width: 0;
  padding: 0.5rem 0.65rem;
  font: inherit;
  font-size: 0.95rem;
  border: 1px solid #cfcbdb;
  border-radius: 4px;
  background: #fff;
}
.joinlist input[type="email"]:focus {
  outline: 2px solid #36236a;
  outline-offset: 1px;
  border-color: #36236a;
}
.joinlist button {
  flex: 0 0 auto;
  padding: 0.5rem 1.1rem;
  font: inherit;
  font-size: 0.95rem;
  color: #fff;
  background: #36236a;
  border: 1px solid #36236a;
  border-radius: 4px;
  cursor: pointer;
}
.joinlist button:hover { background: #2a1b53; }
.joinlist-note {
  margin: 0.7rem 0 0;
  font-size: 0.85rem;
  color: #6f6f7a;
  line-height: 1.45;
}
.joinlist-status { margin: 0.6rem 0 0; font-size: 0.87rem; }
.joinlist-status:empty { margin: 0; }
.joinlist-status.is-ok { color: #2f6b3a; }
.joinlist-status.is-error { color: #9a2f2f; }

@media (max-width: 30rem) {
  .hero { gap: 0.9rem; }
  .hero-logo { width: 68px; }
  .hero-title { font-size: 1.4rem; }
  .joinlist button { flex: 1 1 100%; }
}
</style>

<div class="hero">
  <img class="hero-logo" src="{{ site.url }}{{ site.baseurl }}/assets/img/hrwg-logo.png" alt="UW Homelessness Research Working Group logo">
  <div>
    <h1 class="hero-title">UW Homelessness Research Working Group</h1>
    <p class="hero-tagline">A weekly interdisciplinary meeting space at the University of Washington</p>
  </div>
</div>

## Time and Location

<div class="meet-grid">
  <div>
    <img class="meet-photo" src="{{ site.url }}{{ site.baseurl }}/assets/img/savery.png" alt="Savery Hall, University of Washington">
    <ul class="meet-list">
      <li><strong>Location:</strong> <a href="https://www.washington.edu/maps/#!/sav">Savery Hall</a> Room 409</li>
      <li><strong>Time:</strong> 10:00 to 11:00 AM every Friday</li>
      <li><strong>Zoom (Hybrid):</strong> <a href="https://washington.zoom.us/meeting/register/w1KOov-0TXOTqpcVjueGlg">Registration Link</a></li>
    </ul>
  </div>
  <div class="meet-calendar">
    <iframe src="https://calendar.google.com/calendar/embed?src=c_8a4d342ffc52c6a6cd74d8b34194357db32be62ebd88f9ba47e235570c29e78e%40group.calendar.google.com&amp;ctz=America%2FLos_Angeles" frameborder="0" scrolling="no" title="Homelessness Research Working Group calendar"></iframe>
  </div>
</div>

### Faculty Sponsors

* [Zack W. Almquist](https://depts.washington.edu/zalmquist), Sociology
* [Amy Hagopian](https://sph.washington.edu/sph-profiles/faculty-profiles/amy-hagopian), Health Systems and Population Health

## Email List

<form class="joinlist" id="joinlist">
  <label class="joinlist-label" for="joinlist-email">Get meeting announcements and the weekly speaker schedule</label>
  <div class="joinlist-row">
    <input id="joinlist-email" name="email" type="email" inputmode="email" autocomplete="email"
           placeholder="you@uw.edu" aria-describedby="joinlist-note" required>
    <button type="submit">Join the list</button>
  </div>
  <p class="joinlist-status" id="joinlist-status" role="status" aria-live="polite"></p>
  <p class="joinlist-note" id="joinlist-note">
    Sign-up is confirmed on the UW Mailman page, which opens in a new tab. You can also
    <a href="https://lists.uw.edu/postorius/lists/kcpehworkinggroup.lists.uw.edu/">subscribe there directly</a>,
    or send a blank email to
    <a href="mailto:kcpehworkinggroup-join@lists.uw.edu">kcpehworkinggroup-join@lists.uw.edu</a>.
  </p>
</form>

<script>
(function () {
  var LIST_URL = "https://lists.uw.edu/postorius/lists/kcpehworkinggroup.lists.uw.edu/";
  var form = document.getElementById("joinlist");
  if (!form) return;
  var input = document.getElementById("joinlist-email");
  var status = document.getElementById("joinlist-status");

  form.addEventListener("submit", function (e) {
    e.preventDefault();
    var email = (input.value || "").trim();
    if (!email || !input.checkValidity()) {
      status.textContent = "Please enter a valid email address.";
      status.className = "joinlist-status is-error";
      input.focus();
      return;
    }
    // The UW list is Mailman/Postorius and is CSRF-protected, so the address cannot be
    // posted from here. Copy it instead so it only has to be pasted once on their form.
    var done = function (copied) {
      status.textContent = copied
        ? "Address copied. Paste it into the UW form in the new tab to finish."
        : "Opening the UW sign-up form in a new tab — enter " + email + " there to finish.";
      status.className = "joinlist-status is-ok";
      window.open(LIST_URL, "_blank", "noopener");
    };
    if (navigator.clipboard && navigator.clipboard.writeText) {
      navigator.clipboard.writeText(email).then(function () { done(true); }, function () { done(false); });
    } else {
      done(false);
    }
  });
})();
</script>

## Executive summary

The <u>Homelessness Research Working Group</u> at the University of Washington is a weekly interdisciplinary meeting space for UW faculty, students, and scientists to collaborate and interact with community members engaged in the homelessness care system.
